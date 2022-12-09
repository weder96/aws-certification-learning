<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Module 98: Common‌ ‌Exam‌ ‌Scenarios‌ ‌

## Contents
1. <a href="#section-1"> Common‌ ‌Exam‌ ‌Scenarios‌ - AWS‌ ‌CERTIFIED‌ ‌CLOUD‌ ‌PRACTITIONER</a>
2. <a href="#section-2"> Common‌ ‌Exam‌ ‌Scenarios‌ - AWS‌ ‌CERTIFIED‌ ‌SOLUTIONS‌ ‌ARCHITECT‌ ‌ASSOCIATE</a>



##################################################################################################################################
## <a id="section-01" ></a> **01 - Common‌ ‌Exam‌ ‌Scenarios‌  - AWS‌ ‌CERTIFIED‌ ‌CLOUD‌ ‌PRACTITIONER**

### **Domain‌ 1 :‌ Cloud‌ Concepts‌**

|Scenario                                   | Solution‌                          |
|-------------------------------------------|-----------------------------------|
|A‌ ‌key‌ ‌financial‌ ‌benefit‌ ‌of‌ ‌migrating‌ ‌systems‌ ‌hosted‌‌ on‌ ‌your‌ ‌on-premises‌ ‌data‌ ‌center‌ ‌to‌ ‌AWS | ‌1. ‌Replaces‌ ‌upfront‌ ‌capital‌ expenses‌ ‌(CAPEX)‌ ‌with‌ ‌low‌‌ variable‌ ‌operational‌ ‌expenses‌ ‌(OPEX).‌ <br/>‌ 2. ‌Reduce‌ ‌the‌ ‌Total‌ ‌Cost‌ ‌of‌ ‌Ownership‌ ‌(TCO)‌ ‌|
|Cloud‌ ‌architectures‌ ‌design‌ ‌principle‌ ‌in‌ ‌AWS | 1. Design‌ ‌for‌ ‌failure.‌ ‌<br/>‌ 2. Decouple‌ ‌your‌ ‌components‌ ‌<br/>‌ 3. Implement‌ ‌elasticity‌ ‌<br/>‌ 4. Think‌ ‌parallel‌ ‌|
|A‌ ‌cloud‌ ‌architecture‌ ‌for‌ ‌mission-critical‌ ‌workloads‌ ‌in‌‌ AWS‌ ‌which‌ ‌must‌ ‌be‌ ‌highly-available. | Use‌ ‌multiple‌ ‌Availability‌ ‌Zones‌ ‌|
|A ‌change‌ ‌or‌ ‌a‌ ‌failure‌ ‌in‌ ‌one‌ ‌component‌ ‌should‌ ‌not‌‌ cascade‌ ‌to‌ ‌other‌ ‌components.‌| Loose‌ ‌coupling‌ ‌|
|You‌ ‌need‌ ‌to‌ ‌enable‌ ‌your‌ ‌Amazon‌ ‌EC2‌ ‌instances‌ ‌in‌ ‌the‌‌ public‌ ‌subnet‌ ‌to‌ ‌connect‌ ‌to‌ ‌the‌ ‌public‌ ‌Internet. | Internet‌ ‌Gateway‌ |
|You‌ ‌need‌ ‌to‌ ‌enable‌ ‌your‌ ‌EC2‌ ‌instances‌ ‌in‌ ‌the‌ ‌private‌‌ subnet‌ ‌to‌ ‌connect‌ ‌to‌ ‌the‌ ‌public‌ ‌Internet.‌ | NAT‌ ‌Gateway‌ |



### **Domain‌ 2:‌ Security‌ and‌ Compliance‌ ‌**

