<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws certification learning

# Module 26: Developer Tools

## Content

1.  <a href="#section_01">AWS X-Ray</a>
2.  <a href="#section_02">AWS Cloud9</a>
3.  <a href="#section_03">AWS CodeStar</a>
4.  <a href="#section_04">AWS CodeBuild</a>
5.  <a href="#section_05">AWS CloudShell</a>
6.  <a href="#section_06">AWS CodeCommit</a>
7.  <a href="#section_07">AWS CodeDeploy</a>
8.  <a href="#section_08">Amazon Corretto</a>
9.  <a href="#section_09">AWS CodeArtifact</a>
10. <a href="#section_10">AWS CodePipeline</a>
11. <a href="#section_11">AWS Tools and SDKs</a>
12. <a href="#section_12">AWS Cloud Development Kit</a>
13. <a href="#section_13">AWS Command Line Interface</a>

***************************************************************************************************
## <a id="section_01"></a> **1 - AWS X-Ray**
![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-X-Ray_64.svg)

**Definitions**

- AWS X-Ray analyzes and debugs production, distributed applications, such as those built using a microservices architecture. With X-Ray, you can identify performance bottlenecks, edge case errors, and other hard to detect issues.

### **Pricing**
- You pay based on the number of traces recorded, retrieved, and scanned. A trace represents a request to your application and may include multiple data points, such as for calls to other services and database access.
- The maximum size of a trace is 500 KB.
- Trace data is retained for 30 days from the time it is recorded at no additional cost.

**Cheat Sheets**

https://tutorialsdojo.com/aws-x-ray/

**References:**

https://aws.amazon.com/xray/features/

https://aws.amazon.com/xray/pricing/

https://docs.aws.amazon.com/xray/latest/devguide/aws-xray.html

https://aws.amazon.com/xray/faqs/

**Videos**

https://youtu.be/5MQkX57eTh8

https://www.youtube.com/results?search_query=AWS+x-ray

**Hands On**

https://www.youtube.com/results?search_query=AWS+x-ray+hands+on++

***************************************************************************************************
## <a id="section_02"></a> **2 - AWS Cloud9**
![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-Cloud9_64.svg)

### **Definitions**

**AWS Cloud9** is a cloud-based integrated development environment (IDE) that allows developers to write, run, and debug code directly from a web browser. It provides a rich set of features, including a code editor, a terminal, and debugging tools, all integrated into a single environment. Cloud9 is particularly useful for developers who need an environment that can be easily accessed from anywhere without the need for complex local setups.

Key Features:

- **Browser-Based IDE**: Access your development environment from any device with an internet connection.
- **Preconfigured with AWS Tools**: AWS Cloud9 comes preconfigured with the AWS SDKs and command-line tools, making it easy to develop applications that interact with AWS services.
- **Collaborative Development**: You can invite team members to work on the same code in real time, which simplifies collaboration on projects.
- **Support for Multiple Languages**: AWS Cloud9 supports multiple programming languages such as Python, JavaScript, PHP, Ruby, and more.
- **Built-in Terminal**: Integrated with a terminal that allows you to run AWS CLI commands directly from the IDE.
- **Debugging Tools**: Provides powerful debugging tools, including breakpoints, stack traces, and variable inspection.

**Use Case**:
AWS Cloud9 is particularly useful for cloud-based development, remote teams, or anyone needing to access a development environment without managing local resources. It is also handy for serverless application development, as it integrates easily with other AWS services like AWS Lambda.


**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_03"></a> **3 - AWS CodeStar**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CodeStar_64.svg)

**Definitions**

AWS CodeStar enables you to quickly develop, build, and deploy applications on AWS. AWS CodeStar provides a unified user interface, enabling you to easily manage your software development activities in one place. With AWS CodeStar, you can set up your entire continuous delivery toolchain in minutes, allowing you to start releasing code faster. AWS CodeStar makes it easy for your whole team to work together securely, allowing you to easily manage access and add owners, contributors, and viewers to your projects. Each AWS CodeStar project comes with a project management dashboard, including an integrated issue tracking capability powered by Atlassian JIRA Software. With the AWS CodeStar project dashboard, you can easily track progress across your entire software development process, from your backlog of work items to teams’ recent code deployments. Visit here to learn more.

