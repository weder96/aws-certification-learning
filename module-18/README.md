<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# [Módulo 18: Containers](https://aws.amazon.com/what-is/compute/)

## Content
1. <a href="#section-01"> Amazon Elastic Container Registry (Amazon ECR) </a>
2. <a href="#section-02"> Amazon Elastic Container Service (Amazon ECS) </a>
3. <a href="#section-03"> Amazon Elastic Kubernetes Service (Amazon EKS) </a>
4. <a href="#section-04"> AWS Fargate </a>


***************************************************************************************************
## <a id="section-01"></a> **1 - Amazon Elastic Container Registry (Amazon ECR)**

![Elastic-Container-Registry](../images/Architecture-Service-Icons_06072024/Arch_Containers/48/Arch_Amazon-Elastic-Container-Registry_48.svg "Elastic-Container-Registry")

**Definitions**

Amazon Elastic Container Registry (ECR) is a fully managed container image registry that makes it easy to store, manage, and deploy Docker container images on AWS. ECR integrates seamlessly with other AWS services like Amazon ECS and Amazon EKS, simplifying the management of your containerized applications.
- A managed AWS Docker registry service.
- Amazon ECR is a regional service.

### **Features**
- ECR supports Docker Registry HTTP API V2 allowing you to use Docker CLI commands or your preferred Docker tools in maintaining your existing development workflow.
- ECR stores both the containers you create and any container software you buy through AWS Marketplace.
- ECR stores your container images in Amazon S3.
- ECR supports the ability to define and organize repositories in your registry using namespaces.
- You can transfer your container images to and from Amazon ECR via HTTPS.

### **Security**
- By default, IAM users don’t have permission to create or modify Amazon ECR resources, or perform tasks using the Amazon ECR API.
- Use IAM policies to grant or deny permission to use ECR resources and operations.
- ECR partially supports resource-level permissions.
- ECR supports the use of customer master keys (CMK) managed by AWS Key Management Service (KMS) to encrypt container images stored in your - ECR repositories.

### **Pricing**
- You pay only for the amount of data you store in your repositories and data transferred to the Internet.


### Key Features

### Store and Manage Docker Images on AWS

  Amazon ECR provides a secure and scalable solution to store your Docker container images. It enables developers to easily push, pull, and manage images with just a few clicks, making it simpler to work with containerized applications in the AWS ecosystem.

### Private and Public Repositories

  ECR allows you to create both private and public repositories. Private repositories are fully secured and accessible only to authorized AWS users, while public repositories, such as the [Amazon ECR Public Gallery](https://gallery.ecr.aws), allow you to share container images with the broader community. This flexibility enables you to manage both internal and external images with ease.

### Fully Integrated with ECS and EKS

  ECR is deeply integrated with Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS), allowing you to easily deploy container images to these services without needing to manually handle container image storage or access. ECR seamlessly works with ECS Task Definitions and EKS Pods to streamline container orchestration.

### Backed by Amazon S3

  ECR stores container images in Amazon S3, providing high durability and availability. The underlying infrastructure ensures that your images are highly available and fault-tolerant, offering a secure and scalable storage solution for containerized applications.

### Access Control through IAM

  Access to Amazon ECR repositories is managed through AWS Identity and Access Management (IAM). You can define fine-grained permissions to control who can push, pull, or manage images within your repositories. This ensures that sensitive container images are accessible only to the right users and services.

### Vulnerability Scanning

  ECR supports image vulnerability scanning to help identify security issues within your container images. By scanning for known vulnerabilities, it enables you to improve the security posture of your containerized applications, ensuring that any potential risks are detected early in the development or deployment pipeline.

### Image Versioning and Tags

  ECR provides support for image versioning and tagging. You can tag different versions of the same image and easily manage and reference these versions when deploying to ECS or EKS. This enables better version control and rollback capabilities for containerized applications.

### Image Lifecycle Policies

  ECR offers image lifecycle policies that allow you to automatically manage the lifecycle of container images within a repository. You can define rules to automatically delete or archive old, unused images based on tags, age, or other criteria. This helps optimize storage costs and maintain a clean, organized image repository.


