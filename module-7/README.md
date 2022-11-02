<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Módulo 7: Armazenamento

## Conteúdo
1. <a href="#section-1"> Amazon Simple Storage Service (S3) </a>
2. <a href="#section-2"> AWS Snowball </a>
3. <a href="#section-3"> Amazon Elastic Block Store (EBS) </a>
4. <a href="#section-4"> Instance Store Volumes </a>
5. <a href="#section-5"> Amazon Elastic File System (EFS) </a>
6. <a href="#section-6"> AWS Storage Gateway </a>

----------------------------------------------------------------------------------------------------

## <a id="section-1" ></a> **1 - Amazon Simple Storage Service (S3)**

Amazon S3 is an object store built to store and retrieve any amount of data from anywhere – websites and mobile apps, enterprise applications, and data from sensors or IoT devices.

You can store any type of file on S3.

The S3 is designed to deliver 99.999999999% durability and stores data from millions of applications used by market leaders across all industries.

S3 offers comprehensive security and compliance features that meet even the most stringent regulatory requirements.

S3 gives customers flexibility in how they manage data for cost optimization, access control and compliance.

Typical use cases include:
- **Backup and Storage** – Provides data backup and storage services to others.
- **App Hosting** – Provides services that deploy, install and manage web applications.
- **Media Hosting** – Create a redundant, scalable, highly available infrastructure that hosts video, photo or music uploads and downloads.
- **Software Delivery** – Host your software applications that customers can download.
- **Static Website** – You can configure a static website to run from an S3 bucket.

S3 provides on-premises query functionality, allowing you to run powerful analytics directly on your data at rest in S3. And Amazon S3 is the most supported cloud storage service available, with integration from the largest community of third-party solutions, systems integrator partners, and other AWS services.

Files can be from 0 bytes to 5 TB.

There is unlimited storage available.

Files are stored in buckets.

Buckets are root-level folders.

Any subfolder within a bucket is known as a “folder”.

S3 is a universal namespace, so bucket names must be globally unique.

**There are seven S3 storage classes.**
- **S3 Standard** (durable, immediately available, frequently accessed).
- **S3 Intelligent-Tiering** (automatically moves data to the most economical level).
- **S3 Standard-IA** (durable, immediately available, infrequently accessed).
- **S3 One Zone-IA** (lower cost for infrequently accessed data with less resiliency).
- **S3 Glacier Instant Retrieval** (data that is rarely accessed and requires millisecond retrieval).
- **S3 Glacier Flexible Retrieval** (archived data, retrieval times in minutes or hours).
- **S3 Glacier Deep Archive** (lowest cost storage class for long-term retention).

The table below provides the details for each Amazon S3 storage class:

| |S3 Standard |S3 Intelligent Tiering |S3 Standard-IA |S3 One Zone-IA |S3 Glacier Instant Retrieval |S3 Glacier Flexible Retrieval |S3 Glacier Deep Archive|
|---|---------------|-----------------------|----- ----------|---------------|----------------------- --------|-------------------------------|--------- ------|
|Designed for durability |11 9s |11 9s |11 9s |11 9s |11 9s |11 9s |11 9s|
|Designed for availability |99.99% |99.9& |99.9% |99.5% |99.9% |99.99% |99.99%|
|Availability SLA |99.9% |99% |99% |99% |99% |99.99% |99.9%|
|Availability Zones |≥3 |≥3 |≥3 |1 |≥3 |≥3 |≥3|
|Minimum capacity charge per object |N/A |N/A |128KB |128KB |128KB |40KB |40KB|
|Minimum storage duration charge |N/A |N/A |30 days |30 days |90 days |90 days |180 days|
|Retrieval fee |N/A |N/A |Per GB retrieved |Per GB retrieved |Per GB retrieved |Per GB retrieved |Per GB retrieved|
|First byte latency |milliseconds |milliseconds |milliseconds |milliseconds |milliseconds |minutes or hours| hours|


When you successfully upload a file to S3, you receive an HTTP 200 code.

S3 is a highly durable, persistent data store.

Persistent data stores are non-volatile storage systems that retain data when turned off.

This is in contrast to temporary data stores and ephemeral data stores that lose data when turned off.

The following table provides a description of persistent, transient, and ephemeral data stores and which AWS service to use:


|Storage Type |Description |Examples|
|---------------|---------------|--------|
|Persistent Data Store |Data is durable and sticks around after reboots, restarts, or power cycles |S3, Glacier, EBS, EFS|
|Transient Data Store |Data is just temporarily stored and passed along to another process or persistent store |SQS, SNS|
|Ephemeral Data Store |Data is lost when the system is stopped |EC2 Instance Store, Memcached|


**Bucket names must follow a set of rules:**
- Names must be unique across AWS.
- Names must be 3 to 63 characters long.
- Names can only contain lowercase letters, numbers and hyphens.
- Names cannot be formatted as an IP address.