|Scenario                                                                        | Solution‌                          |
|--------------------------------------------------------------------------------|-----------------------------------|
|A‌ ‌security‌ ‌management‌ ‌tool‌ ‌to‌ ‌configure‌ ‌your‌ ‌AWS‌‌ WAF‌ ‌rules‌ ‌across‌ ‌your‌ ‌accounts.‌|AWS‌ ‌Firewall‌ ‌Manager‌ ‌|
|A‌ ‌company‌ ‌needs‌ ‌to‌ ‌download‌ ‌the‌‌ compliance-related‌ ‌documents‌ ‌in‌ ‌AWS‌ ‌such‌ ‌as‌‌ Service‌ ‌Organization‌ ‌Controls‌ ‌(SOC)‌ ‌reports‌ | AWS‌ ‌Artifact‌ ‌|
|Improve‌ ‌the‌ ‌security‌ ‌of‌ ‌IAM‌ ‌users. | 1. Enable‌ ‌Multi-Factor‌ ‌Authentication‌ ‌(MFA)‌ ‌<br/> 2. ‌Configure‌ ‌a‌ ‌strong‌ ‌password‌ ‌policy‌|
|An‌ ‌IAM‌ ‌identity‌ ‌that‌ ‌uses‌ ‌access‌ ‌keys‌ ‌to‌ ‌manage‌‌ cloud‌ ‌resources‌ ‌via‌ ‌AWS‌ ‌CLI.‌ | IAM‌ ‌User‌ |
|Grant‌ ‌temporary‌ ‌access‌ ‌to‌ ‌your‌ ‌AWS‌ ‌resources.‌ |IAM‌ ‌Role‌|
|Apply‌ ‌and‌ ‌easily‌ ‌manage‌ ‌the‌ ‌common‌ ‌access‌‌ permissions‌ ‌to‌ ‌a‌ ‌large‌ ‌number‌ ‌of‌ ‌IAM‌ ‌users‌ ‌in‌ ‌AWS |IAM‌ ‌Group‌ |
|Grant‌ ‌the‌ ‌required‌ ‌permissions‌ ‌to‌ ‌access‌ ‌your‌‌ Amazon‌ ‌S3‌ ‌resources. | 1. Bucket‌ ‌Policy‌ ‌ <br/> 2. User‌ ‌Policy‌| ‌
|You‌ ‌must‌ ‌provide‌ ‌temporary‌ ‌AWS‌ ‌credentials‌ ‌for‌‌ users‌ ‌who‌ ‌have‌ ‌authenticated‌ ‌via‌ ‌their‌ ‌social‌ ‌media‌‌ logins‌ ‌as‌ ‌well‌ ‌as‌ ‌for‌ ‌guest‌ ‌users‌ ‌who‌ ‌do‌ ‌not‌ ‌require‌‌ any‌ ‌authentication.‌ | Amazon‌ ‌Cognito‌ ‌Identity‌ ‌Pool‌ ‌|
|A‌ ‌startup‌ ‌needs‌ ‌to‌ ‌evaluate‌ ‌the‌ ‌newly‌ ‌created‌ ‌IAM‌‌ policies.‌ |IAM‌ ‌Policy‌ ‌Simulator‌|
|A‌ ‌service‌ ‌that‌ ‌discovers,‌ ‌classifies,‌ ‌and‌ ‌protects‌‌ sensitive‌ ‌data‌ ‌such‌ ‌as‌ ‌personally‌ ‌identifiable‌‌ information‌ ‌(PII)‌ ‌or‌ ‌intellectual‌ ‌property. | Amazon‌ ‌Macie‌ ‌|
|A‌ ‌threat‌ ‌detection‌ ‌service‌ ‌that‌ ‌continuously‌ ‌monitors‌‌ ‌for‌ ‌malicious‌ ‌activity‌ ‌to‌ ‌protect‌ ‌your‌ ‌AWS‌ ‌account.‌|  Amazon‌ ‌GuardDuty‌ |
|Prevent‌ ‌unauthorized‌ ‌deletion‌ ‌of‌ ‌Amazon‌ ‌S3‌ ‌objects.‌ ‌ | Enable‌ ‌Multi-Factor‌ ‌Authentication‌ ‌(MFA)‌|
| ‌A‌ ‌company‌ ‌needs‌ ‌to‌ ‌control‌ ‌the‌ ‌traffic‌ ‌going‌ ‌in‌ ‌and‌‌ out‌ ‌of‌ ‌their‌ ‌VPC‌ ‌subnets.‌ ‌ | Network‌ ‌Access‌ ‌Control‌ ‌List‌ ‌(NACL)‌|
|What‌ ‌acts‌ ‌as‌ ‌a‌ ‌virtual‌ ‌firewall‌ ‌in‌ ‌AWS‌ ‌that‌ ‌controls‌‌ the‌ ‌traffic‌ ‌at‌ ‌the‌ ‌EC2‌ ‌instance‌ ‌level?‌ ‌ | Security‌ ‌Group‌ ‌ |
|Set‌ ‌up‌ ‌an‌ ‌automated‌ ‌security‌ ‌assessment‌ ‌service‌ ‌to‌‌ improve‌ ‌the‌ ‌security‌ ‌and‌ ‌compliance‌ ‌of‌ ‌your‌‌ applications.‌ ‌ |Amazon‌  Inspector‌ | ‌


### **Domain‌ 3:‌ Technology‌ ‌**