**Cheat Sheets**

https://tutorialsdojo.com/amazon-elastic-container-registry-amazon-ecr/

**References:**

https://docs.aws.amazon.com/AmazonECR/latest/userguide/

https://aws.amazon.com/ecr/features/

https://aws.amazon.com/ecr/pricing/

https://aws.amazon.com/ecr/faqs/

**Videos**

https://www.youtube.com/results?search_query=Elastic+Container+Registry

**Hands On**

https://www.youtube.com/results?search_query=Elastic+Container+Registry+Hans+on

***************************************************************************************************
## <a id="section-02"></a> **2 - Amazon Elastic Container Service (Amazon ECS)**

![Elastic-Container-Service](../images/Architecture-Service-Icons_06072024/Arch_Containers/64/Arch_Amazon-Elastic-Container-Service_64.svg "Elastic-Container-Service")

**Definition**

Amazon Elastic Container Service (ECS) is a fully managed container orchestration service provided by AWS. It allows users to run and scale Docker containers across a managed cluster of EC2 instances or in a serverless model using AWS Fargate. ECS integrates seamlessly with other AWS services, providing a powerful solution for deploying and managing containerized applications.

### ECS Clusters

An ECS Cluster is a logical grouping of resources, such as EC2 instances or Fargate tasks, that can be used to run ECS tasks and services. Each cluster can contain multiple EC2 instances or Fargate tasks, and all resources within a cluster can communicate with each other securely within the same VPC.

- **EC2 Cluster:** If using the EC2 launch type, ECS tasks run on EC2 instances that you provision and manage.
- **Fargate Cluster:** If using the Fargate launch type, tasks are managed entirely by AWS without the need for EC2 instances.

### Task Definitions

A Task Definition is a blueprint that describes the containers that will be used in an ECS task. It defines various settings such as:

- Container images (e.g., Docker images)
- CPU and memory requirements
- Port mappings for container networking
- Environment variables and secrets
- Log configuration (e.g., sending logs to CloudWatch)
- Volumes to mount (e.g., EFS volumes)

A task definition is required for launching containers, and you can create multiple revisions of a task definition to update container configurations over time.

### ECS Tasks

An ECS Task is the basic unit of work in ECS. A task represents one or more Docker containers running on an ECS cluster. Tasks are instantiated from task definitions and run on either EC2 instances or Fargate.

- **Task Lifecycle:** ECS tasks can be started, stopped, and managed through the ECS service. Tasks can run on EC2 instances or in a serverless environment using Fargate.
- **Task Placement:** ECS places tasks on instances based on defined resource requirements (CPU, memory), availability zones, and task placement strategies (e.g., binpacking, spread, etc.).

### Amazon ECS – EC2 Launch Type

- **Launch Docker Containers on AWS:** The EC2 launch type is ideal for users who need to run containerized applications on a cluster of Amazon EC2 instances. You are responsible for provisioning and maintaining the EC2 instances, providing full control over the underlying infrastructure.
- **ECS Agent on EC2 Instances:** Each EC2 instance in the ECS cluster must run the ECS Agent. This agent registers the instance with the ECS service, allowing ECS to schedule and manage tasks on that instance.
- **Auto Scaling ECS Clusters:** ECS integrates with EC2 Auto Scaling groups to allow the ECS cluster to scale dynamically based on resource utilization such as CPU or memory. This ensures that the cluster can accommodate varying workloads while optimizing resource allocation.
- **Manual Infrastructure Management:** With the EC2 launch type, you have full control over the infrastructure and must manage the scaling, maintenance, and security patches for EC2 instances. This offers flexibility but requires more operational overhead.

### Amazon ECS – Fargate Launch Type

