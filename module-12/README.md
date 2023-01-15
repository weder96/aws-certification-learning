<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Módulo 12: AWS Integration & Messaging

## Conteúdo
1. <a href="#section-1"> Amazon Simple Notification Service (Amazon SNS) </a>
2. <a href="#section-2"> Amazon Simple Queue Service (Amazon SQS) </a>
3. <a href="#section-3"> Amazon-MQ </a>
4. <a href="#section-4"> AWS-AppSync </a>
5. <a href="#section-5"> Amazon-AppFlow</a>
6. <a href="#section-6"> Amazon-API-Gateway</a>
7. <a href="#section-7"> Amazon-EventBridge</a>
8. <a href="#section-8"> AWS-Step-Functions</a>
9. <a href="#section-9"> AWS-Express-Workflows</a>
10. <a href="#section-10"> AWS-Console-Mobile-Application </a>
11. <a href="#section-11"> Amazon-Managed-Workflows-for-Apache-Airflow</a>



## <a id="section-1" > </a> **1 - Amazon Simple Notification Service (Amazon SNS)**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-Simple-Notification-Service_64.svg)

**Definition**

### What if you want to send one message to many receivers?

- The “event producer” only sends message to one SNS topic
- As many “event receivers” (subscriptions) as we want to listen to the SNS topic notifications
- Each subscriber to the topic will get all the messages (note: new feature to filter messages)
- Up to 12,500,000 subscriptions per topic
- 100,000 topics limit

### SNS integrates with a lot of AWS services

- CloudWatch Alarms 
- AWS Budgets
- Lambda
- Auto Scaling Group (Notifications)
- S3 Bucket (Events)
- DynamoDB
- CloudFormation (State Changes)
- AWS DMS (New Replic)
- RDS Events

### Amazon SNS – How to publish

- **Topic Publish (using the SDK)**
    - Create a topic
    - Create a subscription (or many)
    - Publish to the topic

- **Direct Publish (for mobile apps SDK)**
    - Create a platform application
    - Create a platform endpoint
    - Publish to the platform endpoint
    - Works with Google GCM, Apple APNS, Amazon ADM...

### Amazon SNS – Security

- **Encryption:**
    - In-flight encryption using HTTPS API
    - At-rest encryption using KMS keys
    - Client-side encryption if the client wants to perform encryption/decryption itself

- Access Controls: IAM policies to regulate access to the SNS API

- SNS Access Policies (similar to S3 bucket policies)
    - Useful for cross-account access to SNS topics
    - Useful for allowing other services ( S3...) to write to an SNS topic

### SNS + SQS: Fan Out

- Push once in SNS, receive in all SQS queues that are subscribers
- Fully decoupled, no data loss
- SQS allows for: data persistence, delayed processing and retries of work
- Ability to add more SQS subscribers over time
- Make sure your SQS queue access policy allows for SNS to write

### Application: S3 Events to multiple queues

- For the same combination of: event type (e.g. object create) and prefix (e.g. images/) you can only have one S3 Event rule
- If you want to send the same S3 event to many SQS queues, use fan-out

### Application: SNS to Amazon S3 through

- Kinesis Data Firehose


### Amazon SNS – FIFO Topic

- FIFO = First In First Out (ordering of messages in the topic)
- Similar features as SQS FIFO:
    - Ordering by Message Group ID (all messages in the same group are ordered)
    - Deduplication using a Deduplication ID or Content Based Deduplication
- Can only have SQS FIFO queues as subscribers
- Limited throughput (same throughput as SQS FIFO)

### SNS FIFO + SQS FIFO: Fan Out
- In case you need fan out + ordering + deduplication

### SNS – Message Filtering

- JSON policy used to filter messages sent to SNS topic’s subscriptions
- If a subscription doesn’t have a filter policy, it receives every message


**Cheat Sheets**

https://tutorialsdojo.com/amazon-sns/

**References**

https://docs.aws.amazon.com/sns/latest/dg

https://aws.amazon.com/sns/features/

https://aws.amazon.com/sns/pricing/

https://aws.amazon.com/sns/faqs/

**Videos**

https://www.youtube.com/results?search_query=aws+SNS

**Hands On**

https://www.youtube.com/results?search_query=aws+SNS+hands+on

-------------------------------------------------------------------------------------------------
## <a id="section-2" > </a> **2 - Amazon Simple Queue Service (Amazon SQS)**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-Simple-Queue-Service_64.svg)

**Definition**

-  Oldest offering (over 10 years old)
-  Fully managed service, used to decouple applications
-  Attributes:
    - Unlimited throughput, unlimited number of messages in queue
    - Default retention of messages: 4 days, maximum of 14 days
    - Low latency (<10 ms on publish and receive)
    - Limitation of 256KB per message sent
