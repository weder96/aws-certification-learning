<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Module 5: Networking and Content Delivery:

## Content
01. <a href="#section-1">  Amazon CloudFront  </a>
02. <a href="#section-2">  AWS Direct Connect  </a>
03. <a href="#section-3">  Elastic Load Balancing (ELB) </a> 
04. <a href="#section-4">  AWS Global Accelerator  </a>
05. <a href="#section-5">  AWS PrivateLink  </a>
06. <a href="#section-6">  Amazon Route 53  </a>
07. <a href="#section-7">  AWS Transit Gateway  </a> 
08. <a href="#section-8">  Amazon VPC </a> 
09. <a href="#section-9">  AWS VPN </a>
10. <a href="#section-10"> Amazon API Gateway </a>
11. <a href="#section-11"> Amazon VPC Lattice </a>
12. <a href="#section-12"> AWS App Mesh </a>
13. <a href="#section-13"> AWS Client VPN </a>
14. <a href="#section-14"> AWS Cloud WAN </a>
15. <a href="#section-15"> AWS Private 5G </a>
16. <a href="#section-16"> AWS Site-to-Site VPN </a>
17. <a href="#section-17"> AWS Verified Access </a>
18. <a href="#section-18"> AWS Network Firewall </a>
98. <a href="#section-98"> Networks Comments </a>
99. <a href="#section-99"> Additional resources </a>

***************************************************************************************************
## <a id="section-1"></a> **1 - Amazon CloudFront**

![Amazon CloudFront](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_Amazon-CloudFront_64.png "Amazon CloudFront")

**Cheat Sheets**

https://tutorialsdojo.com/amazon-cloudfront/

https://digitalcloud.training/amazon-cloudfront/

**References:**

https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide

https://aws.amazon.com/cloudfront/features/

https://aws.amazon.com/cloudfront/pricing/

https://aws.amazon.com/cloudfront/faqs/

https://aws.amazon.com/cloudfront/streaming/

https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/on-demand-streaming-video.html

**Videos**

https://www.youtube.com/user/AmazonWebServices/search?query=CloudFront


***************************************************************************************************
## <a id="section-2"></a> **2 - AWS Direct Connect**

![Amazon CloudFront](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_AWS-Direct-Connect_64.png "AWS Direct Connect")

**Cheat Sheets**

https://tutorialsdojo.com/aws-direct-connect/

**References:**

https://docs.aws.amazon.com/directconnect/latest/UserGuide

https://aws.amazon.com/directconnect/features/

https://aws.amazon.com/directconnect/pricing/

https://aws.amazon.com/directconnect/faqs/

**Videos**

https://www.youtube.com/results?search_query=aws+direct+connect


***************************************************************************************************
## <a id="section-3"></a> **3 - Elastic Load Balancing (ELB)**

![Elastic Load Balancing (ELB)](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_Elastic-Load-Balancing_64.png "Elastic Load Balancing (ELB)")

**Cheat Sheets**

https://digitalcloud.training/aws-elastic-load-balancing-aws-elb/

https://tutorialsdojo.com/aws-elastic-load-balancing-elb/

https://tutorialsdojo.com/application-load-balancer-vs-network-load-balancer-vs-classic-load-balancer/

**References:**

https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html

https://docs.aws.amazon.com/elasticloadbalancing/latest/network/introduction.html

https://docs.aws.amazon.com/elasticloadbalancing/latest/classic/introduction.html

https://aws.amazon.com/elasticloadbalancing/features/

https://aws.amazon.com/elasticloadbalancing/pricing/?nc=sn&loc=3

**Videos**

https://www.youtube.com/results?search_query=aws+Elastic+Load+Balancing

***************************************************************************************************
## <a id="section-4"></a> **4 - AWS Global Accelerator**

![AWS Global Accelerator](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_AWS-Global-Accelerator_64.png "AWS Global Accelerator")


**Definitions**