- **Serverless Container Management:** The Fargate launch type abstracts away the need to manage EC2 instances entirely. With Fargate, you only need to define task definitions, which include the CPU and memory specifications, and AWS will handle the rest. This allows for fully serverless operation, removing the complexity of infrastructure management.
- **Task-Level Scaling:** Fargate allows users to scale containerized applications by adjusting the number of tasks running in their ECS service. It eliminates the need for manual instance provisioning, making it ideal for dynamic workloads that require elasticity without manual intervention.
- **Pay-as-You-Go:** Fargate charges based on the resources (CPU and memory) your tasks use during execution. This model allows you to pay only for the compute resources required for your containers, ensuring cost efficiency for variable workloads.

### IAM Roles for ECS

- **EC2 Instance Profile (EC2 Launch Type Only):** Each EC2 instance in the ECS cluster requires an associated EC2 instance profile. This profile allows the ECS agent to interact with AWS services on behalf of the instance, such as pulling Docker images from Amazon ECR, pushing logs to CloudWatch, and retrieving sensitive information from services like Secrets Manager or SSM Parameter Store.
- **ECS Task Role:** Each ECS task can have an IAM role assigned specifically to it, known as the ECS task role. This role allows the task to access AWS resources such as S3, DynamoDB, and other services necessary for its operation. Each ECS service can define different roles for different tasks, providing fine-grained access control.

### Amazon ECS – Load Balancer Integrations

- **Application Load Balancer (ALB):** The ALB is the most commonly used load balancer with ECS. It supports advanced routing features like host-based routing, path-based routing, and WebSocket support, making it a versatile choice for most ECS workloads. ALBs automatically distribute incoming traffic across the tasks in your ECS service, improving fault tolerance and scalability.
- **Network Load Balancer (NLB):** NLB is used for high-throughput, low-latency applications that require performance at the network layer. It is ideal for use cases requiring high-performance workloads, including those that handle millions of requests per second. NLB can be paired with AWS PrivateLink to securely access ECS services from within a VPC.
- **Classic Load Balancer (CLB):** Although the Classic Load Balancer is still supported, it is not recommended for modern use cases. CLB lacks many of the advanced features provided by ALB and NLB, such as the ability to handle containerized applications running on Fargate.

### Amazon ECS – Data Volumes (Amazon EFS Integration)

- **Mounting EFS File Systems:** Amazon ECS allows you to mount Amazon EFS file systems to ECS tasks, providing persistent storage that is shared across multiple availability zones (AZs). This integration works for both EC2 and Fargate launch types, enabling scalable, distributed file storage for containerized applications.
- **Fargate + EFS = Serverless Storage:** Combining Fargate with EFS offers a fully serverless solution for containerized applications that require persistent storage. This allows ECS tasks to interact with a shared file system, while the serverless nature of Fargate ensures scalability and reduced operational overhead.
- **Use Cases for EFS in ECS:** EFS is particularly useful for applications that require multi-AZ shared storage, such as content management systems, media processing workflows, and data analytics pipelines. It supports applications that require file locking and direct file system interaction.
- **Important Note:** While Amazon EFS provides persistent storage for containerized workloads, Amazon S3 cannot be mounted as a file system on ECS tasks. S3 is an object storage service, and while it’s excellent for storing large amounts of unstructured data, it does not provide the file system capabilities required by some applications.

### Auto Scaling

Implementing an ECS cluster with Auto Scaling groups and creating scaling policies based on resource utilization (like CPU and memory reservation metrics) will ensure that the application can dynamically scale in response to changing workloads, maintaining high throughput and performance.

### Amazon CloudWatch Container Insights

- **Monitoring and Observability:** CloudWatch Container Insights is a feature of Amazon CloudWatch that provides real-time monitoring and troubleshooting capabilities for containerized applications running on ECS, EKS, and Kubernetes clusters. It collects metrics, logs, and traces from ECS tasks and clusters, providing end-to-end visibility into containerized environments.
- **Automatic Dashboards:** Container Insights automatically generates pre-configured dashboards that display important metrics such as CPU utilization, memory usage, and task status. These dashboards can be customized to monitor other key performance indicators (KPIs) relevant to your workloads.
- **Log Collection and Analysis:** ECS integrates with CloudWatch Logs, allowing you to capture logs from containers, ECS tasks, and ECS services. This integration simplifies log management, enabling you to view logs in a centralized location and troubleshoot issues quickly.
- **Alarming and Notifications:** CloudWatch Container Insights supports creating custom alarms based on ECS metrics. You can set up alerts to notify you when a container is running out of memory or when a task fails, ensuring you can respond quickly to potential issues before they impact production workloads.