**Objects consist of:**
- Key (object name).
- Value (data formed by a sequence of bytes).
- Version ID (used for version control).
- Metadata (data about stored data).

**Sub-resources:**
- Access control lists.
- Torrent.

Object Sharing – The ability to make any object publicly available via a URL.

Lifecycle Management – ​​Define rules to transfer objects between storage classes at defined time intervals.

Version Control – Automatically maintains multiple versions of an object (when enabled).

Encryption can be enabled for the bucket.

Data is protected using ACLs and bucket policies.

**Charges:**
- Store(Storage).
- Requests.
- Storage management pricing.(Storage management pricing)
- Data transfer pricing. (Data transfer pricing.)
- Transfer acceleration.(Transfer acceleration)

When creating a bucket, you need to select the region where it will be created.

It is a best practice to create buckets in regions that are physically closer to your users to reduce latency.

Additional features offered by Amazon S3 include:


|Additional S3 Capability |How it Works|
|---------------------------|------------|
|Transfer Acceleration |Speed ​​up data uploads using CloudFront in reverse|
|Requester Pays |The requester rather than the bucket owner pays for requests and data transfer|
|Tags |Assign tags to objects to use in costing, billing, security etc.|
|Events |Trigger notifications to SNS, SQS, or Lambda when certain events happen in your bucket|
|Static Web Hosting |Simple and massively scalable static website hosting|
|BitTorrent |Use the BitTorrent protocol to retrieve any publicly available object by automatically generating a .torrent file|

----------------------------------------------------------------------------------------------------
## <a id="section-2"></a> **2 - AWS Snowball**

AWS Snowball (Snowball), you can transfer hundreds of terabytes or petabytes of data between your on-premises data centers and Amazon Simple Storage Service (Amazon S3).

Uses a secure storage device for physical transport.

The AWS Snowball Client is software installed on a local computer and used to identify, compress, encrypt, and transfer data.

Uses 256-bit encryption (managed with AWS KMS) and tamper-proof enclosures with TPM.

The table below describes high-level AWS Snow offerings:


|Service |What it Is|
|-----------|----------|
|AWS Snowball |Bulk data transfer, edge storage, and edge compute|
|AWS Snowmobile |A literal shipping container full of storage (up to 100PB) and a truck to transport it|
|AWS Snowcone |The smallest device in the range that is best suited for outside the data center|


Snowball can import to S3 or export from S3.

Import/Export is when you upload your own disks to AWS – this is being deprecated in favor of Snowball.

Snowball must be ordered and returned in the same region.

To speed up data transfer, it is recommended that you run simultaneous instances of the AWS Snowball Client on multiple endpoints and transfer small files in batches.

----------------------------------------------------------------------------------------------------
## <a id="section-3" ></a> **3 - Amazon Elastic Block Store (EBS)**