|Scenario                                                                        | Solution‌                          |
|--------------------------------------------------------------------------------|-----------------------------------|
|A‌ ‌company‌ ‌needs‌ ‌to‌ ‌use‌ ‌the‌ ‌AWS‌ ‌global‌ ‌network‌ ‌to‌‌ improve‌ ‌availability‌ ‌of‌ ‌deployed‌ ‌applications‌ ‌on‌ ‌AWS‌‌ using‌ ‌an‌ ‌anycast‌ ‌static‌ ‌IP‌ ‌address.‌ ‌ |AWS‌ ‌Global‌ ‌Accelerator‌ ‌|
|You‌ ‌need‌ ‌to‌ ‌securely‌ ‌transfer‌ ‌hundreds‌ ‌of‌ ‌petabytes‌‌ of‌ ‌data‌ ‌into‌ ‌and‌ ‌out‌ ‌of‌ ‌the‌ ‌AWS‌ ‌Cloud.‌ ‌ | AWS‌ ‌Snowball‌ ‌Edge‌ | ‌
|A‌ ‌type‌ ‌of‌ ‌an‌ ‌EC2‌ ‌instance‌ ‌that‌ ‌allows‌ ‌you‌ ‌to‌ ‌use‌ ‌your‌‌ existing‌ ‌server-bound‌ ‌software‌ ‌licenses.‌ | Dedicated‌ ‌Host‌ |
|A‌ ‌service‌ ‌that‌ ‌allows‌ ‌you‌ ‌to‌ ‌continuously‌ ‌monitor‌ ‌and‌‌ ‌ log‌ ‌account‌ ‌activities‌ ‌such‌ ‌as‌ ‌the‌ ‌user‌ ‌actions‌ ‌made‌‌ from‌ ‌the‌ ‌AWS‌ ‌Management‌ ‌Console‌ ‌and‌ ‌AWS‌ ‌SDKs. | AWS‌ ‌CloudTrail‌ |
|A‌ ‌highly‌ ‌available‌ ‌and‌ ‌scalable‌ ‌cloud‌ ‌DNS‌ ‌web‌‌ service‌ ‌in‌ ‌AWS.‌ ‌| Amazon‌ ‌Route‌ ‌53‌ ‌|
|Store‌ ‌the‌ ‌results‌ ‌of‌ ‌I/O-intensive‌ ‌SQL‌ ‌database‌‌ queries‌ ‌to‌ ‌improve‌ ‌the‌ ‌application‌ ‌performance.‌ | Amazon‌ ‌ElastiCache‌ |
|A‌ ‌combination‌ ‌of‌ ‌AWS‌ ‌services‌ ‌that‌ ‌allows‌ ‌you‌ ‌to‌‌ serve‌ ‌the‌ ‌static‌ ‌files‌ ‌with‌ ‌lowest‌ ‌possible‌ ‌latency. | 1. Amazon‌ ‌S3‌ ‌<br/> 2. Amazon‌ ‌CloudFront‌| ‌
|Automatically‌ ‌scale‌ ‌the‌ ‌capacity‌ ‌of‌ ‌an‌ ‌AWS‌ ‌cloud‌‌ resource‌ ‌based‌ ‌on‌ ‌the‌ ‌incoming‌ ‌traffic‌ ‌to‌ ‌improve‌‌ availability‌ ‌and‌ ‌reduce‌ ‌failures‌ | AWS‌ ‌Auto‌ ‌Scaling‌ |
|A‌ ‌company‌ ‌needs‌ ‌to‌ ‌migrate‌ ‌an‌ ‌on-premises‌ ‌MySQL‌‌ database‌ ‌to‌ ‌Amazon‌ ‌RDS.‌ |  ‌AWS‌ ‌Database‌ ‌Migration‌ ‌Service‌ ‌(AWS‌ ‌DMS)‌ ‌|
|Automatically‌ ‌transfer‌ ‌your‌ ‌infrequently‌ ‌accessed‌‌ data‌ ‌in‌ ‌your‌ ‌S3‌ ‌bucket‌ ‌to‌ ‌a‌ ‌more‌ ‌cost-effective‌‌ storage‌ ‌class.‌ |S3‌ ‌Lifecycle‌ ‌Policy‌|
| ‌You‌ ‌need‌ ‌to‌ ‌upload‌ ‌a‌ ‌single‌ ‌object‌ ‌as‌ ‌a‌ ‌set‌ ‌of‌ ‌parts‌ ‌to‌‌ Use‌ ‌ improve‌ ‌throughput‌ ‌and‌ ‌have‌ ‌a‌ ‌quicker‌ ‌recovery‌ ‌from‌‌ any‌ ‌network‌ ‌issues.‌| ‌Multipart‌ ‌Upload‌ ‌API‌ |
|A‌ ‌company‌ ‌needs‌ ‌to‌ ‌establish‌ ‌a‌ ‌dedicated‌‌ connection‌ ‌between‌ ‌their‌ ‌on-premises‌ ‌network‌ ‌and‌‌ their‌ ‌AWS‌ ‌VPC.‌ | AWS‌ ‌Direct‌ ‌Connect‌|
|A‌ ‌Machine‌ ‌Learning‌ ‌service‌ ‌that‌ ‌allows‌ ‌you‌ ‌to‌ ‌add‌ ‌a‌‌ visual‌ ‌analysis‌ ‌feature‌ ‌to‌ ‌your‌ ‌applications.‌ |Amazon‌ ‌Rekognition‌|
|A‌ ‌source‌ ‌control‌ ‌service‌ ‌that‌ ‌allows‌ ‌you‌ ‌to‌ ‌host‌‌ Git-based‌ ‌repositories.‌ | ‌AWS‌ ‌CodeCommit‌ ‌|
|A‌ ‌service‌ ‌that‌ ‌can‌ ‌trace‌ ‌user‌ ‌requests‌ ‌in‌ ‌your‌‌ application | AWS‌ ‌X-Ray‌ ‌|
|A‌ ‌company‌ ‌needs‌ ‌to‌ ‌retrieve‌ ‌the‌ ‌instance‌ ‌ID,‌ ‌public‌‌ keys,‌ ‌and‌ ‌public‌ ‌IP‌ ‌address‌ ‌of‌ ‌their‌ ‌EC2‌ ‌instance.‌ | Instance‌ ‌metadata‌ |
|You‌ ‌need‌ ‌to‌ ‌speed‌ ‌up‌ ‌the‌ ‌content‌ ‌delivery‌ ‌of‌ ‌static‌‌ assets‌ ‌to‌ ‌your‌ ‌customers‌ ‌around‌ ‌the‌ ‌globe‌ | Amazon‌ ‌CloudFront‌ ‌|
|Create‌ ‌and‌ ‌deploy‌ ‌infrastructure-as-code‌ ‌templates‌ | AWS‌ ‌CloudFormation‌|
|You‌ ‌have‌ ‌to‌ ‌encrypt‌ ‌the‌ ‌log‌ ‌data‌ ‌that‌ ‌is‌ ‌stored‌ ‌and‌‌ managed‌ ‌by‌ ‌AWS‌ ‌CloudTrail.‌ | AWS‌ ‌Key‌ ‌Management‌ ‌Service‌ ‌(AWS‌ ‌KMS)‌ |
|A‌ ‌database‌ ‌service‌ ‌that‌ ‌can‌ ‌be‌ ‌used‌ ‌to‌ ‌store‌ ‌JSON‌‌ documents.‌ | Amazon‌ ‌DynamoDB‌ |