### Troubleshooting ECS Tasks and Pods

- **Diagnosing Task Failures:** When tasks or containers fail to run as expected, CloudWatch Logs and CloudWatch Metrics can provide valuable insights into the issue. You can use the logs to debug the container’s behavior, and CloudWatch Metrics can indicate if the failure is due to resource exhaustion (e.g., CPU or memory limits).
- **Reviewing Logs:** Reviewing logs from ECS tasks and the ECS Agent is crucial in understanding why a task is failing. These logs can provide error messages, stack traces, and details about resource provisioning, which can help resolve configuration issues or application bugs.
- **Node and Infrastructure Issues:** In cases where tasks are failing on a specific EC2 instance or node, reviewing the node’s logs and metrics can uncover issues related to infrastructure. Resource limitations such as insufficient memory, CPU, or disk space on the EC2 instance can also cause task failures. Ensuring that your EC2 instances are correctly sized for the workload is essential for maintaining stable task execution.

### Integrating ECS with Other AWS Services

- **AWS Step Functions Integration:** ECS can be integrated with AWS Step Functions to orchestrate multi-step workflows and complex application architectures. Step Functions allows you to define a state machine that can trigger ECS tasks at different stages of the workflow, helping you build end-to-end automation for batch processing, data pipelines, and microservices applications.
- **Amazon S3 for Input and Output Data:** ECS can interact with Amazon S3 for data storage. For example, ECS tasks can read input data from S3, process it, and then write the results back to S3. This is a common pattern for data processing and analytics applications.
- **Amazon RDS and DynamoDB for Database Access:** ECS integrates with relational databases like Amazon RDS and NoSQL databases like DynamoDB, enabling containerized applications to read from and write to databases. This is essential for stateful applications that require persistent data storage.


### Extras 

- A container management service to run, stop, and manage Docker containers on a cluster.
- ECS can be used to create a consistent deployment and build experience, manage, and scale batch and Extract-Transform-Load (ETL) workloads, and build sophisticated application architectures on a microservices model.
- Amazon ECS is a **regional service**.
- The Amazon Elastic Container Service (ECS) is a highly scalable, high performance container management service that supports **Docker containers**.
- Amazon ECS allows you to easily run applications on a managed cluster of Amazon EC2 instances.
- Amazon ECS eliminates the need for you to install, operate, and scale your own cluster management infrastructure.
- Using API calls you can launch and stop container-enabled applications, query the complete state of clusters, and access features like security  groups, Elastic Load Balancing, EBS volumes and IAM roles.
- Amazon ECS can be used to schedule the placement of containers across clusters based on resource needs and availability requirements.
- There is no additional charge for Amazon ECS. You pay for:
- Resources created with the EC2 Launch Type (e.g. EC2 instances and EBS volumes).
- The number and configuration of tasks you run for the Fargate Launch Type.


**Cheat Sheets**

https://tutorialsdojo.com/amazon-elastic-container-service-amazon-ecs/

https://digitalcloud.training/amazon-ecs-and-eks/

**References:**

https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html

https://aws.amazon.com/ecs/features/

https://aws.amazon.com/ecs/pricing/

https://aws.amazon.com/ecs/faqs/

**Videos**

https://www.youtube.com/results?search_query=Amazon+ECS

**Hands On**

https://www.youtube.com/results?search_query=Amazon+ECS+hands+on


***************************************************************************************************

***************************************************************************************************
## <a id="section-03"></a> **3 - Amazon Elastic Kubernetes Service (Amazon EKS)**

![Amazon-EKS-Cloud](../images/Architecture-Service-Icons_06072024/Arch_Containers/64/Arch_Amazon-Elastic-Kubernetes-Service_64.svg "Amazon-EKS-Cloud")

**Definition**

### What is Amazon EKS?