There is no additional charge for using AWS CodeStar. You only pay for the AWS resources that you provision for developing and running your application (for example, Amazon EC2 instances).

**Cheat Sheets**

https://tutorialsdojo.com/aws-codestar/

**References:**

https://aws.amazon.com/codestar/

https://docs.aws.amazon.com/codestar/latest/userguide/welcome.html

https://aws.amazon.com/codestar/faqs/?nc=sn&loc=4

https://aws.amazon.com/codestar/?nc1=h_ls

**Videos**

https://www.youtube.com/results?search_query=+AWS+CodeStar

**Hands On**

https://www.youtube.com/results?search_query=+AWS+CodeStar+Hands+On

***************************************************************************************************
## <a id="section_04"></a> **4 - AWS CodeBuild**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CodeBuild_64.svg)

**Definition**

A fully managed continuous integration service that compiles source code, runs tests, and produces software packages that are ready to deploy.

AWS **CodeBuild** is a fully managed, serverless build service that compiles source code, runs tests, and produces deployment-ready packages. It integrates seamlessly with other AWS services, such as CodePipeline and CodeDeploy, making it an essential component for building a robust CI/CD pipeline.

### **Concepts**

- A **build project** defines how CodeBuild will run a build. It includes information such as where to get the source code, which build environment to use, the build commands to run, and where to store the build output.

- A **build environment** is the combination of operating system, programming language runtime, and tools used by CodeBuild to run a build.

- The **build specification** is a YAML file that lets you choose the commands to run at each phase of the build and other settings. Without a build spec, CodeBuild cannot successfully convert your build input into build output or locate the build output artifact in the build environment to upload to your output bucket.
    - If you include a build spec as part of the source code, by default, the build spec file must be named buildspec.yml and placed in the root of your source directory.

- A collection of input files is called build input artifacts or build input and a deployable version of a source code is called build output artifact or build output.

### Key Features

- **Fully Managed and Scalable**: CodeBuild automatically scales to meet your build requirements, without the need to manage infrastructure.
- **Secure and Pay-As-You-Go**: You only pay for the build time you use, and builds are isolated for security.
- **Buildspec File**: CodeBuild uses a `buildspec.yml` file that defines the build commands, environment variables, and runtime environment for your build, allowing for highly customizable build configurations.
- **Integrates with AWS Services**: Works seamlessly with CodeCommit, CodePipeline, CodeDeploy, and other AWS services to automate the entire build and deployment process.

### Use Cases

- **Automated Build Process**: Automates compiling source code, running unit tests, and preparing the application for deployment.
- **Customizable Build Environment**: Through `buildspec.yml`, developers can configure the build environment for different resource requirements, such as different compute resources for intensive builds.


**Cheat Sheets**

https://digitalcloud.training/aws-developer-tools/

https://tutorialsdojo.com/aws-codebuild/

**References:**

https://aws.amazon.com/codebuild/features/?nc=sn&loc=2

https://aws.amazon.com/codebuild/pricing/?nc=sn&loc=3

https://aws.amazon.com/codebuild/faqs/?nc=sn&loc=5

https://docs.aws.amazon.com/codebuild/latest/userguide/getting-started.html

**Videos**

https://www.youtube.com/watch?v=3lGga5rqbts

**Hands On**

https://www.youtube.com/results?search_query=CodeBuild+Hands+on



***************************************************************************************************
## <a id="section_05"></a> **5 - AWS CloudShell**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CloudShell_64.svg)

**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_06"></a> **6 - AWS CodeCommit**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CodeCommit_64.svg)

**Definition**