### **Domain‌ 4:‌ Billing‌ and‌ Pricing‌**

|Scenario                                                                        | Solution‌                          |
|--------------------------------------------------------------------------------|-----------------------------------|
|A‌ ‌designated‌ ‌technical‌ ‌point‌ ‌of‌ ‌contact‌ ‌that‌ ‌will‌‌ maintain‌ ‌an‌ ‌operationally‌ ‌healthy‌ ‌AWS‌ ‌environment. | Technical‌ ‌Account‌ ‌Manage(TAM)‌|
|A‌ ‌tool‌ ‌that‌ ‌inspects‌ ‌your‌ ‌AWS‌ ‌environment‌ ‌and‌‌ makes‌ ‌recommendations‌ ‌that‌ ‌follows‌ ‌AWS‌ ‌best‌‌ practices.‌| ‌ AWS‌ ‌Trusted‌ ‌Advisor‌ ‌|
|A‌ ‌startup‌ ‌needs‌ ‌to‌ ‌estimate‌ ‌the‌ ‌costs‌ ‌of‌ ‌moving‌ ‌their‌‌ application‌ ‌to‌ ‌AWS. |AWS‌ ‌Pricing‌‌ Calculator‌ ‌|
|Set‌ ‌coverage‌ ‌targets‌ ‌and‌ ‌receive‌ ‌alerts‌ ‌when‌ ‌your‌‌ utilization‌ ‌drops.‌ ‌ |AWS‌ ‌Budgets‌| ‌
|A‌ ‌type‌ ‌of‌ ‌Reserved‌ ‌Instance‌ ‌that‌ ‌allows‌ ‌you‌ ‌to‌‌ change‌ ‌its‌ ‌instance‌ ‌family,‌ ‌instance‌ ‌type,‌ ‌platform,‌‌ scope,‌ ‌or‌ ‌tenancy.‌ | Convertible‌ ‌RI‌ ‌|
|Take‌ ‌advantage‌ ‌of‌ ‌unused‌ ‌EC2‌ ‌capacity‌ ‌in‌ ‌the‌ ‌AWS‌‌ Cloud‌ ‌and‌ ‌provides‌ ‌up‌ ‌to‌ ‌90%‌ ‌discount.‌ ‌| Spot‌ ‌Instance‌| ‌
|You‌ ‌need‌ ‌to‌ ‌centrally‌ ‌manage‌ ‌policies‌ ‌and‌‌ consolidate‌ ‌billing‌ ‌across‌ ‌multiple‌ ‌AWS‌ ‌accounts.‌ ‌ |AWS‌ ‌Organizations‌| ‌
|The‌ ‌most‌ ‌cost-efficient‌ ‌storage‌ ‌option‌ ‌for‌ ‌retaining‌‌ database‌ ‌backups‌ ‌that‌ ‌allows‌ ‌occasional‌ ‌data‌‌ retrieval‌ ‌in‌ ‌minutes.‌ ‌| Amazon‌ ‌Glacier‌ ‌|
|Forecast‌ ‌future‌ ‌costs‌ ‌and‌ ‌usage‌ ‌of‌ ‌your‌ ‌AWS‌‌ resources‌ ‌based‌ ‌on‌ ‌your‌ ‌past‌ ‌consumption.‌ ‌ |AWS‌ ‌Cost‌ ‌Explorer‌| ‌
|Categorize‌ ‌and‌ ‌track‌ ‌AWS‌ ‌costs‌ ‌on‌ ‌a‌ ‌detailed‌ ‌level.‌ ‌ |Cost‌ ‌allocation‌ ‌tags‌| ‌
|A‌ ‌company‌ ‌launched‌ ‌a‌ ‌new‌ ‌VPC‌ ‌which‌ ‌is‌ ‌way‌ ‌beyond‌‌ the‌ ‌default‌ ‌service‌ ‌limit.‌ |Request‌ ‌a‌ ‌service‌ ‌limit‌ ‌increase‌ ‌in‌ ‌AWS‌ ‌Support‌ ‌Center‌| ‌
|The‌ ‌most‌ ‌cost-effective‌ ‌option‌ ‌when‌ ‌you‌ ‌purchase‌ ‌a‌‌ Reserved‌ ‌Instance‌ ‌for‌ ‌a‌ ‌1-year‌ ‌term.‌ ‌|All‌ ‌Upfront‌| ‌
|You‌ ‌have‌ ‌to‌ ‌combine‌ ‌usage‌ ‌volume‌ ‌discounts‌ ‌of‌ ‌your‌‌  ‌ multiple‌ ‌AWS‌ ‌accounts.‌  |Consolidated‌ ‌Billing‌| ‌
|Sell‌ ‌your‌ ‌catalog‌ ‌of‌ ‌custom‌ ‌AMIs‌ ‌in‌ ‌AWS‌ ‌ |AWS‌ ‌Marketplace‌| ‌

