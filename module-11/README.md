<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [Conteudo Geral AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Módulo 11: AWS Analytics Services

## Conteúdo
1. <a href="#section-1"> Amazon Elastic Map Reduce (Amazon EMR)</a>
2. <a href="#section-2"> Amazona Athena</a>
3. <a href="#section-3"> AWS Glue</a>
4. <a href="#section-4"> Data Analysis and Query Use Cases</a>
5. <a href="#section-5"> Amazon Kinesis</a>
6. <a href="#section-6"> Amazon Kinesis Video Streams</a>
7. <a href="#section-7"> Amazon Kinesis Data Streams</a>
8. <a href="#section-8"> Amazon Kinesis Data Firehose</a>
9. <a href="#section-9"> Amazon Kinesis Data Analytics</a>
10. <a href="#section-10"> Amazon OpenSearch </a>
11. <a href="#section-11"> Amazon Data Exchange </a>
12. <a href="#section-12"> Amazon Data Pipeline </a>
13. <a href="#section-13"> Amazon CloudSearch </a>
14. <a href="#section-14"> Amazon Lake Formation </a>
------------------------------------------------------------------------------------------------------------------------

There are several AWS Analytics services and they include:

- Amazon Athena 
- Amazon Data Exchange
- Amazon Data Pipeline
- Amazon Amazon Elastic Map Reduce(Amazon EMR)
- Amazon Glue
- Amazon Kinesis
- Amazon Lake Formation
- Amazon Managed Streaming for Apache Kafka (Amazon MSK)
- Amazon OpenSearch Service (Amazon Elasticsearch Service)
- Amazon QuickSight
- Amazon Redshift

Below, we will have an analysis of each one, as these are the services most likely
You may also want to follow the links to the other services and read on to understand what they are at a high level.
But here we will try to explain each one and its advantages and also its disadvantages, as well as the links
for you to delve deeper.

------------------------------------------------------------------------------------------------------------------------

## <a id="section-1" ></a> **1 - Amazon Elastic Map Reduce**
![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-EMR_48.png)

Amazon EMR is a web service that enables companies, researchers, data analysts, and developers to process large amounts of data easily and cost-effectively.

EMR uses a hosted Hadoop framework running on Amazon EC2 and Amazon S3.

Managed Hadoop framework for processing large amounts of data.

It also supports Apache Spark, HBase, Presto and Flink.

Most commonly used for log analysis, financial analysis, or extract, translate, and load (ETL) activities.

A Step is a programmatic task to perform some process on the data (eg count words).

A cluster is a collection of EC2 instances provisioned by EMR to run its steps.

EMR uses Apache Hadoop as its distributed data processing engine, which is an open source Java software framework that supports data-intensive distributed applications running on large clusters of common hardware.

EMR is a good place to deploy Apache Spark, an open source distributed processing used for big data workloads that utilizes in-memory caching and optimized query execution.

You can also start Presto clusters. Presto is an open source distributed SQL query engine designed for fast analytical queries on large datasets.

EMR starts all nodes in a given cluster in the same Amazon EC2 Availability Zone.

You can access Amazon EMR using the AWS Management Console, Command Line Tools, SDKS, or the EMR API.

With EMR you have access to the underlying operating system (you can use SSH).

------------------------------------------------------------------------------------------------------------------------
## <a id="section-2" ></a> **2 - Amazon Athena**
![Amazon Athena](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-Athena_48.png)

Amazon Athena is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL.

Athena is serverless, so there is no infrastructure to manage and you only pay for the queries you run.

Athena is easy to use – just point to your data in Amazon S3, define the schema and start querying using standard SQL.

Amazon Athena uses Presto with full support for standard SQL and works with many standard data formats, including CSV, JSON, ORC, Apache Parquet, and Avro.

While Amazon Athena is ideal for fast, ad-hoc queries and integrates with Amazon QuickSight for easy visualization, it can also handle complex analysis, including large joins, window functions, and arrays.

Amazon Athena uses a managed data catalog to store information and schemas about the databases and tables you create for your data stored in Amazon S3.

[digitalcloud.training](https://digitalcloud.training/amazon-athena/)

[https://tutorialsdojo.com/amazon-athena/](https://tutorialsdojo.com/amazon-athena/)

[AWS Knowledge Center Videos: How do I analyze my S3 logs using Athena?](https://www.youtube.com/watch?v=uoLsrKZha0E&t=9s)

**References:**

[https://docs.aws.amazon.com/athena/latest/ug/](https://docs.aws.amazon.com/athena/latest/ug/)

[https://aws.amazon.com/athena/features](https://aws.amazon.com/athena/features)

[https://aws.amazon.com/athena/pricing](https://aws.amazon.com/athena/pricing)

[https://aws.amazon.com/athena/faqs](https://aws.amazon.com/athena/faqs)

------------------------------------------------------------------------------------------------------------------------
## <a id="section-3"></a> **3 - AWS Glue**
![AWS Glue](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_AWS-Glue_48.png)

AWS Glue is a fully managed, pay-as-you-go, extract, transform, and load (ETL) service that automates the time-consuming steps of preparing data for analysis.

AWS Glue automatically discovers and profiles through the Glue Data Catalog, recommends and generates ETL code to transform your source data into target schemas.

AWS Glue runs your ETL jobs in a fully managed and scalable Apache Spark environment to load your data to your destination.

AWS Glue also lets you configure, orchestrate, and monitor complex data flows.

You can create and run an ETL job with just a few clicks from the AWS Management Console.

Use AWS Glue to discover data properties, transform it, and prepare it for analysis.

Glue can automatically discover structured and semi-structured data stored in data lakes on Amazon S3, data warehouses on Amazon Redshift, and multiple databases running on AWS.

It provides a unified view of data through the Glue Data Catalog which is available for ETL, querying and reporting using services such as Amazon Athena, Amazon EMR and Amazon Redshift Spectrum.

Glue automatically generates Scala or Python code for ETL jobs that you can further customize using tools you are already familiar with.

AWS Glue is serverless, so there are no compute resources to configure and manage.

[https://digitalcloud.training/aws-glue/](https://digitalcloud.training/aws-glue/)

[https://tutorialsdojo.com/aws-glue/](https://tutorialsdojo.com/aws-glue/)

**References:**

[https://aws.amazon.com/glue/faqs/](https://aws.amazon.com/glue/faqs/)

[https://docs.aws.amazon.com/glue/latest/dg/what-is-glue.html](https://docs.aws.amazon.com/glue/latest/dg/what-is-glue.html)


**AWS Glue Databrew**

![AWS Glue Databrew](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_AWS-Glue-DataBrew_48.png)

AWS Glue DataBrew is a new visual data preparation tool that makes it easy for data analysts and data scientists to clean and normalize data to prepare it for analytics and machine learning. You can choose from over 250 pre-built transformations to automate data preparation tasks, all without the need to write any code. You can automate filtering anomalies, converting data to standard formats, and correcting invalid values, and other tasks. After your data is ready, you can immediately use it for analytics and machine learning projects. You only pay for what you use - no upfront commitment

[https://aws.amazon.com/glue/features/databrew/](https://aws.amazon.com/glue/features/databrew/)



**AWS Glue Elastic Views**

![AWS Glue Databrew](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_AWS-Glue-Elastic-Views_48.png)


------------------------------------------------------------------------------------------------------------------------
## <a id="section-4"></a> **4 - Data Analysis and Query Use Cases**
Query services like Amazon Athena, data warehouses like Amazon Redshift, and sophisticated data processing frameworks like Amazon EMR all address different needs and use cases.

Amazon Redshift provides the fastest query performance for enterprise reporting and business intelligence workloads, particularly those involving extremely complex SQL with multiple joins and subqueries.

Amazon EMR makes it simple and cost-effective to run highly distributed processing frameworks such as Hadoop, Spark, and Presto compared to on-premises deployments. Amazon EMR is flexible – you can run custom applications and code and define specific compute, memory, storage, and application parameters to optimize your analytical requirements.

Amazon Athena provides the easiest way to run ad-hoc queries for data on S3 without having to configure or manage servers.

**The table below shows the main use case and situations for using some AWS query and analysis services:**

|AWS Service | Main use case | When to use |
|-------------|----------------------|-------------|
|Amazon Athena |Query |Run interactive queries on data directly in Amazon S3 without worrying about formatting the data or managing the infrastructure. Can be used with other services such as Amazon RedShift| 
|Amazon RedShift|Data Warehouse | Extract data from multiple sources, format and organize it, store it, and support complex, high-speed queries that produce business reports. |
|Amazon EMR | Data Processing | Highly distributed processing frameworks such as Hadoop, Spark and Presto. Perform a wide variety of data processing tasks at scale-out for applications such as machine learning, graph analysis, data transformation, streaming data.|
|AWS Glue | ETL Service | Transform and move data to multiple destinations. Used to prepare and load data for analysis. The data source can be S3, RedShift or another database. The Glue Data Catalog can be consulted by Athena, EMR and RedShift Spectrum|

------------------------------------------------------------------------------------------------------------------------
## <a id="section-5"></a> **5 - Kinesis**
Amazon Kinesis makes it easy to collect, process, and analyze streaming data in real time so you can gain timely insights and react quickly to new information.

- Collection services for processing streams of various data.
- Data is processed in “fragments(Shards)”.
- There are **four types of Kinesis service**, detailed below.

------------------------------------------------------------------------------------------------------------------------
## <a id="section-6"></a> **6 - Kinesis Video Streams**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-Kinesis_48.png)

Kinesis Video Streams makes it easy to securely stream video from device
those connected to AWS for analytics, machine learning (ML), and other processing.

Durably stores, encrypts and indexes video data streams and allows access to the data through easy-to-use APIs.
- Producers provide data streams.
- Stores data for 24 hours by default, up to 7 days.
- Consumers receive and process data.
- Can have multiple fragments in a stream.
- Supports encryption at rest with server-side encryption (KMS) with a client master key

------------------------------------------------------------------------------------------------------------------------
## <a id="section-7"></a> **7 - Kinesis Data Streams**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-Kinesis-Data-Streams_48.png)

Kinesis Data Streams lets you build custom applications that process or analyze streaming data for specialized needs.

Kinesis Data Streams enables real-time processing of streaming big data.

Kinesis Data Streams is useful for quickly moving data from data producers and continuously processing it.

Kinesis Data Streams stores data for further processing by applications (key difference with Firehose, which delivers data directly to AWS services).

Common use cases include:
- Accelerated registration and data feed ingestion.
- Real-time metrics and reports.
- Real-time data analysis.
- Complex stream processing.

------------------------------------------------------------------------------------------------------------------------
## <a id="section-8"></a> **8 - Kinesis Data Firehose**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-Kinesis-Firehose_48.png)

Kinesis Data Firehose is the easiest way to load streaming data into data stores and analytics tools.

Captures, transforms and loads streaming data.

Enables near real-time analytics with existing business intelligence tools and dashboards.

Kinesis Data Streams can be used as source(s) for Kinesis Data Firehose.

You can configure Kinesis Data Firehose to transform your data before you deliver it.

With Kinesis Data Firehose, you don't have to write an application or manage resources.

Firehose can bundle, compress, and encrypt data before loading.

Firehose synchronously replicates data across three AZs as it travels to destinations.

Each delivery stream stores data records for up to 24 hours.

------------------------------------------------------------------------------------------------------------------------
## <a id="section-9"></a> **9 - Kinesis Data Analytics**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-Kinesis-Data-Analytics_48.png)

Amazon Kinesis Data Analytics is the easiest way to process and analyze streaming data in real time.

Can use standard SQL queries to process Kinesis data streams.

Provides real-time analytics.
Use cases:
- Generate time series analyses.
- Power panels in real time.
- Create real-time alerts and notifications.
- Quickly create and execute powerful SQL code in streaming sources.

It can ingest data from Kinesis Streams and Kinesis Firehose.

Output to S3, RedShift, Elasticsearch and Kinesis Data Streams.

It sits on top of Kinesis Data Streams and Kinesis Data Firehose.

------------------------------------------------------------------------------------------------------------------------
## <a id="section-10"></a> **10 - Amazon OpenSearch**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-OpenSearch-Service_48.png)

Amazon OpenSearch Service is the successor to Amazon Elasticsearch Service.

Amazon OpenSearch Service is an open source distributed research and analytics package based on Elasticsearch.

Elasticsearch is a distributed search and analysis engine built on Apache Lucene.

Elasticsearch is a popular search engine commonly used for log analytics, full-text search, security intelligence, business analytics, and operational intelligence use cases.

With OpenSearch, you can interactively perform log analysis, perform real-time application monitoring, site search, analyze performance metrics, and much more.

You can choose from a variety of open source engine options for your OpenSearch cluster.

Options include the latest version of OpenSearch and many versions of ALv2 Elasticsearch.

<img src="../images/aws/graphical-user-interface-description-automaticall.png" alt="graphical-user-interface-description-automaticall.png" width=90% height=300 />
<br/><br/><br/>

### **Deployment and Monitoring**

An OpenSearch cluster can be created using the AWS Management Console, API, or AWS CLI.

Specify the number of instances, instance types, and storage options.

In-place upgrades can be performed without downtime.

Provides built-in monitoring and alerts with automatic notifications.

You can configure alerts using Kibana or OpenSearch dashboards and the REST API.

Notifications can be sent via custom webhooks, Slack, Amazon SNS, and Amazon Chime.

The OpenSearch service supports multiple query languages ​​such as:

**Domain-Specific Language (DSL).**
- SQL queries with OpenSearch SQL.
- OpenSearch piped processing language (PPL).

**OpenSearch integrates with open source tools including:**
- Logstash.
- OpenTelemetry.
- ElasticSearch APIs.

### **OpenSearch in an Amazon VPC**

OpenSearch Services domains can run in an Amazon VPC.

Using a VPC allows secure communication between the OpenSearch Service and other services in the VPC.

Here are some of the differences between VPC domains and public domains.
- Because of their logical isolation, domains that reside in a VPC have an extra layer of security compared to domains that use public endpoints.
- While public domains are accessible from any device connected to the internet, VPC domains require some form of VPN or proxy.
- Compared to public domains, VPC domains display less information in the console. Specifically, the cluster health tab does not include shards information and the Indexes tab is not present.
- Domain endpoints take different forms (https://search-domain-name vs. https://vpc-domain-name).
- You cannot apply IP-based access policies to domains that reside in a VPC because security groups already enforce IP-based access policies.

**Please note the following limitations:**
- If you start a new domain in a VPC, you cannot later switch it to use a public endpoint. The opposite is also true.
- You can launch your domain in a VPC or use a public endpoint, but you cannot do both.
- You cannot launch your domain in a VPC that uses dedicated tenancy. You must use a VPC with tenancy set to Default.
- Once you place a domain in a VPC, you cannot move it to a different VPC, but you can change the subnets and security groups settings.
- To access the default installation of OpenSearch Dashboards for a domain residing in a VPC, users must have access to the VPC.

### **The ELK Stack**
ELK is an acronym that describes a popular combination of projects: Elasticsearch, Logstash, and Kibana.

The ELK stack gives you the ability to aggregate logs from all your systems and applications, analyze those logs, and create views.

ELK is useful for visualizing application and infrastructure monitoring data, troubleshooting, security analysis, and more.

### **Safety**
OpenSearch service domains offer data encryption at rest.

Uses AWS KMS for encryption key storage and management.

Encryption uses AES-256.

Encryption also encrypts node-to-node communications using TLS 1.2.

Node-to-node encryption is optional and can be enabled through the console, CLI, or API.

Once node-to-node encryption is enabled, it cannot be disabled. Instead, you must create a new domain from a snapshot without this setting enabled.

Amazon OpenSearch Service supports three types of access policies:
- Resource-based policies
- Identity-based policies
- IP-based policies

Fine-grained access control provides additional features in Amazon OpenSearch Service.

**Fine access control offers the following benefits:**
- Role-based access control.
- Index, document and field level security.
- OpenSearch Dashboards multi-tenancy.
- Basic HTTP authentication for OpenSearch and OpenSearch dashboards.

OpenSearch Service supports authentication through SAML and Amazon Cognito.


------------------------------------------------------------------------------------------------------------------------

## <a id="section-11" ></a> **11 - AWS Data Exchange**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_AWS-Data-Exchange_48.png)

**AWS Data Exchange advantage**

AWS Data Exchange is on a mission to increase speed to value for third-party data sets in the cloud.

There is no other place where customers can find data files, data tables, and data APIs from a vast portfolio of third-party data sets. We continuously innovate to make the world's third-party data easy to find in one data catalog, simple to subscribe to with consistent pricing options, and seamless to use with AWS data and analytics and machine learning services.

Create personalized mobile experiences with third-party data
90% of consumers believe that a brand’s ability to personalize their shopping experience impacts the amount they spend/shop with that brand. Read our latest article and learn
how you create personalized mobile experiences using data from AWS Data Exchange.


[https://aws.amazon.com/data-exchange/?nc1=h_ls](https://aws.amazon.com/data-exchange/?nc1=h_ls)

[https://www.youtube.com/watch?v=Lu9QVJ0Rml4](https://www.youtube.com/watch?v=Lu9QVJ0Rml4)

[https://www.youtube.com/watch?v=VpIdwc3zLlo&list=PLhr1KZpdzukeyNGiv3gE8m3_jMNNbxNkJ](https://www.youtube.com/watch?v=VpIdwc3zLlo&list=PLhr1KZpdzukeyNGiv3gE8m3_jMNNbxNkJ)


------------------------------------------------------------------------------------------------------------------------

## <a id="section-12" ></a> **11 - AWS Data Pipeline**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_AWS-Data-Pipeline_48.png)

### **What is AWS Data Pipeline?**

AWS Data Pipeline is a web service that you can use to automate the movement and transformation of data. With AWS Data Pipeline, you can define data-driven workflows, so that tasks can be dependent on the successful completion of previous tasks. You define the parameters of your data transformations and AWS Data Pipeline enforces the logic that you've set up.

The following components of AWS Data Pipeline work together to manage your data:

A pipeline definition specifies the business logic of your data management. For more information, see Pipeline Definition File Syntax.

A pipeline schedules and runs tasks by creating Amazon EC2 instances to perform the defined work activities. You upload your pipeline definition to the pipeline, and then activate the pipeline. You can edit the pipeline definition for a running pipeline and activate the pipeline again for it to take effect. You can deactivate the pipeline, modify a data source, and then activate the pipeline again. When you are finished with your pipeline, you can delete it.

Task Runner polls for tasks and then performs those tasks. For example, Task Runner could copy log files to Amazon S3 and launch Amazon EMR clusters. Task Runner is installed and runs automatically on resources created by your pipeline definitions. You can write a custom task runner application, or you can use the Task Runner application that is provided by AWS Data Pipeline. For more information, see Task Runners.

For example, you can use AWS Data Pipeline to archive your web server's logs to Amazon Simple Storage Service (Amazon S3) each day and then run a weekly Amazon EMR (Amazon EMR) cluster over those logs to generate traffic reports. AWS Data Pipeline schedules the daily tasks to copy data and the weekly task to launch the Amazon EMR cluster. AWS Data Pipeline also ensures that Amazon EMR waits for the final day's data to be uploaded to Amazon S3 before it begins its analysis, even if there is an unforeseen delay in uploading the logs.

[https://tutorialsdojo.com/aws-data-pipeline/](https://tutorialsdojo.com/aws-data-pipeline/)

[https://docs.aws.amazon.com/datapipeline/latest/DeveloperGuide/datapipeline-dg.pdf#what-is-datapipeline](https://docs.aws.amazon.com/datapipeline/latest/DeveloperGuide/datapipeline-dg.pdf#what-is-datapipeline)


**References:**

[https://docs.aws.amazon.com/datapipeline/latest/DeveloperGuide](https://docs.aws.amazon.com/datapipeline/latest/DeveloperGuide)

[https://aws.amazon.com/datapipeline/pricing/](https://aws.amazon.com/datapipeline/pricing/)

[https://aws.amazon.com/datapipeline/faqs/](https://aws.amazon.com/datapipeline/faqs/)

**Videos**

[https://www.youtube.com/watch?v=lRWkGVBb13o](https://www.youtube.com/watch?v=lRWkGVBb13o)

[https://www.youtube.com/watch?v=5eq6fiw1dPA](https://www.youtube.com/watch?v=5eq6fiw1dPA)


------------------------------------------------------------------------------------------------------------------------
## <a href="#section-13"></a> **13 - Amazon CloudSearch**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_Amazon-CloudSearch_48.png)

A fully-managed service in the AWS Cloud that makes it easy to set up, manage, and scale a search solution for your website or application.

**Features**

- You can use CloudSearch to index and search both structured data and plain text.
- Full text search with language-specific text processing
- Boolean search
- Prefix searches
- Range searches
- Term boosting
- Faceting
- Highlighting
- Autocomplete Suggestions
- You can get search results in JSON or XML, sort and filter results based on field values, and sort results alphabetically, numerically, or according to custom expressions.
- CloudSearch can scale to accommodate the amount of data uploaded to the domain and the volume and complexity of search requests.
- You can integrate CloudSearch with API Gateway.

**Cheat Sheets**

[https://digitalcloud.training/amazon-opensearch/](https://digitalcloud.training/amazon-opensearch/)

[https://tutorialsdojo.com/amazon-cloudsearch/](https://tutorialsdojo.com/amazon-cloudsearch/)

**References:**

[https://docs.aws.amazon.com/cloudsearch/latest/developerguide/](https://docs.aws.amazon.com/cloudsearch/latest/developerguide/)

[https://aws.amazon.com/cloudsearch/pricing/](https://aws.amazon.com/cloudsearch/pricing/)

[https://aws.amazon.com/cloudsearch/faqs/](https://aws.amazon.com/cloudsearch/faqs/)

**Videos**

[https://www.youtube.com/watch?v=eOVRt46RwT8](https://www.youtube.com/watch?v=eOVRt46RwT8)

[https://www.youtube.com/watch?v=mdj8RQhqOEg](https://www.youtube.com/watch?v=mdj8RQhqOEg)

------------------------------------------------------------------------------------------------------------------------
## <a href="#section-14"></a> **14 - Amazon Lake Formation**

![EMR](/images/Architecture09172021/Arch_Analytics/Arch_48/Arch_AWS-Lake-Formation_48.png)

AWS Lake Formation is a service that makes it easy to set up a secure data lake in days. A data lake is a centralized, curated, and secured repository that stores all your data, both in its original form and prepared for analysis. A data lake lets you break down data silos and combine different types of analytics to gain insights and guide better business decisions.

Setting up and managing data lakes today involves a lot of manual, complicated, and time-consuming tasks. This work includes loading data from diverse sources, monitoring those data flows, setting up partitions, turning on encryption and managing keys, defining transformation jobs and monitoring their operation, reorganizing data into a columnar format, deduplicating redundant data, and matching linked records. 

Once data has been loaded into the data lake, you need to grant fine-grained access to datasets, and audit access over time across a wide range of analytics and machine learning (ML) tools and services.

Creating a data lake with Lake Formation is as simple as defining data sources and what access and security policies you want to apply. Lake Formation then helps you collect and catalog data from databases and object storage, move the data into your new Amazon Simple Storage Service (S3) data lake, clean and classify your data using ML algorithms, and secure access to your sensitive data using granular controls at the column, row, and cell-levels. 

Your users can access a centralized data catalog that describes available datasets and their appropriate usage. They then use these datasets with their choice of analytics and ML services, such as Amazon Redshift, Amazon Athena, Amazon EMR for Apache Spark, and Amazon QuickSight. Lake Formation builds on the capabilities available in AWS Glue.


**References:**

[https://aws.amazon.com/lake-formation/?nc1=h_ls&whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc](https://aws.amazon.com/lake-formation/?nc1=h_ls&whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc)


**Videos**

[https://www.youtube.com/watch?v=Aj5T5fcZZr0](https://www.youtube.com/watch?v=Aj5T5fcZZr0)