**EBS Pricing**
[EBS Pricing](https://aws.amazon.com/ebs/pricing/)

With Amazon Elastic Block Store (EBS), you pay only for what you provision. Volume storage for all EBS volume types is charged by the amount of GB you provision per month until you release the storage. Costs increase for EBS volumes that support additional input/output operations per second (IOPS) and throughput beyond baseline performance.

- **Free Tier**
    - AWS Free Tier includes 30 GB of storage, 2 million I/Os, and 1 GB of snapshot storage with Amazon Elastic Block Store (EBS).

Amazon Elastic Block Store (Amazon EBS) provides persistent block storage volumes for use with Amazon EC2 instances in the AWS Cloud.

Each Amazon EBS volume is automatically replicated across its Availability Zone to protect against component failures, providing high availability and durability.

Amazon EBS volumes provide the consistent, low-latency performance you need to run your workloads. With Amazon EBS, you can scale your usage up or down in minutes – all while paying a low price just for what you provision.

The following EBS volumes appear most frequently in AWS exams:

|Volume Type |EBS Provisioned IOPS SSD (io1/io2) |EBS General Purpose SSD (gp2/gp3) |Throughput Optimized HDD (st1) |Cold HDD (sc1)|
|---------------|-------------------------------- -----|------------------------------------|------- ------------------------|--------------|
|Short Description |Highest performance SSD volume designed for latency-sensitive transactional workloads| General Purpose SSD volume that balances price performance for a wide variety of transactional workloads| Low-cost HDD volume, designed for frequently accessed. Throughput intensive workloads| Lowest cost HDD volume designed for less frequently accessed workloads|
|Use Cases |I/O-intensive NoSQL and relational databases| Boot volumes, low-latency interactive apps, dev & test| Big data, data warehouses, log processing| Colder data requiring fewer scans per day|
|Volume Size |4 GiB – 16 TiB| 1 GiB – 16 TiB| 125 GB – 16 TiB |125 GB – 16 TiB|
|Max IOPS** / Volume |64,000 |16,000 |500 |250|
|Max Throughput***Volume |1,000 MiB/s |250 MiB/s (gp2) |1000 MiB/s (gp3) |500 MiB/s |250 MiB/s|
|Can be boot volume? |Yes |Yes |No |No|
|EBS Multi-attach |Supported |Not Supported |Not Supported |Not Supported|



EBS volume data persists regardless of the lifetime of the instance.

EBS volumes do not need to be attached to an instance.

You can attach multiple EBS volumes to an instance.

You cannot attach an EBS volume to multiple instances (use Elastic File Store instead).

EBS volumes must be in the same AZ as the instances to which they are attached.

Termination protection is off by default and must be manually enabled (keeps volume/data when instance is terminated).

EBS root volumes are deleted on shutdown by default.

Extra non-boot volumes are not deleted on shutdown by default.

The behavior can be changed by changing the “DeleteOnTermination” attribute.

EBS Snapshots:
- Snapshots capture a point-in-time state of an instance.
- Snapshots are stored on S3.
- Does not provide granular backup (does not replace backup software).
- If you take periodic snapshots of a volume, the Snapshots will be incremental, which means that only the blocks on the device that changed after the last snapshot are saved in the new snapshot.
- Although snapshots are saved incrementally, the snapshot deletion process is designed so that you only need to retain the most recent snapshot to restore the volume.
- Snapshots can only be accessed through EC2 APIs.
- EBS volumes are AZ specific, but Snapshots are region specific.

----------------------------------------------------------------------------------------------------
## <a id="section-4" ></a> **4 - Instance Store Volumes**

**Instance Store Volumes** are high-performance local disks that are physically connected to the host computer on which an EC2 instance runs.

**Instance Store Volumes** are ephemeral, which means data is lost when powered off (non-persistent).

**Instance Store Volumes** are ideal for temporary storage of information that changes frequently, such as buffers, caches or temporary data.

**Instance Store Volumes** root devices are created from AMI templates stored in S3.

**Instance Store Volumes** cannot be detached/reattached.

-------------------------------------------------- --------------------------------------------------
## <a id="section-5" ></a> **5 - Amazon Elastic File System (EFS)**

EFS is a fully managed service that makes it easy to configure and scale your file storage on the Amazon Cloud.

Good for big data and analytics, media processing workflows, content management, web service, home directories, etc.

EFS uses the NFS protocol.

Pay for what you use (no pre-provisioning required).

It can scale up to petabytes.

EFS is elastic and grows and shrinks as you add and remove data.

Can simultaneously connect 1 to 1000 EC2 instances from multiple AZs.

A file system can be accessed simultaneously from all AZs in the region where it is located.

By default, you can create up to 10 file systems per account.

Local access can be enabled via Direct Connect or AWS VPN.

You can choose General Purpose or Max I/O (both SSD).

The connecting instance's VPC must have DNS hostnames enabled.

EFS provides a file system interface, file system access semantics (such as strong consistency and file locking).

Data is stored in multiple AZs within a region.

Read after write consistency.

Need to create mount targets and choose AZs to include (recommended to include all AZs).

Instances can be behind an ELB.

**There are two performance modes:**
- “General Purpose” performance mode is suitable for most file systems.
- “Max I/O” performance mode is optimized for applications where tens, hundreds or thousands of EC2 instances are accessing the file system.

Amazon EFS is designed for bursting to allow for high levels of throughput over periods of time.

----------------------------------------------------------------------------------------------------

## <a id="section-6" ></a> **6 - AWS Storage Gateway**

The [**AWS Storage Gateway**](https://aws.amazon.com/storagegateway/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc) is a hybrid cloud storage service that gives you virtually unlimited local access to cloud storage.

Customers use Storage Gateway to simplify storage management and reduce costs for key hybrid cloud storage use cases.

This includes moving backups to the cloud, using local file shares with cloud storage support, and providing low-latency access to data in AWS for on-premises applications.

To support these use cases, Storage Gateway offers three different types of gateways:
- **File Gateway** – provides file system interfaces to local servers.
- **Volume Gateway** – provides block-based access to local servers.
- **Tape Gateway** – provides a virtual tape library compatible with common backup software (block and file interfaces).


how it works

AWS Storage Gateway is a set of hybrid cloud storage services that provide on-premises access to virtually unlimited cloud storage.

<img src="../images/extra/product-page-diagram_AWS-Storage-Gateway_HIW@2x.6.png" alt="product-page-diagram_AWS-Storage-Gateway_HIW@2x.6" width=80% />



https://docs.aws.amazon.com/vpc/latest/privatelink/gateway-endpoints.html#gateway-endpoint-pricing



