<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# [Módulo 18: Containers](https://aws.amazon.com/what-is/compute/)

## Content
1. <a href="#section-01"> Amazon Elastic Container Registry (Amazon ECR) </a>
2. <a href="#section-02"> Amazon Elastic Container Service (Amazon ECS) </a>
3. <a href="#section-03"> Amazon Elastic Kubernetes Service (Amazon EKS) </a>
4. <a href="#section-04"> AWS Fargate </a>

https://tutorialsdojo.com/aws-fargate/

***************************************************************************************************
## <a id="section-01"></a> **1 - Amazon Elastic Container Registry (Amazon ECR)**

![Elastic-Container-Registry](../images/Architecture-Service-Icons_01312022/Arch_Containers/48/Arch_Amazon-Elastic-Container-Registry_48.png "Elastic-Container-Registry")

**Cheat Sheets**

**References:**

**Videos**

***************************************************************************************************
## <a id="section-02"></a> **2 - Amazon Elastic Container Service (Amazon ECS)**

![Elastic-Container-Service](../images/Architecture-Service-Icons_01312022/Arch_Containers/64/Arch_Amazon-Elastic-Container-Service_64.svg "Elastic-Container-Service")

**Definition**

A container management service to run, stop, and manage Docker containers on a cluster.

ECS can be used to create a consistent deployment and build experience, manage, and scale batch and Extract-Transform-Load (ETL) workloads, and build sophisticated application architectures on a microservices model.

Amazon ECS is a **regional service**.

The Amazon Elastic Container Service (ECS) is a highly scalable, high performance container management service that supports **Docker containers**.

Amazon ECS allows you to easily run applications on a managed cluster of Amazon EC2 instances.

Amazon ECS eliminates the need for you to install, operate, and scale your own cluster management infrastructure.

Using API calls you can launch and stop container-enabled applications, query the complete state of clusters, and access features like security groups, Elastic Load Balancing, EBS volumes and IAM roles.

Amazon ECS can be used to schedule the placement of containers across clusters based on resource needs and availability requirements.

There is no additional charge for Amazon ECS. You pay for:

Resources created with the EC2 Launch Type (e.g. EC2 instances and EBS volumes).
The number and configuration of tasks you run for the Fargate Launch Type.

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

![Amazon-EKS-Cloud](../images/Architecture-Service-Icons_01312022/Arch_Containers/64/Arch_Amazon-Elastic-Kubernetes-Service_64.svg "Amazon-EKS-Cloud")

**Definition**

### What is Amazon EKS?

A managed service that allows you to run Kubernetes on AWS without installing, operating, or maintaining your own Kubernetes control plane or nodes.

Integration with various AWS services to provide scalability and security for your applications:

Amazon ECR for container images

Elastic Load Balancing for load distribution

IAM for authentication

Amazon VPC for isolation

### **Amazon EKS Anywhere**

![Amazon-EKS-Cloud](../images/Architecture-Service-Icons_01312022/Arch_Containers/64/Arch_Amazon-EKS-Anywhere_64.svg "Amazon-EKS-Cloud")

Using Amazon EKS Anywhere is another way to deploy your containers on-premises. 

It works like Amazon ECS Anywhere, which allows you to run your containerized cluster entirely on your own. 

This means that the hardware, app deployment location, control plane, and data plane are all controlled on your own physical network. 

This gives you extensive control over all the components of your containerized application suite while maintaining official support from AWS.

### **Amazon EKS Distro**
![Amazon EKS Distro](../images/Architecture-Service-Icons_01312022/Arch_Containers/64/Arch_Amazon-EKS-Distro_64.svg "Amazon EKS Distro")

The other deployment option that you can choose is Amazon EKS Distro. 

The word “distro” simply refers to the distribution of the same open-source Kubernetes software deployed by Amazon EKS in the AWS cloud. 

Amazon EKS Distro follows the same Kubernetes version release cycle as Amazon EKS and is provided to you as an open-source project that you can deploy on your own computer or on-site environment. 

It’s similar to the Amazon EKS Anywhere option, except that it does not include support services offered by AWS.
 

### **Amazon EKS Pricing**

For each Amazon EKS cluster you create, you are charged an hourly rate.

You are charged for the AWS resources that you create to run Kubernetes worker nodes in Amazon EC2 with Amazon EKS managed node groups.

In Amazon EKS on AWS Fargate, you are charged for the vCPU and memory resources.

Amazon EKS on AWS Outposts charges an hourly rate for EKS clusters deployed in the cloud, but there is no additional charge for Kubernetes worker nodes running on Outposts EC2.


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

![AWS Fargate](../images/Architecture-Service-Icons_01312022/Arch_Containers/64/Arch_AWS-Fargate_64.svg "AWS Fargate")

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