A service that uses the AWS Global Network to improve the availability and performance of your applications to your local and global users. 
It provides static IP addresses that act as a fixed entry point to your application endpoints in a single or multiple AWS Regions, such as your Application Load Balancers, Network Load Balancers or Amazon EC2 instances.
AWS Global Accelerator continually monitors the health of your application endpoints and will detect an unhealthy endpoint and redirect traffic to healthy endpoints in less than 1 minute.


### **Concepts**

An accelerator is the resource you create to direct traffic to optimal endpoints over the AWS global network.

Network zones are isolated units with their own set of physical infrastructure and service IP addresses from a unique IP subnet.

AWS Global Accelerator provides you with a set of two static IP addresses that are anycast from the AWS edge network. It also assigns a default Domain 
Name System (DNS) name to your accelerator, similar to a1234567890abcdef.awsglobalaccelerator.com, that points to the static IP addresses.

A listener processes inbound connections from clients to Global Accelerator, based on the port (or port range) and protocol that you configure. Global 
Accelerator supports both TCP and UDP protocols.

Each endpoint group is associated with a specific AWS Region. Endpoint groups include one or more endpoints in the Region.

Endpoints can be Network Load Balancers, Application Load Balancers, EC2 instances, or Elastic IP addresses.



**Cheat Sheets**

https://tutorialsdojo.com/aws-global-accelerator/

**References:**

https://aws.amazon.com/global-accelerator/

https://aws.amazon.com/global-accelerator/faqs/

https://docs.aws.amazon.com/pt_br/global-accelerator/latest/dg/what-is-global-accelerator.html

**Videos**

https://www.youtube.com/results?search_query=aws+AWS+Global+Accelerator


***************************************************************************************************
## <a id="section-5"></a> **5 - AWS PrivateLink**

![](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_AWS-PrivateLink_64.png "AWS PrivateLink")

**Definitions**

**Cheat Sheets**

**References:**

https://docs.aws.amazon.com/vpc/latest/userguide/endpoint-services-overview.html

**Videos**

https://www.youtube.com/results?search_query=AWS+PrivateLink

***************************************************************************************************
## <a id="section-6"></a> **6 - Amazon Route 53**

![Amazon Route 53 ](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_Amazon-Route-53_64.png "Amazon Route 53 ")

**Cheat Sheets**

https://digitalcloud.training/amazon-route-53/

https://digitalcloud.training/aws-content-delivery-and-dns-services/

https://tutorialsdojo.com/amazon-route-53/

**References:**

https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html

https://aws.amazon.com/route53/features/

https://aws.amazon.com/route53/pricing/

**Videos**

https://www.youtube.com/user/AmazonWebServices/search?query=Route+53



***************************************************************************************************
## <a id="section-7"></a> **7 - AWS Transit Gateway**

![AWS Transit Gateway ](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_AWS-Transit-Gateway_64.png "AWS Transit Gateway ")

**How it works**

AWS Transit Gateway connects your Amazon Virtual Private Clouds (VPCs) and on-premises networks through a central hub. This connection simplifies your network and puts an end to complex peering relationships. Transit Gateway acts as a highly scalable cloud router—each new connection is made only once.

**Benefits**
- Streamline your architecture
- Better visibility and control
- Improve security
- Lift and shift


**Why Transit Gateway?**

AWS Transit Gateway helps you design and implement networks at scale by acting as a cloud router. As your network grows, the complexity of managing incremental connections can slow you down. 
AWS Transit Gateway connects VPCs and on-premises networks through a central hub.

**Use cases**

- Deliver applications around the world
- Rapidly move to global scale
- Smoothly respond to spikes in demand
- Host multicast applications on AWS



**Cheat Sheets**

https://tutorialsdojo.com/aws-transit-gateway/

https://digitalcloud.training/aws-direct-connect/

**References:**

https://aws.amazon.com/transit-gateway/

**Videos**

https://www.youtube.com/results?search_query=AWS+Transit+Gateway

https://youtu.be/xlTHkoKR-Os

***************************************************************************************************
## <a id="section-8"></a> **8 - Amazon VPC**

