<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [Conteudo Geral AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Additional AWS Services

## Conteúdo
1. <a href="#section-1"> Compute </a>
2. <a href="#section-2"> Database </a>
3. <a href="#section-3"> Networking & Content Delivery </a>
4. <a href="#section-4"> Developer Tools </a>
5. <a href="#section-5"> AWS Managed Services </a>
6. <a href="#section-6"> Analytics </a>
7. <a href="#section-7"> Media Services </a>
8. <a href="#section-8"> Mobile Services </a>
9. <a href="#section-9"> End User Computing </a>
10. <a href="#section-10"> Internet of Things (IoT) </a>


There are Additional AWS Services & Tools that may feature on the exam. Often you do not need to know these at a deep level but do need to understand what they are and what they are used for.

On this page, you’ll find some high-level details and links for more information on some of these services and tools.

Exam tip: Before sitting the exam, it would be wise to go through the AWS console and pick out any services you’re not familiar with and do a bit of reading up on them using the AWS documentation.

Note: If a service starts appearing regularly on the exam it may be moved to the main cheat sheet for the AWS service category.

**************************************************************************************
## <a id="section-1" ></a> **1 - Compute**
### [Amazon Elastic Container Service for Kubernetes (EKS)](https://aws.amazon.com/eks/features/)

Amazon Elastic Container Service for Kubernetes (EKS) is a managed Kubernetes service that makes it easy for you to run Kubernetes on AWS without needing to install, operate, and maintain your own Kubernetes control plane.

EKS is certified Kubernetes conformant, so existing applications running on upstream Kubernetes are compatible with Amazon EKS.

EKS automatically manages the availability and scalability of the Kubernetes control plane nodes that are responsible for starting and stopping containers, scheduling containers on virtual machines, storing cluster data, and other tasks.

EKS automatically detects and replaces unhealthy control plane nodes for each cluster.

Generally available but only in limited regions currently


**************************************************************************************
## <a id="section-2" ></a> **2 - Database**
### [Amazon Neptune](https://aws.amazon.com/neptune/features/)

Amazon Neptune is a fast, reliable, fully managed graph database service that makes it easy to build and run applications that work with highly connected datasets.

With Amazon Neptune, you can create sophisticated, interactive graph applications that can query billions of relationships in milliseconds.

SQL queries for highly connected data are complex and hard to tune for performance. Instead, Amazon Neptune allows you to use the popular graph query languages Apache TinkerPop Gremlin and W3C’s SPARQL to execute powerful queries that are easy to write and perform well on connected data

### [AWS Migration Hub](https://aws.amazon.com/migration-hub/features/)
AWS Migration Hub provides a single location to track the progress of application migrations across multiple AWS and partner solutions.

Using Migration Hub allows you to choose the AWS and partner migration tools that best fit your needs, while providing visibility into the status of migrations across your portfolio of applications.

For example, you might use AWS Database Migration Service, AWS Server Migration Service, and partner migration tools such as ATADATA ATAmotion, CloudEndure Live Migration, or RiverMeadow Server Migration SaaS to migrate an application comprised of a database, virtualized web servers, and a bare metal server.

Using Migration Hub, you can view the migration progress of all the resources in the application.

### [AWS Database Migration Service](https://aws.amazon.com/dms/)
AWS Database Migration Service helps you migrate databases to AWS quickly and securely.

The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database.

The AWS Database Migration Service can migrate your data to and from most widely used commercial and open-source databases.

AWS Database Migration Service supports homogenous migrations such as Oracle to Oracle, as well as heterogeneous migrations between different database platforms, such as Oracle or Microsoft SQL Server to Amazon Aurora.

With AWS Database Migration Service, you can continuously replicate your data with high availability and consolidate databases into a petabyte-scale data warehouse by streaming data to Amazon Redshift and Amazon S3.
    

### [AWS Server Migration Service](https://aws.amazon.com/server-migration-service/)
AWS Server Migration Service (SMS) is an agentless service which makes it easier and faster for you to migrate thousands of on-premises workloads to AWS

AWS SMS allows you to automate, schedule, and track incremental replications of live server volumes, making it easier for you to coordinate large-scale server migrations

**************************************************************************************
## <a id="section-3" ></a> **3 - Networking & Content Delivery**
### [Amazon API Gateway](https://aws.amazon.com/api-gateway/features/)
Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.

With a few clicks in the AWS Management Console, you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services.

Back-end services may include Amazon Elastic Compute Cloud (Amazon EC2), code running on AWS Lambda, or any web application.

**************************************************************************************
## <a id="section-4" ></a> **4 - Developer Tools**
### [AWS CodeStar](https://aws.amazon.com/codestar/features/)
AWS CodeStar enables you to quickly develop, build, and deploy applications on AWS. AWS CodeStar provides a unified user interface, enabling you to easily manage your software development activities in one place.

With AWS CodeStar, you can set up your entire continuous delivery toolchain in minutes, allowing you to start releasing code faster. AWS CodeStar makes it easy for your whole team to work together securely, allowing you to easily manage access and add owners, contributors, and viewers to your projects.

With AWS CodeStar, you can use a variety of project templates to start developing applications on Amazon EC2, AWS Lambda, and AWS Elastic Beanstalk.

AWS CodeStar projects support many popular programming languages including Java, JavaScript, PHP, Ruby, and Python.

### [AWS CodeCommit](https://aws.amazon.com/codecommit/features/)
AWS CodeCommit is a fully managed source control service that hosts secure Git-based repositories.

It makes it easy for teams to collaborate on code in a secure and highly scalable ecosystem.

CodeCommit eliminates the need to operate your own source control system or worry about scaling its infrastructure.

You can use CodeCommit to securely store anything from source code to binaries, and it works seamlessly with your existing Git tools.

### [AWS CodeBuild](https://aws.amazon.com/codebuild/features/)
AWS CodeBuild is a fully managed continuous integration service that compiles source code, runs tests, and produces software packages that are ready to deploy.

With CodeBuild, you don’t need to provision, manage, and scale your own build servers. CodeBuild scales continuously and processes multiple builds concurrently, so your builds are not left waiting in a queue.

You can get started quickly by using prepackaged build environments, or you can create custom build environments that use your own build tools.

With CodeBuild, you are charged by the minute for the compute resources you use.

### [AWS CodeDeploy](https://aws.amazon.com/codedeploy/features/)
AWS CodeDeploy is a fully managed deployment service that automates software deployments to a variety of compute services such as Amazon EC2, AWS Lambda, and your on-premises servers.

AWS CodeDeploy makes it easier for you to rapidly release new features, helps you avoid downtime during application deployment, and handles the complexity of updating your applications.

You can use AWS CodeDeploy to automate software deployments, eliminating the need for error-prone manual operations. The service scales to match your deployment needs, from a single Lambda function to thousands of EC2 instances.


### [AWS CodePipeline](https://aws.amazon.com/codepipeline/features/)
AWS CodePipeline is a fully managed continuous delivery service that helps you automate your release pipelines for fast and reliable application and infrastructure updates.

CodePipeline automates the build, test, and deploy phases of your release process every time there is a code change, based on the release model you define.

This enables you to deliver features and updates rapidly and reliably.

You can easily integrate AWS CodePipeline with third-party services such as GitHub or with your own custom plugin.

### [AWS X-Ray](https://aws.amazon.com/xray/features/)
AWS X-Ray helps developers analyze and debug production, distributed applications, such as those built using a microservices architecture.    

With X-Ray, you can understand how your application and its underlying services are performing to identify and troubleshoot the root cause of performance issues and errors.

X-Ray provides an end-to-end view of requests as they travel through your application and shows a map of your application’s underlying components.

You can use X-Ray to analyze both applications in development and in production, from simple three-tier applications to complex microservices applications consisting of thousands of service. [servicecatalog](https://aws.amazon.com/servicecatalog/features/)

**************************************************************************************
## <a id="section-5" ></a> **5 - AWS Managed Services**

[AWS Managed Services](https://aws.amazon.com/managed-services/#) provides ongoing management of your AWS infrastructure so you can focus on your applications.

By implementing best practices to maintain your infrastructure, AWS Managed Services helps to reduce your operational overhead and risk.

AWS Managed Services automates common activities such as change requests, monitoring, patch management, security, and backup services, and provides full-lifecycle services to provision, run, and support your infrastructure.

AWS Managed Services delivers consistent operations management and predictable results by following ITIL® best practices, and provides tooling and automation to increase efficiency, and reduce your operational overhead and risk.
    
**************************************************************************************
## <a id="section-6" ></a> **6 - Analytics**
### [Amazon Athena](https://aws.amazon.com/athena/features/)
Amazon Athena is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL.

Athena is serverless, so there is no infrastructure to manage, and you pay only for the queries that you run.

With a few clicks in the AWS Management Console, customers can point Athena at their data stored in S3 and begin using standard SQL to run ad-hoc queries and get results in seconds.

You can use Athena to process logs, perform ad-hoc analysis, and run interactive queries

Athena scales automatically – executing queries in parallel – so results are fast, even with large datasets and complex queries.
    
### [Amazon EMR](https://aws.amazon.com/emr/features/)
Amazon Elastic Map Reduce (EMR) provides a managed Hadoop framework that makes it easy, fast, and cost-effective to process vast amounts of data across dynamically scalable Amazon EC2 instances.

You can also run other popular distributed frameworks such as Apache Spark, HBase, Presto, and Flink in Amazon EMR, and interact with data in other AWS data stores such as Amazon S3 and Amazon DynamoDB.

Amazon EMR securely and reliably handles a broad set of big data use cases, including log analysis, web indexing, data transformations (ETL), machine learning, financial analysis, scientific simulation, and bioinformatic.
    
### [Amazon CloudSearch](https://aws.amazon.com/cloudsearch/)

Amazon CloudSearch is a managed service in the AWS Cloud that makes it simple and cost-effective to set up, manage, and scale a search solution for your website or application.

Amazon CloudSearch supports 34 languages and popular search features such as highlighting, autocomplete, and geospatial search.

### [Amazon Elasticsearch](https://aws.amazon.com/elasticsearch-service/features/)
Amazon Elasticsearch Service is a fully managed service that makes it easy for you to deploy, secure, operate, and scale Elasticsearch to search, analyze, and visualize data in real-time.

With Amazon Elasticsearch Service you get easy-to-use APIs and real-time analytics capabilities to power use-cases such as log analytics, full-text search, application monitoring, and clickstream analytics, with enterprise-grade availability, scalability, and security.
    

### [Amazon Kinesis](https://aws.amazon.com/kinesis/)
Amazon Kinesis makes it easy to collect, process, and analyze real-time, streaming data so you can get timely insights and react quickly to new information.

There are four types of Kinesis service:
- **Kinesis Video Streams** makes it easy to securely stream video from connected .devices to AWS for analytics, machine learning (ML), and other processing.
- **Kinesis Data Streams** enables you to build custom applications that process or analyze streaming data for specialized needs.
- **Kinesis Data Firehose** is the easiest way to load streaming data into data stores and analytics tools.
- **Amazon Kinesis Data Analytics** is the easiest way to process and analyze real-time, streaming data.
    
### [AWS Data Pipeline](https://aws.amazon.com/datapipeline/)
AWS Data Pipeline is a web service that helps you reliably process and move data between different AWS compute and storage services, as well as on-premises data sources, at specified intervals.

With AWS Data Pipeline, you can regularly access your data where it’s stored, transform, and process it at scale, and efficiently transfer the results to AWS services such as Amazon S3, Amazon RDS, Amazon DynamoDB, and Amazon EMR.

AWS Data Pipeline helps you easily create complex data processing workloads that are fault tolerant, repeatable, and highly available.

### [AWS Glue](https://aws.amazon.com/glue/features/)
AWS Glue is a fully managed extract, transform, and load (ETL) service that makes it easy for customers to prepare and load their data for analytics.

You can create and run an ETL job with a few clicks in the AWS Management Console.

You simply point AWS Glue to your data stored on AWS, and AWS Glue discovers your data and stores the associated metadata (e.g. table definition and schema) in the AWS Glue Data Catalog.

Once cataloged, your data is immediately searchable, queryable, and available for ETL.

AWS Glue generates the code to execute your data transformations and data loading processes.


## <a id="section-7" ></a> **7 - Media Services**
### [Amazon Elastic Transcoder](https://aws.amazon.com/elastictranscoder/)
Amazon Elastic Transcoder is media transcoding in the cloud.

It is designed to be a highly scalable, easy to use and a cost-effective way for developers and businesses to convert (or “transcode”) media files from their source format into versions that will playback on devices like smartphones, tablets, and PCs.

**************************************************************************************
## <a id="section-8" ></a> **8 - Mobile Services**
### [AWS AppSync](https://aws.amazon.com/appsync/product-details/)
AWS AppSync makes it easy to build data-driven mobile and browser-based apps that deliver responsive, collaborative experiences by keeping the data updated when devices are connected, enabling the app to use local data when offline, and synchronizing the data when the devices reconnect.

AWS AppSync uses the open standard GraphQL query language so you can request, change, and subscribe to the exact data you need with just a few lines of code.

### [AWS Device Farm](https://aws.amazon.com/device-farm/)

AWS Device Farm is an app testing service that lets you test and interact with your Android, iOS, and web apps on many devices at once, or reproduce issues on a device in real time.

View video, screenshots, logs, and performance data to pinpoint and fix issues and increase quality before shipping your app.
**************************************************************************************
## <a id="section-9" ></a> **9 - End User Computing**
### [Amazon Workspaces](https://aws.amazon.com/workspaces/features/)

Amazon WorkSpaces is a managed, secure cloud desktop service. You can use Amazon WorkSpaces to provision either Windows or Linux desktops in just a few minutes and quickly scale to provide thousands of desktops to workers across the globe.

Amazon WorkSpaces offers you an easy way to provide a secure, managed, cloud-based virtual desktop experience to your end-users.

Unlike traditional on-premises Virtual Desktop Infrastructure (VDI) solutions, you don’t have to worry about procuring, deploying, and managing a complex environment – Amazon WorkSpaces takes care of the heavy lifting and provides a fully managed service.

### [AWS AppStream](https://aws.amazon.com/appstream2/features/)
Fully managed non-persistent application streaming service.

Alternative to popular products such as Citrix XenApp.


### [AWS WorkLink](https://aws.amazon.com/worklink/features/)
Provides secure, one-click access to your internal websites and web apps using mobile phone browsers.

Does not require VPN client or App.


### [AWS WorkDocs](https://aws.amazon.com/workdocs/features/)
Fully managed, secure content creation, storage, and collaboration service

Create, edit, and share content that’s centrally stored on AWS.

**************************************************************************************
## <a id="section-10" ></a> **10 - Internet of Things (IoT)**

### [AWS IoT Core](https://aws.amazon.com/iot-core/features/)

Describes the network of physical objects that are embedded with sensors or software.

Each IoT device can communicate and exchange data with other devices and systems.
Use cases include:
- Smart home automation.
- Smart healthcare.
- Manufacturing.
- Agriculture.

Allows you to connect IoT devices to the AWS cloud without the need to provision or manage servers.

Can support billions of devices and trillions of messages.