<br/><br/>
##################################################################################################################################
## <a id="section-02" ></a> **02 - Common‌ ‌Exam‌ ‌Scenarios‌  - AWS‌ ‌CERTIFIED‌ ‌SOLUTIONS‌ ‌ARCHITECT‌ ‌ASSOCIATE‌**

### **Domain‌ 1:‌ Design‌ Resilient‌ Architectures‌**

|Scenario                                   | Solution‌                          |
|-------------------------------------------|-----------------------------------|
|Set‌ ‌up‌ ‌asynchronous‌ ‌data‌ ‌replication‌ ‌to‌ ‌another‌ ‌RDS‌‌ DB‌ ‌instance‌ ‌hosted‌ ‌in‌ ‌another‌ AWS‌ ‌Region‌ | Create‌ ‌a‌ ‌Read‌ ‌Replica‌ ‌|
|A‌ ‌parallel‌ ‌file‌ ‌system‌ ‌for‌ ‌“hot”‌ ‌(frequently‌ ‌accessed)‌‌ data‌ ‌                                 | Amazon‌ ‌FSx‌ ‌For‌ ‌Lustre‌ |
|Implement‌ ‌synchronous‌ ‌data‌ ‌replication‌ ‌across‌‌ Availability‌ ‌Zones‌ ‌with‌ ‌automatic‌ ‌failover‌ ‌in‌ ‌Amazon‌‌ RDS.‌ | Enable‌ ‌Multi-AZ‌ deployment‌ ‌in‌ ‌Amazon‌ ‌RDS.‌|
|Needs‌ ‌a‌ ‌storage‌ ‌service‌ ‌to‌ ‌host‌ ‌“cold”‌ ‌(infrequently‌‌ accessed)‌ ‌data‌ | Amazon‌ ‌S3‌ ‌Glacier‌ ‌|
|Set‌ ‌up‌ ‌a‌ ‌relational‌ ‌database‌ ‌and‌ ‌a‌ ‌disaster‌ ‌recovery‌‌ plan‌ ‌with‌ ‌an‌ ‌RPO‌ ‌of‌ ‌1‌ ‌second‌ ‌and‌ ‌RTO‌ ‌of‌ ‌less‌ ‌than‌ ‌1‌‌ minute.‌ | Use‌ ‌Amazon‌ ‌Aurora‌ ‌Global‌ ‌Database.‌|
|Monitor‌ ‌database‌ ‌metrics‌ ‌and‌ ‌send‌ ‌email‌‌ notifications‌ ‌if‌ ‌a‌ ‌specific‌ ‌threshold‌ ‌has‌ ‌been‌‌ breached. | Create‌ ‌an‌ ‌SNS‌ ‌topic‌ ‌and‌ ‌add‌ ‌the‌ ‌topic‌ ‌in‌ ‌the‌‌
CloudWatch‌ ‌alarm.‌|
|Set‌ ‌up‌ ‌a‌ ‌DNS‌ ‌failover‌ ‌to‌ ‌a‌ ‌static‌ ‌website.‌ | Use‌ ‌Route‌ ‌53‌ ‌with‌ ‌the‌ ‌failover‌ ‌option‌ ‌to‌ ‌a‌ ‌static‌ ‌S3‌‌
website‌ ‌bucket‌ ‌or‌ ‌CloudFront‌ ‌distribution.‌|
|Implement‌ ‌an‌ ‌automated‌ ‌backup‌ ‌for‌ ‌all‌ ‌the‌ ‌EBS‌‌ Volumes.‌ |Use‌ ‌Amazon‌ ‌Data‌ ‌Lifecycle‌ ‌Manager‌ ‌to‌ ‌automate‌‌ the‌ ‌creation‌ ‌of‌ ‌EBS‌ ‌snapshots.|
|Monitor‌ ‌the‌ ‌available‌ ‌swap‌ ‌space‌ ‌of‌ ‌your‌ ‌EC2‌‌ instances‌ ‌ | Install‌ ‌the‌ ‌CloudWatch‌ ‌agent‌ ‌and‌ ‌monitor‌ ‌the‌‌ SwapUtilizationmetric.‌ |
|Implement‌ ‌a‌ ‌90-day‌ ‌backup‌ ‌retention‌ ‌policy‌ ‌on‌‌ Amazon‌ ‌Aurora.‌ | Use‌ ‌AWS‌ ‌Backup‌  |