-  Can have duplicate messages (at least once delivery, occasionally)
-  Can have out of order messages (best effort ordering)

![sqs](../images/sqs.png)

### **SQS – Producing Messages**

- Produced to SQS using the SDK (SendMessage API)
- The message is persisted in SQS until a consumer deletes it
- Message retention: default 4 days, up to 14 day

- Example: send an order to be processed
- Order id
- Customer id
- Any attributes you want

![sqs](../images/sqs_send.png)

- Oldest offering (over 10 years old)
- Fully managed service, used to decouple applications
- Attributes:
    - Unlimited throughput, unlimited number of messages in queue
    - Default retention of messages: 4 days, maximum of 14 days
    - Low latency (<10 ms on publish and receive)
    - Limitation of 256KB per message sent
- Can have duplicate messages (at least once delivery, occasionally)
- Can have out of order messages (best effort ordering)

### **SQS – Consuming Messages**


- Consumers (running on EC2 instances, servers, or AWS Lambda)...
- Poll SQS for messages (receive up to 10 messages at a time)
- Process the messages (example: insert the message into an RDS database)
- Delete the messages using the DeleteMessage API

![sqs](../images/consumerSqs.png)

### **SQS – Multiple EC2 Instances Consumers**

- Consumers receive and process messages in parallel
- At least once delivery
- Best-effort message ordering
- Consumers delete messages after processing them
- We can scale consumers horizontally to improve throughput of processing

### **SQS with Auto Scaling Group (ASG)**

### **SQS to decouple between application tiers**

### **Amazon SQS - Security**

### **SQS Queue Access Policy**

### **SQS – Message Visibility Timeout**

### **Amazon SQS – Dead Letter Queue**

### **SQS DLQ – Redrive to Source**

### **Amazon SQS - Long Polling**

### **SQS – Request-Response Systems**

### **Amazon SQS – FIFO Queue**

- FIFO = First In First Out (ordering of messages in the queue)
- Limited throughput: 300 msg/s without batching, 3000 msg/s with
- Exactly-once send capability (by removing duplicates)
- Messages are processed in order by the consumer

**Cheat Sheets**

https://tutorialsdojo.com/amazon-sqs/

**References**

https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide

https://aws.amazon.com/sqs/features/

https://aws.amazon.com/sqs/pricing/

https://aws.amazon.com/sqs/faqs/


**Videos**

https://www.youtube.com/results?search_query=aws+SQS

**Hands On**

https://www.youtube.com/results?search_query=aws+SQS+hands+On

-------------------------------------------------------------------------------------------------
## <a id="section-3" > </a> **3 - Amazon-MQ**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-MQ_64.svg)

**Definition**
- SQS, SNS are “cloud-native” services: proprietary protocols from AWS
- Traditional applications running from on-premises may use open protocols such as: MQTT, AMQP, STOMP, Openwire, WSS
- When migrating to the cloud, instead of re-engineering the application to use SQS and SNS, we can use Amazon MQ
- Amazon MQ is a managed message broker service for
- Amazon MQ doesn’t “scale” as much as SQS / SNS
- Amazon MQ runs on servers, can run in Multi-AZ with failover
- Amazon MQ has both queue feature (~SQS) and topic features (~SNS)

AWS offering for a managed message broker service for Apache ActiveMQ. Message brokers allow different software systems–often using different programming languages, and on different platforms–to communicate and exchange information.
Amazon MQ also supports RabbitMQ, a popular open-source message broker. Migrate your existing RabbitMQ message brokers to AWS without having to rewrite code.


### **Features**

Amazon MQ uses industry-standard APIs and protocols for messaging, including Java Message Service (JMS), .NET Message Service (NMS), AMQP, STOMP, MQTT, OpenWire, and WebSocket.
Amazon MQ manages administrative tasks such as hardware provisioning, broker setup, software upgrades, and failure detection and recovery.
Amazon MQ stores your messages redundantly across multiple Availability Zones (AZs).
Amazon MQ supports both single-instance brokers, suitable for evaluation and testing, and active/standby brokers for high availability in production. In the event of a failure of the broker, or even a full AZ outage, Amazon MQ automatically fails over to the standby broker.



**Cheat Sheets**

https://tutorialsdojo.com/amazon-mq/

**References**

https://aws.amazon.com/amazon-mq/features/

https://docs.aws.amazon.com/amazon-mq/latest/developer-guide/welcome.html

https://aws.amazon.com/amazon-mq/pricing/

