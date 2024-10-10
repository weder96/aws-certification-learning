<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws certification learning

# Module 97: Which key tools, technologies, and concepts might be covered on the exam

## Content

1. <a href="#section_01"> What Is Disaster Recovery? </a>
2. <a href="#section_02"> Resiliency </a>
3. <a href="#section_03"> High Performance Computing </a>
4. <a href="#section_04"> Microservices and component decoupling </a>

***************************************************************************************************
## <a id="section_01"></a> **1 - What Is Disaster Recovery**

**Definitions**

What is Disaster Recovery?

Disaster recovery is the process by which an organization anticipates and addresses technology-related disasters. IT systems in any company can go down unexpectedly due to unforeseen circumstances, such as power outages, natural events, or security issues. Disaster recovery includes a company's procedures and policies to recover quickly from such events.


[Disaster Recovery learning](https://github.com/weder96/aws-certification-learning/tree/main/module-29)

**Cheat Sheets**

**References:**

https://aws.amazon.com/what-is/disaster-recovery/?nc1=h_ls

https://d1.awsstatic.com/whitepapers/aws-disaster-recovery.121b65092f931567af5370b47dd12cb18866089c.pdf

**Videos**

**Hands On**

***************************************************************************************************

## <a id="section_02"></a> **2 - Resiliency**

**Definitions**

Reliability of a workload in the cloud depends on several factors, the primary of which is Resiliency:

Resiliency is the ability of a workload to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand, and mitigate disruptions, such as misconfigurations or transient network issues.

The other factors impacting workload reliability are:

Operational Excellence, which includes automation of changes, use of playbooks to respond to failures, and Operational Readiness Reviews (ORRs) to confirm that applications are ready for production operations.

Security, which includes preventing harm to data or infrastructure from malicious actors, which would impact availability. For example, encrypt backups to ensure that data is secure.

Performance Efficiency, which includes designing for maximum request rates and minimizing latencies for your workload.

Cost Optimization, which includes trade-offs such as whether to spend more on EC2 instances to achieve static stability, or to rely on automatic scaling when more capacity is needed.

Resiliency is the primary focus of this whitepaper.

**Cheat Sheets**

**References:**

https://aws.amazon.com/blogs/architecture/tag/resilience/

https://aws.amazon.com/blogs/architecture/understand-resiliency-patterns-and-trade-offs-to-architect-efficiently-in-the-cloud/

https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/resiliency-and-the-components-of-reliability.html

https://aws.amazon.com/architecture/well-architected/?wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc&wa-guidance-whitepapers.sort-by=item.additionalFields.sortDate&wa-guidance-whitepapers.sort-order=desc

**Videos**

**Hands On**



***************************************************************************************************

## <a id="section_03"></a> **3 - High Performance Computing**

**Definitions**

Run your large, complex simulations and deep learning workloads in the cloud with a complete suite of high performance computing (HPC) products and services on AWS. Gain insights faster, and quickly move from idea to market with virtually unlimited compute capacity, a high-performance file system, and high-throughput networking.


**Cheat Sheets**

**References:**

https://aws.amazon.com/hpc/

https://aws.amazon.com/hpc/campaigns/hpc-at-scale/

https://docs.aws.amazon.com/wellarchitected/latest/high-performance-computing-lens/welcome.html

**Videos**

**Hands On**



***************************************************************************************************

## <a id="section_04"></a> **4 - Microservices and component decoupling**

**Definitions**

Monolithic vs. Microservices Architecture

With monolithic architectures, all processes are tightly coupled and run as a single service. This means that if one process of the application experiences a spike in demand, the entire architecture must be scaled. Adding or improving a monolithic application’s features becomes more complex as the code base grows. This complexity limits experimentation and makes it difficult to implement new ideas. Monolithic architectures add risk for application availability because many dependent and tightly coupled processes increase the impact of a single process failure.

With a microservices architecture, an application is built as independent components that run each application process as a service. These services communicate via a well-defined interface using lightweight APIs. Services are built for business capabilities and each service performs a single function. Because they are independently run, each service can be updated, deployed, and scaled to meet demand for specific functions of an application.


**Cheat Sheets**

**References:**
https://docs.aws.amazon.com/whitepapers/latest/microservices-on-aws/microservices-on-aws.html

https://aws.amazon.com/microservices/

https://docs.aws.amazon.com/prescriptive-guidance/latest/modernization-integrating-microservices/decouple-messaging.html

https://docs.aws.amazon.com/pdfs/whitepapers/latest/microservices-on-aws/microservices-on-aws.pdf


**Videos**

**Hands On**