AWS **CodeCommit** is a fully managed source control service that hosts Git repositories. While AWS CodeCommit is still available, it is being gradually phased out, with new customers unable to sign up for the service after July 25, 2024. AWS recommends migrating to a third-party Git solution, such as GitHub.
- A fully-managed source control service that hosts secure Git-based repositories, similar to Github.
- You can create your own code repository and use Git commands to interact with your own repository and other repositories.
- You can store and version any kind of file, including application assets such as images and libraries alongside your code.
- The AWS CodeCommit Console lets you visualize your code, pull requests, commits, branches, tags and other settings.


### **Concepts**

- An active user is any unique AWS identity (IAM user/role, federated user, or root account) that accesses AWS CodeCommit repositories during the month. AWS identities that are created through your use of other AWS Services, such as AWS CodeBuild and 
AWS CodePipeline, as well as servers accessing CodeCommit using a unique AWS identity, count as active users.

- A **repository** is the fundamental version control object in CodeCommit. It’s where you securely store code and files for your project. It also stores your project history, from the first commit through the latest changes.
- A **file** is a version-controlled, self-contained piece of information available to you and other users of the repository and branch where the file is stored.
- A **pull request** allows you and other repository users to review, comment on, and merge code changes from one branch to another.
- An **approval** rule is used to designate a number of users who will approve a pull request before it is merged into your branch.
- A **commit** is a snapshot of the contents and changes to the contents of your repository. This includes information like who committed the change, the date and time of the commit, and the changes made as part of the commit.
- In **Git**, branches are simply pointers or references to a commit. You can use branches to separate work on a new or different version of files without impacting work in other branches. You can use branches to develop new features, store a specific version of your project from a particular commit, etc.

### **Pricing**

- The first 5 active users per month are free of charge. You also get to have unlimited repositories, with 50 GB-month total worth of storage, and 10,000 Git requests/month at no cost.
- You are billed for each active user beyond the first 5 per month. You also get an additional 10GB-month of storage per active user, and an additional 2,000 Git requests per active user.
    - A Git request includes any push or pull that transmits repository objects, including a direct edit in the console or through the CodeCommit APIs.

### **Limits**

- 1,000 repositories by default (no limits upon request). 
- A single blob in a repository cannot be more than 2 GB in size.
- Total size of your files in a single commit should not be more than 20 MB.
- An individual file should not exceed 6 MB.

### Key Features

- **Git-based Repository**: Provides a secure and scalable Git repository for storing and versioning your source code.
- **Integrated with AWS Services**: Seamlessly integrates with AWS tools like CodeBuild, CodeDeploy, and CodePipeline, making it easy to build a complete CI/CD pipeline.
- **Secure and Private**: CodeCommit ensures that repositories are secure, private, and integrated with IAM for fine-grained access control.
- **Scalable and Highly Available**: As a fully managed service, CodeCommit automatically scales with your usage and ensures high availability.

### Use Cases

- **Version Control**: Used primarily for storing and versioning code in a private and secure repository.
- **Integration with CI/CD**: Works well with AWS CI/CD tools like CodePipeline, CodeBuild, and CodeDeploy to automate the delivery process.


**Cheat Sheets**

https://tutorialsdojo.com/aws-codecommit/

https://digitalcloud.training/aws-developer-tools/

**References:**

https://aws.amazon.com/codecommit/

https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html

https://aws.amazon.com/codecommit/faqs/


**Videos**

https://www.youtube.com/results?search_query=AWS+CodeCommit+

**Hands On**

https://www.youtube.com/results?search_query=AWS+CodeCommit+Hands+on


***************************************************************************************************
## <a id="section_07"></a> **7 - AWS CodeDeploy**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CodeDeploy_64.svg)


**Definition**
- A fully managed deployment service that automates software deployments to a variety of compute services such as Amazon EC2, AWS Fargate, AWS Lambda, and your on-premises servers.

AWS **CodeDeploy** is a fully managed deployment service that automates the deployment of applications to a variety of compute services, such as Amazon EC2 instances, Lambda functions, and even on-premises servers. CodeDeploy supports rolling updates, blue-green deployments, and can be integrated with other AWS services like AWS CodePipeline for seamless, automated application delivery.

