<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

Module 14: Serverless Design Principles

## Conteúdo
1. <a href="#section-1"> Serverless Overview </a>


## <a id="section-1" ></a> **1 - Serverless Overview**


**Definition**

-  Serverless is a new paradigm in which the developers don’t have to manage servers anymore...
-  They just deploy code
-  They just deploy... functions !
-  Initially... Serverless == FaaS (Function as a Service)
-  Serverless was pioneered by AWS Lambda but now also includes anything that’s managed: “databases, messaging, storage, etc.”
-  Serverless does not mean there are no servers... it means you just don’t manage / provision / see them

### **Serverless in AWS**

- AWS Lambda
- DynamoDB
- AWS Cognito
- AWS API Gateway
- Amazon S3
- AWS SNS & SQS
- AWS Kinesis Data Firehose
- Aurora Serverless
- Step Functions
- Fargate


### **Why AWS Lambda**

**Amazon EC2**
- Virtual Servers in the Cloud
- Limited by RAM and CPU
- Continuously running
- Scaling means intervention to add / remove servers

**Amazon Lambda**
- Virtual functions – no servers to manage!
- Limited by time - short executions
- Run on-demand
- Scaling is automated!

**Benefits of AWS Lambda**
-  Easy Pricing:
    -  Pay per request and compute time
    -  Free tier of 1,000,000 AWS Lambda requests and 400,000 GBs of compute time

-  Integrated with the whole AWS suite of services
-  Integrated with many programming languages
-  Easy monitoring through AWS CloudWatch
-  Easy to get more resources per functions (up to 10GB of RAM!)
-  Increasing RAM will also improve CPU and network!


**AWS Lambda language support**

- Node.js (JavaScript)
- Python
- Java (Java 8 compatible)
- C# (.NET Core)
- Golang
- C# / Powershell
- Ruby
- Custom Runtime API (community supported, example Rust)

- Lambda Container Image
    - The container image must implement the Lambda Runtime API
    - ECS / Fargate is preferred for running arbitrary Docker images


**AWS Lambda Integrations - Main ones**

- API Gateway
- CloudWatch Events EventBridge
- Kinesis 
- DynamoDB 
- S3 
- CloudFront
- CloudWatch Logs 
- SNS 
- SQS 
- Cognito


**Example: Serverless Thumbnail creation**
**Example: Serverless CRON Job**


**AWS Lambda Pricing:**

-  You can find overall pricing information here:
    https://aws.amazon.com/lambda/pricing/
-  Pay per calls:
    -  First 1,000,000 requests are free
    -  $0.20 per 1 million requests thereafter ($0.0000002 per request)

-  Pay per duration: (in increment of 1 ms)
    - 400,000 GB-seconds of compute time per month for FREE
    - 400,000 seconds if function is 1GB RAM
    - 3,200,000 seconds if function is 128 MB RAM
    - After that $1.00 for 600,000 GB-seconds

-  It is usually very cheap to run AWS Lambda so it’s very popular


**AWS Lambda Limits to Know - per region**

-  Execution:
    - Memory allocation: 128 MB – 10GB (1 MB increments)
    - Maximum execution time: 900 seconds (15 minutes)
    - Environment variables (4 KB)
    - Disk capacity in the “function container” (in /tmp): 512 MB
    - Concurrency executions: 1000 (can be increased)

-  Deployment:
    - Lambda function deployment size (compressed .zip): 50 MB
    - Size of uncompressed deployment (code + dependencies): 250 MB
    - Can use the /tmp directory to load other files at startup
    - Size of environment variables: 4 KB


**Lambda@Edge**


- You have deployed a CDN using CloudFront
- What if you wanted to run a global AWS Lambda alongside?
- Or how to implement request filtering before reaching your application?

- For this, you can use Lambda@Edge: deploy Lambda functions alongside your CloudFront CDN
    - Build more responsive applications
    - You don’t manage servers, Lambda is deployed globally
    - Customize the CDN content
    - Pay only for what you use

- You can use Lambda to change CloudFront requests and responses:
    - After CloudFront receives a request from a viewer (viewer request)
    - Before CloudFront forwards the request to the origin (origin request)
    - After CloudFront receives the response from the origin (origin response)
    - Before CloudFront forwards the response to the viewer (viewer response)


**Lambda@Edge: Use Cases**

- Website Security and Privacy
- Dynamic Web Application at the Edge
- Search Engine Optimization (SEO)
- Intelligently Route Across Origins and Data Centers
- Bot Mitigation at the Edge
- Real-time Image Transformation
- A/B Testing
- User Authentication and Authorization
- User Prioritization
- User Tracking and Analytics


**Cheat Sheets**

https://digitalcloud.training/aws-lambda/

https://tutorialsdojo.com/aws-lambda/

**References**

https://docs.aws.amazon.com/elasticloadbalancing/latest/application/lambda-functions.html

https://aws.amazon.com/pt/elasticloadbalancing/pricing/

https://aws.amazon.com/pt/lambda/pricing/

https://docs.aws.amazon.com/lambda/latest/dg

https://aws.amazon.com/lambda/features/

https://aws.amazon.com/lambda/faqs/

**Videos**

https://www.youtube.com/results?search_query=aws+Lambda

**Hands On**

https://www.youtube.com/results?search_query=aws+Lambda+hands+on