------------------------------------------------------------------------------------------------------------------------
### **Domain‌ 2 :‌ Design‌ High-Performing‌ Architectures‌**


|Scenario                                   | Solution‌                          |
|-------------------------------------------|-----------------------------------|
|Implement‌ ‌a‌ ‌fanout‌ ‌messaging.‌              |Create‌ ‌an‌ ‌SNS‌ ‌topic‌ ‌with‌ ‌a‌ ‌message‌ ‌filtering‌ ‌policy‌‌ and‌ ‌configure‌ ‌multiple‌ ‌SQS‌ ‌queues‌ ‌to‌ ‌subscribe‌ ‌to‌‌ the‌ ‌topic.‌ ‌|
|A‌ ‌database‌ ‌that‌ ‌has‌ ‌a‌ ‌read‌ ‌replication‌ ‌latency‌ ‌of‌ ‌less‌‌ than‌ ‌1‌ ‌second. | Use‌ ‌Amazon‌ ‌Aurora‌ ‌with‌ ‌cross-region‌ ‌replicas.|
|A‌ ‌specific‌ ‌type‌ ‌of‌ ‌Elastic‌ ‌Load‌ ‌Balancer‌ ‌that‌ ‌uses‌ ‌UDP‌‌  ‌ as‌ ‌the‌ ‌protocol‌ ‌for‌ ‌communication‌ ‌between‌ ‌clients‌‌ and‌ ‌thousands‌ ‌of‌ ‌game‌ ‌servers‌ ‌around‌ ‌the‌ ‌world.| Use‌ ‌Network‌ ‌Load‌ ‌Balancer‌ ‌for‌ ‌TCP/UDP‌ ‌protocols.‌ |
|Monitor‌ ‌the‌ ‌memory‌ ‌and‌ ‌disk‌ ‌space‌ ‌utilization‌ ‌of‌ ‌an‌‌ EC2‌ ‌instance.‌ | Install‌ ‌Amazon‌ ‌CloudWatch‌ ‌agent‌ ‌on‌ ‌the‌ ‌instance |
|Retrieve‌ ‌a‌ ‌subset‌ ‌of‌ ‌data‌ ‌from‌ ‌a‌ ‌large‌ ‌CSV‌ ‌file‌ ‌stored‌‌ in‌ ‌the‌ ‌S3‌ ‌bucket. |Perform‌ ‌an‌ ‌S3‌ ‌Select‌ ‌operation‌ ‌based‌ ‌on‌ ‌the‌‌ bucket's‌ ‌name‌ ‌and‌ ‌object's‌ ‌key.‌ ‌|
|Upload‌ ‌1‌ ‌TB‌ ‌file‌ ‌to‌ ‌an‌ ‌S3‌ ‌bucket. | Use‌ ‌Amazon‌ ‌S3‌ ‌multipart‌ ‌upload‌ ‌API‌ ‌to‌ ‌upload‌ ‌large‌‌ objects‌ ‌in‌ ‌parts.‌ |
|Improve‌ ‌the‌ ‌performance‌ ‌of‌ ‌the‌ ‌application‌ ‌by‌‌ reducing‌ ‌the‌ ‌response‌ ‌times‌ ‌from‌ ‌milliseconds‌ ‌to‌ microseconds.‌ | Use‌ ‌Amazon‌ ‌DynamoDB‌ ‌Accelerator‌ ‌(DAX)‌ ‌|
|Retrieve‌ ‌the‌ ‌instance‌ ‌ID,‌ ‌public‌ ‌keys,‌ ‌and‌ ‌public‌ ‌IP‌‌ address‌ ‌of‌ ‌an‌ ‌EC2‌ ‌instance.‌ | Access‌ ‌the‌ ‌url:‌‌ http://169.254.169.254/latest/meta-data/‌‌ ‌using‌ ‌the‌‌ EC2‌ ‌instance.‌|
|Route‌ ‌the‌ ‌internet‌ ‌traffic‌ ‌to‌ ‌the‌ ‌resources‌ ‌based‌ ‌on‌ ‌the‌‌  ‌location‌ ‌of‌ ‌the‌ ‌user.‌ | Use‌ ‌Route‌ ‌53‌ ‌Geolocation‌ ‌Routing‌ ‌policy.|




------------------------------------------------------------------------------------------------------------------------
### **Domain‌ 3 :‌ Design‌ Secure‌ Applications‌ and‌ Architectures‌**