### **Concepts**

- An Application is a name that uniquely identifies the application you want to deploy. CodeDeploy uses this name, which functions as a container, to ensure the correct combination of revision, deployment configuration, and deployment group are referenced during a deployment.
- Compute platform is the platform on which CodeDeploy deploys an application (EC2, ECS, Lambda, On-premises servers).
- Deployment configuration is a set of deployment rules and deployment success and failure conditions used by CodeDeploy during a deployment.
- Deployment group contains individually tagged instances, Amazon EC2 instances in Amazon EC2 Auto Scaling groups, or both.
    - In an Amazon ECS deployment, a deployment group specifies the Amazon ECS service, load balancer, optional test listener, and two target groups. It also specifies when to reroute traffic to the replacement task set and when to terminate the original task set and ECS application after a successful deployment.
    - In an AWS Lambda deployment, a deployment group defines a set of CodeDeploy configurations for future deployments of an AWS Lambda function.
    - In an EC2/On-Premises deployment, a deployment group is a set of individual instances targeted for a deployment.
        - In an in-place deployment, the instances in the deployment group are updated with the latest application revision.
        - In a blue/green deployment, traffic is rerouted from one set of instances to another by deregistering the original instances from a load balancer and registering a replacement set of instances that typically has the latest application revision already installed.

### Key Features

- **Supports EC2 & On-Premises Deployments**: CodeDeploy can manage deployments to EC2 instances as well as on-premises servers, making it a flexible solution for hybrid cloud environments.
- **Deployment Strategies**: CodeDeploy supports multiple deployment strategies, including:
  - **Rolling deployments**: Gradual deployment of new application versions to EC2 instances.
  - **Blue/Green deployments**: Shifting traffic between two environments (blue and green) to ensure minimal downtime and rapid rollback capabilities.
- **Integrated with AWS Services**: Easily integrates with services like CodePipeline for CI/CD, and Lambda for serverless deployments.
- **Customizable Deployment**: CodeDeploy allows you to customize deployment scripts (like hooks) to run specific actions at various stages of the deployment process.

### Use Cases

- **Automated Application Deployment**: Ideal for automatically deploying updates to applications on EC2 instances, Lambda, or on-premises systems.
- **Zero-Downtime Deployments**: Blue/Green deployments help ensure that your application has no downtime during updates.




**Cheat Sheets**

https://digitalcloud.training/aws-developer-tools/

https://tutorialsdojo.com/aws-codedeploy/

**References:**

https://aws.amazon.com/codedeploy/features/?nc=sn&loc=2

https://docs.aws.amazon.com/codedeploy/latest/userguide/welcome.html

https://aws.amazon.com/codedeploy/faqs/?nc=sn&loc=6

**Videos**

https://www.youtube.com/results?search_query=AWS+CodeDeploy+

https://www.youtube.com/watch?time_continue=1&v=ClWBJT6k20Q&embeds_euri=https%3A%2F%2Ftutorialsdojo.com%2F&feature=emb_logo

**Hands On**

https://www.youtube.com/results?search_query=AWS+CodeDeploy++Hands+On


***************************************************************************************************
## <a id="section_08"></a> **8 - AWS Corretto**

![08](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_Amazon-Corretto_64.svg)

**Definition**

**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_09"></a> **9 - AWS CodeArtifact**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CodeArtifact_64.svg)

**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_10"></a> **10 - AWS CodePipeline**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-CodePipeline_64.svg)

**Definitions**

AWS **CodePipeline** is a fully managed service that automates the build, test, and deployment processes in a continuous integration and continuous delivery (CI/CD) workflow. CodePipeline orchestrates the entire CI/CD pipeline, integrating services like CodeCommit for source control, CodeBuild for building and testing, and CodeDeploy for deployment.

- A fully managed continuous delivery service that helps you automate your release pipelines for application and infrastructure updates.
- You can easily integrate AWS CodePipeline with third-party services such as GitHub or with your own custom plugin