https://aws.amazon.com/amazon-mq/faqs/

https://aws.amazon.com/quickstart/architecture/ibm-mq/

https://aws-quickstart.s3.amazonaws.com/quickstart-ibm-mq/doc/ibm-mq-on-the-aws-cloud.pdf

**Videos**

https://www.youtube.com/results?search_query=aws+Amazon+MQ

**Hands On**

https://www.youtube.com/results?search_query=aws+Amazon+MQ+Hands+ON


-------------------------------------------------------------------------------------------------
## <a id="section-4" > </a> **4 - AWS-AppSync**

![AppSync](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_AWS-AppSync_64.svg)

**Definition**

A serverless GraphQL and Pub/Sub API service that streamlines the development of modern web and mobile applications

AppSync GraphQL APIs – provides a unified endpoint for securely querying and updating data from multiple databases, microservices, and APIs

AppSync Pub/Sub APIs – data updates are automatically published to subscribed API clients via serverless WebSockets connections.


### **Monitoring**

Use Amazon CloudWatch Logs to monitor your AWS AppSync GraphQL API and debug request issues.
You can use AWS X-Ray to trace GraphQL requests in AWS AppSync.
With AWS CloudTrail, you can log AWS AppSync API calls.


### **Security**

- In your API or CLI call, you can specify which authorization type you want:
    - API_KEY
    - AWS_LAMBDA
    - AWS_IAM
    - OPENID_CONNECT
    - AMAZON_COGNITO_USER_POOLS

- Using schema directives, you can specify additional authorization modes at the schema level.
- You can use AWS WAF to configure a set of rules to protect your web applications and APIs from attacks

### **Pricing**
- You are charged for the following:
    - Query and data modification operations.
    - Performing real-time updates on your data.
    - Minutes of connection to AppSync.
    - Dedicated cache instance.

**Cheat Sheets**

https://tutorialsdojo.com/aws-appsync/

**References**

https://aws.amazon.com/appsync/

https://docs.aws.amazon.com/appsync/latest/devguide/what-is-appsync.html

**Videos**

https://www.youtube.com/results?search_query=aws+appsync

**Hands On**

https://www.youtube.com/results?search_query=aws+appsync+hands+on

-------------------------------------------------------------------------------------------------
## <a id="section-5" > </a> **5 - Amazon-AppFlow**

![AppFlow](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-AppFlow_64.svg)

**Definition**

An integration service that automates data flows by securely integrating third-party applications and AWS services without writing any code.

### **Features**

- Run flows on-demand or on a schedule to keep data in sync across SaaS applications and AWS services.
- Aggregate data from multiple sources to train analytics tools more effectively and save money.
- Use flow management tools to track where and when data has moved.
- Data is encrypted at rest and in transit.
- Integrates with AWS PrivateLink to allow private data transfer over AWS rather than public data transfer over the internet.
- Use custom connectors to transfer data between private APIs, on-premise systems, and cloud services.
- Publish events related to the status of a flow using Amazon Event Bridge.

### **How it works**
- With Amazon AppFlow automate bi-directional data flows between SaaS applications and AWS services in just a few clicks. 
- Run the data flows at the frequency you choose, whether on a schedule, in response to a business event, or on demand. 
- Simplify data preparation with transformations, partitioning, and aggregation. 
- Automate preparation and registration of your schema with the AWS Glue Data Catalog so you can discover and share data with AWS analytics and machine learning services.

### **Pricing**

- You are charged per flow run and the maximum number of flow runs.
- You are charged for data processing for flows whose destinations are:
    - Hosted on AWS
    - Integrated with AWS PrivateLink
- You are charged per standard request and storage to read and write from AWS services.
- You are charged for the use of AWS KMS CMKs to encrypt access tokens and data in transit.



**Cheat Sheets**

https://tutorialsdojo.com/amazon-appflow/

**References**

https://aws.amazon.com/appflow/

https://docs.aws.amazon.com/appflow/index.html

https://docs.aws.amazon.com/pdfs/appflow/latest/userguide/appflow.pdf

**Videos**

https://www.youtube.com/results?search_query=aws+AppFlow

https://youtu.be/6NSxo5syl40


**Hands On**

https://www.youtube.com/results?search_query=aws+AppFlow+hands+on

-------------------------------------------------------------------------------------------------
## <a id="section-6" > </a> **6 - Amazon-API-Gateway**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-API-Gateway_64.svg)

**Definition**

**Cheat Sheets**

**References**

**Videos**

**Hands On**


-------------------------------------------------------------------------------------------------
## <a id="section-7" > </a> **7 - Amazon-EventBridge**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-EventBridge_64.svg)