|Scenario                                   | Solution‌                          |
|-------------------------------------------|-----------------------------------|
|Encrypt‌ ‌EBS‌ ‌volumes‌ ‌restored‌ ‌from‌ ‌the‌ ‌unencrypted‌‌ EBS‌ ‌snapshots | Copy‌ ‌the‌ ‌snapshot‌ ‌and‌ ‌enable‌ ‌encryption‌ ‌with‌ ‌a‌‌
new‌ ‌symmetric‌ ‌CMK‌ ‌while‌ ‌creating‌ ‌an‌ ‌EBS‌ ‌volume‌‌ using‌ ‌the‌ ‌snapshot.‌ |
|Limit‌ ‌the‌ ‌maximum‌ ‌number‌ ‌of‌ ‌requests‌ ‌from‌ ‌a‌ ‌single‌‌ IP‌ ‌address. | Create‌ ‌a‌ ‌rate-based‌ ‌rule‌ ‌in‌ ‌AWS‌ ‌WAF‌ ‌and‌ ‌set‌ ‌the‌‌ rate‌ limit.|
|Grant‌ ‌the‌ ‌bucket‌ ‌owner‌ ‌full‌ ‌access‌ ‌to‌ ‌all‌ ‌uploaded‌‌ objects‌ ‌in‌ ‌the‌ ‌S3‌ ‌bucket.‌ |Create‌ ‌a‌ ‌bucket‌ ‌policy‌ ‌that‌ ‌requires‌ ‌users‌  to‌ ‌set‌ ‌the‌‌ object's‌ ‌ACL‌ ‌to‌ ‌bucket-owner-full-control.‌|
|Protect‌ ‌objects‌ ‌in‌ ‌the‌ ‌S3‌ ‌bucket‌ ‌from‌ ‌accidental‌‌ deletion‌ ‌or‌ ‌overwrite.‌ | Enable‌ ‌versioning‌ ‌and‌ ‌MFA‌ ‌delete.‌|
|Access‌ ‌resources‌ ‌on‌ ‌both‌ ‌on-premises‌ ‌and‌ ‌AWS‌‌ using‌ ‌on-premises‌ ‌credentials‌ ‌that‌ ‌are‌ ‌stored‌ ‌in‌ ‌Active‌‌ Directory.‌ ‌ | Set‌ ‌up‌ ‌SAML‌ ‌2.0-Based‌ ‌Federation‌ ‌by‌ ‌using‌ ‌a‌‌ Microsoft‌ ‌Active‌ ‌Directory‌ ‌Federation‌ ‌Service. |
|Secure‌ ‌the‌ ‌sensitive‌ ‌data‌ ‌stored‌ ‌in‌ ‌EBS‌ ‌volumes‌ | Enable‌ ‌EBS‌ ‌Encryption‌ |
|Ensure‌ ‌that‌ ‌the‌ ‌data-in-transit‌ ‌and‌ ‌data-at-rest‌ ‌of‌ ‌the‌‌ Amazon‌ ‌S3‌ ‌bucket‌ ‌is‌ ‌always‌ ‌encrypted‌ | Enable‌ ‌Amazon‌ ‌S3‌ ‌Server-Side‌  or‌ ‌use‌ ‌Client-Side‌‌ Encryption‌ |
|Secure‌ ‌the‌ ‌web‌ ‌application‌ ‌by‌ ‌allowing‌ ‌multiple‌‌ domains‌ ‌to‌ ‌serve‌ ‌SSL‌ ‌traffic‌ ‌over‌ ‌the‌ ‌same‌ ‌IP‌‌ address.‌ | Use‌ ‌AWS‌  Certificate‌ ‌Manager‌ ‌to‌ ‌generate‌ ‌an‌ ‌SSL‌‌ certificate.‌ ‌Associate‌ ‌the‌ ‌certificate‌ ‌to‌ ‌the‌‌ CloudFront‌ ‌distribution‌ ‌and‌ ‌enable‌ ‌Server‌ ‌Name‌‌ Indication‌ ‌(SNI).‌ ‌|
|Control‌ ‌the‌ ‌access‌ ‌for‌ ‌several‌ ‌S3‌ ‌buckets‌ ‌by‌ ‌using‌ ‌a‌‌ gateway‌ ‌endpoint‌ ‌to‌ ‌allow‌ ‌access‌ ‌to‌ ‌trusted‌ ‌buckets | Create‌ ‌an‌ ‌endpoint‌ ‌policy‌ ‌for‌ ‌trusted‌ ‌S3‌ ‌buckets.‌ ‌|
|Enforce‌ ‌strict‌ ‌compliance‌ ‌by‌ ‌tracking‌ ‌all‌ ‌the‌‌ configuration‌ ‌changes‌ ‌made‌ ‌to‌ ‌any‌ ‌AWS‌ ‌services. | Set‌ ‌up‌ ‌a‌ ‌rule‌ ‌in‌ ‌AWS‌  Config‌ ‌to‌ ‌identify‌ ‌compliant‌‌ and‌ ‌non-compliant‌ ‌services.‌|
|Provide‌ ‌short-lived‌ ‌access‌ ‌tokens‌ ‌that‌ ‌acts‌ ‌as‌‌ temporary‌ ‌security‌ ‌credentials‌ ‌to‌ ‌allow‌ ‌access‌ ‌to‌ ‌AWS‌‌ resources.‌ | Use‌ ‌AWS‌ ‌Security‌ ‌Token‌ ‌Service‌ ‌|
|Encrypt‌ ‌and‌ ‌rotate‌ ‌all‌ ‌the‌ ‌database‌ ‌credentials,‌ ‌API‌‌ keys,‌ ‌and‌ ‌other‌ ‌secrets‌ ‌on‌ ‌a‌ ‌regular‌ ‌basis.  | Use‌ ‌AWS‌ ‌Secrets‌ ‌Manager‌ ‌and‌ ‌enable‌ ‌automatic‌‌ rotation‌ ‌of‌ ‌credentials.‌ |