![Amazon VPC](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_Amazon-Virtual-Private-Cloud_64.png "Amazon VPC")

An Amazon VPC includes multiple Availability Zones. Within a VPC you can create subnets in each AZ that is available in the Region and distribute your resources across these subnets for high availability.



**Cheat Sheets**
https://tutorialsdojo.com/amazon-vpc/

https://digitalcloud.training/aws-networking-services/

**References:**

https://aws.amazon.com/vpc

https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html

https://aws.amazon.com/vpc/details/

https://aws.amazon.com/vpc/pricing/

https://aws.amazon.com/vpc/faqs/

**Videos**

https://www.youtube.com/results?search_query=Amazon+vpc

https://www.youtube.com/watch?v=jZAvKgqlrjY&t=1s

***************************************************************************************************
## <a id="section-9"></a> **9 - AWS VPN**

![Amazon CloudFront](../images/Architecture-Service-Icons_06072024/Arch_Networking-Content-Delivery/64/Arch_AWS-Client-VPN_64.png "AWS VPN")

**Cheat Sheets**

**References:**

https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/what-is.html

**Videos**

https://www.youtube.com/results?search_query=AWS+Client+VPN



***************************************************************************************************
## <a id="section-10"></a> **10 - Amazon API Gateway**

![API-Gateway](../images/Architecture09172021/Arch_App-Integration/Arch_64/Arch_Amazon-API-Gateway_64.svg)

**Cheat Sheets**

https://tutorialsdojo.com/amazon-api-gateway/


**References:**

https://docs.aws.amazon.com/apigateway/latest/developerguide/

https://aws.amazon.com/api-gateway/features/

https://aws.amazon.com/api-gateway/pricing/

https://aws.amazon.com/api-gateway/faqs/

**Videos**

https://www.youtube.com/results?search_query=aws+api+gateway




***************************************************************************************************
## <a id="section-11"></a> **11 - Amazon VPC Lattice**


***************************************************************************************************
## <a id="section-12"></a> **12 - AWS App Mesh**


***************************************************************************************************
## <a id="section-13"></a> **13 - AWS Client VPN**

***************************************************************************************************
## <a id="section-14"></a> **14 - AWS Cloud WAN**

***************************************************************************************************
## <a id="section-15"></a> **15 - AWS Private 5G**

***************************************************************************************************
## <a id="section-16"></a> **16 - AWS Site-to-Site VPN**


***************************************************************************************************
## <a id="section-17"></a> **17 - AWS Verified Access**


***************************************************************************************************
## <a id="section-18"></a> **18 - AWS Network Firewall**

![Amazon Artifact](../images/Architecture09172021/Arch_Security-Identity-Compliance/48/Arch_AWS-Network-Firewall_48.png)


- Protect your entire Amazon VPC
- From Layer 3 to Layer 7 protection
- Any direction, you can inspect
    - VPC to VPC traffic
    - Outbound to internet
    - Inbound from internet
    - To / from Direct Connect & Site-to-Site VPN

![AWS Network Firewall](../images/network/NetworkFirewall.png)


- AWS Firewall Manager
- Manage security rules in all accounts of an AWS Organization
- Security policy: common set of security rules
    - VPC Security Groups for EC2, Application Load Balancer, etc…
    - WAF rules
    - AWS Shield Advanced
    - AWS Network Firewall
- Rules are applied to new resources as they are created (good for compliance) across all and future accounts in your Organization


**Cheat Sheets**

https://tutorialsdojo.com/aws-network-firewall/

**References**

https://aws.amazon.com/network-firewall/


**Videos**

https://www.youtube.com/results?search_query=Amazon+Network+Firewall

https://www.youtube.com/watch?v=WNFknf9zyZg



***************************************************************************************************
## <a id="section-98"></a> **98 - Networks Comments**

**Networks Comments**