### **Concepts**

- A pipeline defines your release process workflow, and describes how a new code change progresses through your release process.
- A pipeline comprises a series of stages (e.g., build, test, and deploy), which act as logical divisions in your workflow. Each stage is made up of a sequence of actions, which are tasks such as building code or deploying to test environments.
    - Pipelines must have at least two stages. The first stage of a pipeline is required to be a source stage, and the pipeline is required to additionally have at least one other stage that is a build or deployment stage.
- Define your pipeline structure through a declarative JSON document that specifies your release workflow and its stages and actions. These documents enable you to update existing pipelines as well as provide starting templates for creating new pipelines.
- A revision is a change made to the source location defined for your pipeline. It can include source code, build output, configuration, or data. A pipeline can have multiple revisions flowing through it at the same time.
- A stage is a group of one or more actions. A pipeline can have two or more stages.
- An action is a task performed on a revision. Pipeline actions occur in a specified order, in serial or in parallel, as determined in the configuration of the stage.
    - You can add actions to your pipeline that are in an AWS Region different from your pipeline.
    - There are six types of actions
        - Source
        - Build
        - Test
        - Deploy
        - Approval
        - Invoke

- When an action runs, it acts upon a file or set of files called artifacts. These artifacts can be worked upon by later actions in the pipeline. You have an artifact store which is an S3 bucket in the same AWS Region as the pipeline to store items for all pipelines in that Region associated with your account.
- The stages in a pipeline are connected by transitions. Transitions can be disabled or enabled between stages. If all transitions are enabled, the pipeline runs continuously.
- An approval action prevents a pipeline from transitioning to the next action until permission is granted. This is useful when you are performing code reviews before code is deployed to the next stage.


### ** Limits**

- Maximum number of total pipelines per Region in an AWS account is 300
- Number of stages in a pipeline is minimum of 2, maximum of 10

### **Pricing**

- You are charged per active pipeline each month. Newly created pipelines are free to use during the first 30 days after creation.


### Key Features

- **End-to-End Automation**: CodePipeline allows you to automate the entire software delivery process, from source control to deployment.
- **Seamless Integrations**: Easily integrates with other AWS services like CodeCommit, CodeBuild, CodeDeploy, Elastic Beanstalk, CloudFormation, and even third-party services like GitHub.
- **Conditional Execution**: Supports conditional execution of actions, allowing you to customize workflows based on predefined criteria.
- **Fast Delivery and Rapid Updates**: CodePipeline enables rapid application updates and faster time-to-market by automating the workflow.

### Use Cases

- **Automating CI/CD Pipelines**: Automates the entire pipeline process, including building, testing, and deploying applications.
- **Continuous Integration & Delivery**: Ensures your code changes are built, tested, and deployed continuously for faster updates and releases.


**Cheat Sheets**

https://tutorialsdojo.com/aws-codepipeline/

**References:**

https://aws.amazon.com/codepipeline/features/?nc=sn&loc=2

https://aws.amazon.com/codepipeline/pricing/?nc=sn&loc=3

https://docs.aws.amazon.com/codepipeline/latest/userguide/welcome.html

https://aws.amazon.com/codepipeline/faqs/?nc=sn&loc=5

**Videos**

https://www.youtube.com/results?search_query=aws+codepipeline+

**Hands On**

https://www.youtube.com/results?search_query=aws+codepipeline++Hands+On

***************************************************************************************************
## <a id="section_11"></a> **11 - AWS Tools and SDKs<**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-Tools-and-SDKs_64.svg)

**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_12"></a> **12 - Cloud Development Kit**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-Cloud-Development-Kit_64.svg)

### **Definitions**

The **AWS Cloud Development Kit (CDK)** is a powerful framework for defining cloud infrastructure in a high-level programming language, allowing developers to use familiar programming languages to model and provision AWS resources. It abstracts the complexities of AWS infrastructure management by providing constructs, which are high-level components that can be used to create AWS resources.