Amazon Elastic Kubernetes Service (EKS) is a fully managed service that simplifies the deployment, management, and scaling of Kubernetes clusters on AWS. Kubernetes is an open-source orchestration system for automating the deployment, scaling, and management of containerized applications.

- A managed service that allows you to run Kubernetes on AWS without installing, operating, or maintaining your own Kubernetes control plane or nodes.
- Integration with various AWS services to provide scalability and security for your applications:
- Amazon ECR for container images
- Elastic Load Balancing for load distribution
- IAM for authentication
- Amazon VPC for isolation

### **Amazon EKS Anywhere**

![Amazon-EKS-Cloud](../images/Architecture-Service-Icons_06072024/Arch_Containers/64/Arch_Amazon-EKS-Anywhere_64.svg "Amazon-EKS-Cloud")

Using Amazon EKS Anywhere is another way to deploy your containers on-premises. 

It works like Amazon ECS Anywhere, which allows you to run your containerized cluster entirely on your own. 

This means that the hardware, app deployment location, control plane, and data plane are all controlled on your own physical network. 

This gives you extensive control over all the components of your containerized application suite while maintaining official support from AWS.

### **Amazon EKS Distro**
![Amazon EKS Distro](../images/Architecture-Service-Icons_06072024/Arch_Containers/64/Arch_Amazon-EKS-Distro_64.svg "Amazon EKS Distro")

The other deployment option that you can choose is Amazon EKS Distro. 

The word “distro” simply refers to the distribution of the same open-source Kubernetes software deployed by Amazon EKS in the AWS cloud. 

Amazon EKS Distro follows the same Kubernetes version release cycle as Amazon EKS and is provided to you as an open-source project that you can deploy on your own computer or on-site environment. 

It’s similar to the Amazon EKS Anywhere option, except that it does not include support services offered by AWS.
 

### **Amazon EKS Pricing**

- For each Amazon EKS cluster you create, you are charged an hourly rate.
- You are charged for the AWS resources that you create to run Kubernetes worker nodes in Amazon EC2 with Amazon EKS managed node groups.
- In Amazon EKS on AWS Fargate, you are charged for the vCPU and memory resources.
- Amazon EKS on AWS Outposts charges an hourly rate for EKS clusters deployed in the cloud, but there is no additional charge for Kubernetes worker nodes running on Outposts EC2.


### Key Features

- **Managed Kubernetes Clusters:** EKS allows you to run Kubernetes workloads with minimal operational overhead. It integrates seamlessly with Kubernetes ecosystem tools.
- **Flexibility:** Supports both **EC2 instances** (worker nodes) and **AWS Fargate** for serverless containers.
- **Multi-Cloud Compatibility:** Kubernetes is cloud-agnostic, making EKS suitable for organizations transitioning from on-premises Kubernetes or other cloud providers.
- **Regional Deployment:** For high availability and disaster recovery, deploy one EKS cluster per region.

### EKS Components

### Node Management

1. **Managed Node Groups:**
   - Nodes (EC2 instances) are automatically created and managed by EKS.
   - Nodes are part of an Auto Scaling Group (ASG) for dynamic scalability.
   - Supports **On-Demand** and **Spot Instances** for cost optimization.

2. **Self-Managed Nodes:**
   - Nodes are provisioned manually by the user and registered to the EKS cluster.
   - Supports **Amazon EKS Optimized AMI** for quick setup.
   - Offers flexibility but requires additional management.

3. **AWS Fargate:**
   - A **serverless** option for running Kubernetes workloads.
   - Removes the need to manage nodes.
   - Ideal for applications requiring high scalability with minimal operational complexity.

### Storage Integration

Amazon EKS supports multiple AWS storage solutions through the **Container Storage Interface (CSI):**

- **Amazon EBS:** Block storage for persistent volumes.
- **Amazon EFS:** Shared file storage, compatible with Fargate.
- **Amazon FSx for Lustre:** High-performance file systems.
- **Amazon FSx for NetApp ONTAP:** Enterprise-grade storage capabilities.

For optimized storage use:

- Specify the **StorageClass manifest** in the EKS cluster configuration.
- Leverage ephemeral volumes tied to the pod lifecycle for **low-latency workloads**, such as using node RAM for temporary storage.

### Scaling and Performance

Amazon EKS provides robust scaling mechanisms to ensure optimal resource utilization and performance.

### Horizontal Pod Autoscaling (HPA)

Horizontal Pod Autoscaling automatically adjusts the number of pods in a deployment based on observed CPU or memory usage. For example, if an application experiences high traffic and CPU usage increases beyond a defined threshold, HPA will add more pods to handle the load. Conversely, during low traffic periods, it reduces the number of pods to conserve resources. This ensures that applications remain responsive while minimizing resource costs.

>Note: A pod is the smallest deployable unit in Kubernetes. It represents a single instance of a running process in your cluster.

### Dynamic Workload Scaling with Carpenter

Carpenter is a scaling tool for EKS that dynamically adjusts compute resources based on workload demands. It intelligently provisions nodes with the right size and type, such as GPU-enabled instances for AI tasks or memory-optimized instances for data-heavy workloads. As demands change, Carpenter ensures that the cluster has exactly what is needed, reducing waste while maintaining application performance.

### Cluster Auto Scaling with ASG

EKS integrates with Auto Scaling Groups (ASGs) to manage the scaling of EC2 nodes. The cluster automatically increases or decreases the number of EC2 instances based on predefined metrics, such as CPU or memory utilization. For example, if multiple pods cannot find space on existing nodes due to resource constraints, ASG adds new instances to the cluster. Similarly, when nodes are underutilized, ASG reduces the cluster size to cut costs. This dynamic scaling maintains high availability while optimizing expenses.

### Security and Access Control

### IAM Roles for Service Accounts (IRSA)

- Assign **IAM roles** directly to Kubernetes pods for secure and granular access to AWS resources like DynamoDB.
- Recommended for secure and least-privilege access.

### Taints and Tolerations

EKS leverages taints and tolerations to control the placement of pods within the cluster, allowing for advanced workload scheduling and resource segregation.

- Taints on nodes: Nodes in the cluster can be assigned taints, which act as “repellents” to most pods, preventing them from being scheduled on those nodes.
- Tolerations on pods: Only pods with matching tolerations (that can "tolerate" the taint) can be scheduled on those nodes.

### Monitoring and Logging

- Use **Amazon CloudWatch Container Insights** for comprehensive monitoring of metrics and logs.
- Automatically collects data from EKS clusters, providing real-time dashboards for troubleshooting and performance optimization.

### When to Choose EKS

- For Kubernetes-native workloads requiring extensive control and ecosystem integration.
- When migrating from on-premises or multi-cloud Kubernetes deployments.
- When performance optimization with GPU-based EC2 instances or responsive scaling with HPA is critical.


**Cheat Sheets**

https://tutorialsdojo.com/amazon-elastic-kubernetes-service-eks/

https://digitalcloud.training/amazon-ecs-and-eks/

**References:**

https://aws.amazon.com/eks/faqs/

https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html

**Videos**

https://www.youtube.com/results?search_query=Amazon+EKS


**Hands On**

https://www.youtube.com/results?search_query=Amazon+EKS+Hands+on

https://www.youtube.com/watch?v=p6xDCz00TxU


***************************************************************************************************
## <a id="section-04"></a> **4 - AWS Fargate**

![AWS Fargate](../images/Architecture-Service-Icons_06072024/Arch_Containers/64/Arch_AWS-Fargate_64.svg "AWS Fargate")

**Definitions**

A serverless compute engine for containers that works with both Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS).
With Fargate, no manual provisioning, patching, cluster capacity management, or any infrastructure management required.


**Cheat Sheets**

https://tutorialsdojo.com/aws-fargate/

**References:**

https://aws.amazon.com/fargate/

https://aws.amazon.com/fargate/faqs/

https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html

https://aws.amazon.com/blogs/aws/aws-fargate/


**Videos**

https://www.youtube.com/results?search_query=aws+fargate

**Hands On**

https://www.youtube.com/results?search_query=aws+fargate+hands+on