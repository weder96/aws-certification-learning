<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws certification learning

# Module 26: Developer Tools

## Content

1. <a href="#section_01">AWS X-Ray</a>
2. <a href="#section_02">AWS Cloud9</a>
3. <a href="#section_03">AWS CodeStar</a>
4. <a href="#section_04">AWS CodeBuild</a>
5. <a href="#section_05">AWS CloudShell</a>
6. <a href="#section_06">AWS CodeCommit</a>
7. <a href="#section_07">AWS CodeDeploy</a>
8. <a href="#section_08">Amazon Corretto</a>
9. <a href="#section_09">AWS CodeArtifact</a>
10. <a href="#section_10">AWS CodePipeline</a>
11. <a href="#section_11">AWS Tools and SDKs</a>
12. <a href="#section_12">AWS Cloud Development Kit</a>
13. <a href="#section_13">AWS Command Line Interface</a>

***************************************************************************************************
## <a id="section_01"></a> **1 - AWS X-Ray**
![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-X-Ray_64.svg)

**Cheat Sheets**

**References:**

**Videos**

**Hands On**

***************************************************************************************************
## <a id="section_02"></a> **2 - AWS Cloud9**
![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-Cloud9_64.svg)

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

### **Concepts**

- A **build project** defines how CodeBuild will run a build. It includes information such as where to get the source code, which build environment to use, the build commands to run, and where to store the build output.

- A **build environment** is the combination of operating system, programming language runtime, and tools used by CodeBuild to run a build.

- The **build specification** is a YAML file that lets you choose the commands to run at each phase of the build and other settings. Without a build spec, CodeBuild cannot successfully convert your build input into build output or locate the build output artifact in the build environment to upload to your output bucket.
    - If you include a build spec as part of the source code, by default, the build spec file must be named buildspec.yml and placed in the root of your source directory.

- A collection of input files is called build input artifacts or build input and a deployable version of a source code is called build output artifact or build output.

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

**Cheat Sheets**

**References:**

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section_13"></a> **13 - AWS Command Line Interface**

![01](../images/Architecture09172021/Arch_Developer-Tools/64/Arch_AWS-Command-Line-Interface_64.svg)

**Cheat Sheets**

**References:**

**Videos**

**Hands On**