- **Programming Languages**: The AWS CDK supports a variety of languages such as JavaScript, TypeScript, Python, Java, and .NET, making it accessible to developers from different backgrounds.
- **Constructs**: In CDK, the building blocks for your infrastructure are called constructs. These are pre-configured components that represent AWS resources, and you can easily use and customize them in your code.
- **CloudFormation Integration**: While the CDK code is written in a high-level language, it is “compiled” into an underlying **CloudFormation template** (in JSON or YAML format). This enables users to take advantage of CloudFormation's powerful features for provisioning and managing AWS resources.
- **Infrastructure and Application Code Together**: One of the standout features of the CDK is that it allows you to deploy both infrastructure and application runtime code together. This makes it ideal for **Lambda functions** and **Docker containers** running in services like **ECS** and **EKS**.
- **Flexibility**: The CDK is extremely flexible, supporting all AWS services, from EC2 instances to serverless resources, and allowing you to model everything in code.

The CDK is a great tool for developers who are familiar with coding and want to manage their AWS resources in the same way they write application code. It enables rapid development, iteration, and deployment of cloud infrastructure with much more flexibility and control compared to traditional declarative templates.

### Comparison of AWS CDK and SAM

| Feature                       | **AWS CDK**                                     | **AWS SAM**                                  |
|-------------------------------|-------------------------------------------------|----------------------------------------------|
| **Focus**                      | General-purpose cloud infrastructure deployment | Serverless applications, especially Lambda  |
| **Supported Languages**        | JavaScript, TypeScript, Python, Java, .NET      | JSON/YAML (Declarative Templates)            |
| **Abstraction Level**          | High-level, object-oriented constructs          | Declarative, simplifies Lambda & API Gateway |
| **Flexibility**                | Supports all AWS services                       | Focused on Lambda, API Gateway, DynamoDB    |
| **Deployment Model**           | Infrastructure and application code together    | Declarative, limited to specific serverless components |
| **CloudFormation Integration** | Generates CloudFormation templates              | Leverages CloudFormation natively            |
| **Ease of Use**                | Requires programming skills for setup           | Easier to start with, especially for Lambda  |
| **Use Case**                   | Full-scale infrastructure (including Lambda, ECS, EKS, etc.) | Ideal for quick serverless Lambda setups    |

In summary, **AWS CDK** is a versatile framework that can be used for any type of AWS service, giving developers the ability to use familiar programming languages to manage infrastructure, while **AWS SAM** is a more specialized, declarative tool focused on simplifying the deployment of serverless applications such as AWS Lambda functions.


**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_13"></a> **13 - AWS Command Line Interface**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-Command-Line-Interface_64.svg)


### **Definitions**

The **AWS Command Line Interface (CLI)** is a tool that allows you to interact with AWS services using commands directly in your command-line shell. It provides direct access to the public APIs of AWS services, making it a powerful tool for managing and automating AWS resources. The AWS CLI is commonly used for scripting and automating repetitive tasks, as well as for managing resources at scale.

- **Open-source**: The AWS CLI is open-source and can be found on [GitHub](https://github.com/aws/aws-cli).
- **Direct API Access**: It interacts directly with AWS services' public APIs, enabling you to perform actions like creating, managing, and deleting resources.
- **Command-Line Alternative**: The AWS CLI is a convenient alternative to the AWS Management Console, especially for those who prefer command-line interfaces or need automation.
- **Automation & Scripting**: You can develop scripts to automate tasks such as launching EC2 instances, managing S3 buckets, or configuring IAM roles.
- **SSH Access**: The AWS CLI also supports SSH functionality for secure remote access to your EC2 instances. It allows you to connect to and manage instances directly from the command line, which is especially useful for instance management or troubleshooting.

Overall, the AWS CLI is a powerful tool for AWS resource management, automation, and monitoring in environments where a GUI might not be ideal.


**Cheat Sheets**

**References:**

**Videos**

**Hands On**