**Definition**

### What Is Amazon EventBridge?

EventBridge is a serverless service that uses events to connect application components together, making it easier for you to build scalable event-driven applications. 
Use it to route events from sources such as home-grown applications, AWS services, and third- party software to consumer applications across your organization. EventBridge provides a simple and consistent way to ingest, filter, transform, and deliver events so you can build new applications quickly.

EventBridge event buses are well suited for many-to-many routing of events between eventdriven services. 

EventBridge Pipes (p. 90) is intended for point-to-point integrations between

### **Amazon EventBridge Pipes**

Amazon EventBridge Pipes connects sources to targets. It reduces the need for specialized knowledge and integration code when developing event driven architectures, fostering consistency across your company’s applications. To set up a pipe, you choose the source, add optional filtering, define optional enrichment, and choose the target for the event data.

EventBridge Pipes could be used to create an ecommerce system. Imagine that you have an API that contains customer metadata, such as shipping addresses. The source might be an Amazon SQS order received message. 

The pipe then sends that data to an Amazon API Gateway API enrichment that returns the customer information for that order. Final

**Cheat Sheets**


**References**

https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-tutorial.html

https://aws.amazon.com/eventbridge/?nc1=h_ls

https://aws.amazon.com/eventbridge/features/

https://docs.aws.amazon.com/eventbridge/index.html

https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html

https://docs.aws.amazon.com/pdfs/eventbridge/latest/userguide/user-guide.pdf#eb-what-is

**Videos**

https://www.youtube.com/watch?v=gCyOPHlp5Ic

https://www.youtube.com/watch?v=e3sevLjtIQg

https://www.youtube.com/results?search_query=Amazon+EventBridge


**Hands On**

https://www.youtube.com/results?search_query=Amazon+EventBridge+hands+On


-------------------------------------------------------------------------------------------------
## <a id="section-8" > </a> **8 - AWS-Step-Functions**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_AWS-Step-Functions_64.svg)

**Definition**

AWS Step Functions 
• Build serverless visual workflow to orchestrate your Lambda functions
• Features: sequence, parallel, conditions, timeouts, error handling, …
• Can integrate with EC2, ECS, On -premises servers, API Gateway, SQS queues
• Possibility of implementing human approval feature
• Use cases: order fulfillment, data processing, web applications, any workflow


AWS Step Functions is a web service that provides serverless orchestration for modern applications. It enables you to coordinate the components of distributed applications and microservices using visual workflows.

### **Pricing**

- Step Functions counts a state transition each time a step of your workflow is executed. You are charged for the total number of state transitions across all your state machines, including retries.
Common Use Cases

- Step Functions can help ensure that long-running, multiple ETL jobs execute in order and complete successfully, instead of manually orchestrating those jobs or maintaining a separate application.
- By using Step Functions to handle a few tasks in your codebase, you can approach the transformation of monolithic applications into microservices as a series of small steps.
- You can use Step Functions to easily automate recurring tasks such as patch management, infrastructure selection, and data synchronization, and Step Functions will automatically scale, respond to timeouts, and retry failed tasks.
- Use Step Functions to combine multiple AWS Lambda functions into responsive serverless applications and microservices, without having to - write code for workflow logic, parallel processes, error handling, timeouts or retries.
- You can also orchestrate data and services that run on Amazon EC2 instances, containers, or on-premises servers.

**Cheat Sheets**

https://tutorialsdojo.com/aws-step-functions/

**References**

https://aws.amazon.com/step-functions/features/

https://aws.amazon.com/step-functions/pricing/

https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html

https://aws.amazon.com/step-functions/faqs/

**Videos**

https://www.youtube.com/results?search_query=+AWS+Step+Functions

**Hands On**

https://www.youtube.com/results?search_query=+AWS+Step+Functions+hands+on

--------------------------------------------------------------------------------------------------------------------
## <a id="section-9" > </a> **9 - AWS-Express-Workflows**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_AWS-Express-Workflows_64.svg)

**Definition**

**Cheat Sheets**

**References**

**Videos**

**Hands On**

-------------------------------------------------------------------------------------------------
## <a id="section-10"></a> **10 - AWS-Console-Mobile-Application**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_AWS-Console-Mobile-Application_64.svg)

**Definition**

**Cheat Sheets**

**References**

**Videos**

**Hands On**

-------------------------------------------------------------------------------------------------
## <a id="section-11"></a> **11 - Amazon-Managed-Workflows-for-Apache-Airflow**

![SNS](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-Managed-Workflows-for-Apache-Airflow_64.svg)

**Definition**

**Cheat Sheets**

**References**

**Videos**

**Hands On**