- **VPC** – Virtual Private Cloud
- **Subnets** – Tied to an AZ, network partition of the VPC
- **Internet Gateway** – at the VPC level, provide Internet Access
- **NAT Gateway / Instances** – give internet access to private subnets
- **NACL** – Stateless, subnet rules for inbound and outbound
- **Security Groups** – Stateful, operate at the EC2 instance level or ENI
- **VPC Peering** – Connect two VPC with non overlapping IP ranges, nontransitive
- **Elastic IP** –fixed public IPv4, ongoing cost if not in-use
- **VPC Endpoints** – Provide private access to AWS Services within VPC
- **PrivateLink** – Privately connect to a service in a 3rd party VPC
- **VPC Flow Logs** – network traffic logs
- **Site to Site VPN** – VPN over public internet between on-premises DC and AWS
- **Client VPN** – OpenVPN connection from your computer into your VPC
- **Direct Connect** – direct private connection to AWS
- **Transit Gateway** – Connect thousands of VPC and on-premises networks together


***************************************************************************************************
## <a id="section-99"></a> **99 - Additional resources**

![Additional resources](../images/extra/images.jpeg)


[Operational Excellence Pillar](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/welcome.html)

[AWS CloudFormation templates in GitHub](https://github.com/aws-cloudformation/aws-cloudformation-templates)

[CloudFormation templates for AWS services](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)

[AWS Network Firewall CloudFormation template](https://docs.aws.amazon.com/solutions/latest/centralized-network-inspection-on-aws/aws-cloudformation-template.html)

[AWS Solutions Implementations](https://aws.amazon.com/solutions/?nc1=h_ls)

[Scaling VPN throughput using AWS Transit Gateway](https://aws.amazon.com/pt/blogs/networking-and-content-delivery/scaling-vpn-throughput-using-aws-transit-gateway/)

[Reliability Pillar](https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/welcome.html)

[Plan your Network Topology](https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/plan-your-network-topology.html)

[Performance Efficiency Pillar](https://docs.aws.amazon.com/wellarchitected/latest/performance-efficiency-pillar/welcome.html)

[Amazon VPC connectivity options](https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/network-to-amazon-vpc-connectivity-options.html)

[Amazon VPC-to-Amazon VPC connectivity options](https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/amazon-vpc-to-amazon-vpc-connectivity-options.html)

[Architecture](https://docs.aws.amazon.com/vpc/latest/userguide/how-it-works.html)

[Security Pillar](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/welcome.html)

[AWS Compliance Resources](https://aws.amazon.com/compliance/resources/) – This collection of workbooks and guides might apply to your industry and location.

[Evaluating Resources with Rules in the AWS Config Developer Guide](https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config.html) – The AWS Config service assesses how well your resource configurations comply with internal practices, industry guidelines, and regulations.

[AWS Security Hub](https://docs.aws.amazon.com/securityhub/latest/userguide/what-is-securityhub.html) – This AWS service provides a comprehensive view of your security state within AWS that helps you check your compliance with security industry standards and best practices.

[AWS Audit Manager](https://docs.aws.amazon.com/audit-manager/latest/userguide/what-is.html) – This AWS service helps you continuously audit your AWS usage to simplify how you manage risk and compliance with regulations and industry standards.

[AWS Direct Connect Service Level Agreement](https://aws.amazon.com/directconnect/sla/)

[AWS Direct Connect Troubleshooting](https://docs.aws.amazon.com/directconnect/latest/UserGuide/Troubleshooting.html)

[AWS Direct Connect Connections configuration](https://docs.aws.amazon.com/directconnect/latest/UserGuide/create-connection.html)

[Example routing options](https://docs.aws.amazon.com/vpc/latest/userguide/route-table-options.html#route-tables-vgw)


[Cost Optimization](https://wa.aws.amazon.com/wellarchitected/2020-07-02T19-33-23/wat.pillar.costOptimization.en.html)

[Cost Optimization Pillar - AWS Well Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/cost-optimization-pillar/welcome.html)

[AWS Pricing Calculator](https://calculator.aws/#/)

[AWS Network Firewall CloudFormation template](https://docs.aws.amazon.com/solutions/latest/centralized-network-inspection-on-aws/aws-cloudformation-template.html)