### **Domain‌ 4:‌ Design‌ Cost-Optimized‌ Architectures‌**
|Scenario                                                     | Solution‌                          |
|-------------------------------------------------------------|-----------------------------------|
|A‌ ‌cost-effective‌ ‌solution‌ ‌for‌ ‌over-provisioning‌ ‌of‌‌ resources.‌|Configure‌ ‌a‌ ‌target‌ ‌tracking‌ ‌scaling‌ ‌in‌ ‌ASG.‌|
|The‌ ‌application‌ ‌data‌ ‌is‌ ‌stored‌ ‌in‌ ‌a‌ ‌tape‌ ‌backup‌‌ solution.‌ ‌The‌ ‌backup‌ ‌data‌ ‌must‌ ‌be‌ ‌preserved‌ ‌for‌ ‌up‌ ‌to‌‌ directly‌ ‌to‌ 10‌ ‌years. | Use‌ ‌AWS‌ ‌Storage‌ ‌Gateway‌ ‌to‌ ‌backup‌ ‌the‌ ‌data‌‌  ‌Amazon‌ ‌S3‌ ‌Glacier‌ ‌Deep‌ ‌Archive.‌ ‌|
|Accelerate‌ ‌the‌ ‌transfer‌ ‌of‌ ‌historical‌ ‌records‌ ‌from‌‌ on-premises‌ ‌to‌ ‌AWS‌ ‌over‌ ‌the‌ ‌Internet‌ ‌in‌ ‌a‌‌ cost-effective‌ ‌manner. | Use‌ ‌AWS‌ ‌DataSync‌ ‌and‌ ‌select‌ ‌Amazon‌ ‌S3‌ ‌Glacier‌‌ Deep‌ ‌Archive‌ ‌as‌ ‌the‌ ‌destination |
|Globally‌ ‌deliver‌ ‌the‌ ‌static‌ ‌contents‌ ‌and‌ ‌media‌ ‌files‌ ‌to‌‌ customers‌ ‌around‌ ‌the‌ ‌world‌ ‌with‌ ‌low‌ ‌latency. | Store‌ ‌the‌ ‌files‌ ‌in‌ ‌Amazon‌ ‌S3‌ ‌and‌ ‌create‌ ‌a‌‌ CloudFront‌ ‌distribution.‌ ‌Select‌ ‌the‌ ‌S3‌ ‌bucket‌ ‌as‌ ‌the‌‌ origin.‌ |
|An‌ ‌application‌ ‌must‌ ‌be‌ ‌hosted‌ ‌to‌ ‌two‌ ‌EC2‌ ‌instances‌‌ and‌ ‌should‌ ‌continuously‌ ‌run‌ ‌for‌ ‌three‌ ‌years.‌ ‌The‌ ‌CPU‌‌ utilization‌ ‌of‌ ‌the‌ ‌EC2‌ ‌instances‌ ‌is‌ ‌expected‌ ‌to‌ ‌be‌‌ stable‌ ‌and‌ ‌predictable.‌ | Deploy‌ ‌the‌ ‌application‌ ‌to‌ ‌a‌ ‌Reserved‌ ‌instance.‌ |
|Implement‌ ‌a‌ ‌cost-effective‌ ‌solution‌ ‌for‌ ‌S3‌ ‌objects‌ ‌that‌‌  are‌ ‌accessed‌ ‌less‌ ‌frequently.‌ | Create‌ ‌an‌ ‌Amazon‌ ‌S3‌ ‌lifecycle‌ ‌policy‌ ‌to‌ ‌move‌ ‌the‌‌ ‌objects‌ ‌to‌ ‌Amazon‌ ‌S3‌ ‌Standard-IA.|
|Minimize‌ ‌the‌ ‌data‌ ‌transfer‌ ‌costs‌ ‌between‌ ‌two‌ ‌EC2‌‌ instances.‌ | Deploy‌ ‌the‌ ‌EC2‌ ‌instances‌ ‌in‌ ‌the‌ ‌same‌ ‌Region.‌|
|Import‌ ‌the‌ ‌SSL/TLS‌ ‌certificate‌ ‌of‌ ‌the‌ ‌application. | Import‌ ‌the‌ ‌certificate‌ ‌into‌ ‌AWS‌ ‌Certificate‌ ‌Manager‌‌ or‌ ‌upload‌ ‌it‌ ‌to‌ ‌AWS‌ ‌IAM.‌|