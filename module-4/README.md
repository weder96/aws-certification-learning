 <img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [Conteudo Geral AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Módulo 4: Segurança na nuvem (AWS Security Services)

## Conteúdo
1. <a href="#section-1"> Inspector </a>
2. <a href="#section-2"> AWS Artifact </a>
3. <a href="#section-3"> Amazon GuardDuty</a>
4. <a href="#section-4"> AWS WAF & AWS Shield</a>
5. <a href="#section-5"> AWS Key Management Service (AWS KMS)</a>
6. <a href="#section-6"> AWS CloudHSM</a>
7. <a href="#section-7"> AWS Certificate Manager</a>
8. <a href="#section-8"> AWS Inspector and AWS Trusted Advisor</a>
9. <a href="#section-9"> Penetration Testing</a>
10. <a href="#section-10"> AWS Single Sign-On (AWS SSO)</a>
11. <a href="#section-11"> Amazon Cognito</a>
12. <a href="#section-12"> AWS Directory Services </a>
13. <a href="#section-13"> AWS Systems Manager Parameter Store </a>
14. <a href="#section-14"> AWS Secrets Manager </a>
15. <a href="#section-15"> How do I report abuse of AWS resources?</a>

## <a id="section-1" ></a> **1 - Inspector**
[inspector](https://aws.amazon.com/pt/inspector/)

A Nuvem AWS permite um  modelo de responsabilidade compartilhada .

AWS gerencia a segurança da nuvem; você é responsável pela segurança na nuvem .

Você mantém o controle da segurança que escolhe implementar para proteger seu próprio conteúdo, plataforma, aplicativos, sistemas e redes da mesma forma que faria em um data center local.

**Benefícios da segurança da AWS**
- Mantenha seus dados seguros  – a infraestrutura da AWS implementa fortes proteções para ajudar.
- Proteja sua privacidade  – Todos os dados são armazenados em data centers altamente seguros da AWS.
- Atenda aos requisitos de conformidade  – a AWS gerencia dezenas de programas de conformidade em sua infraestrutura. Isso significa que os segmentos de sua conformidade já foram concluídos.
- Economize dinheiro  – reduza custos usando data centers da AWS. Mantenha o mais alto padrão de segurança sem ter que gerenciar suas próprias instalações.
- Escale rapidamente  – a segurança é dimensionada com o uso da Nuvem AWS. Não importa o tamanho do seu negócio, a infraestrutura da AWS foi projetada para manter seus dados seguros.

**Observância(Compliance)**
O AWS Cloud Compliance permite que você entenda os controles robustos em vigor na AWS para manter a segurança e a proteção de dados na nuvem.

À medida que os sistemas são criados com base na infraestrutura da Nuvem AWS, as responsabilidades de conformidade serão compartilhadas.

Os programas de conformidade incluem:
- Certificações / atestados.
- Leis, regulamentos e privacidade.
- Alinhamentos/quadros.


## <a id="section-2" ></a> **2 - AWS Artifact**
O [AWS Artifact](https://aws.amazon.com/pt/artifact/) é seu recurso central para informações relacionadas à conformidade que são importantes para você.

Ele fornece acesso sob demanda aos relatórios de segurança e conformidade da AWS e contratos online selecionados.

Os relatórios disponíveis no AWS Artifact incluem nossos relatórios de: 
- Service Organization Control (SOC) 
- Relatórios do Payment Card Industry (PCI)  
- Certificações de órgãos de credenciamento em todas as geografias e verticais de conformidade que validam a implementação e a eficácia operacional dos controles de segurança da AWS.

Os contratos disponíveis no [AWS Artifact](https://aws.amazon.com/pt/artifact/) incluem o Business Associate Addendum (BAA) e o Nondisclosure Agreement (NDA).

[AWS Artifact](https://aws.amazon.com/pt/artifact/) is the go-to, central resource for compliance-related information that matters to you. It provides on-demand access to AWS’ security and compliance reports and select online agreements.

Reports available in [AWS Artifact](https://aws.amazon.com/pt/artifact/) include Service Organization Control [(SOC) reports, Payment Card Industry (PCI) reports](https://aws.amazon.com/blogs/security/tag/aws-soc-reports/), 
and certifications from accreditation bodies across geographies and compliance verticals that validate the implementation and operating effectiveness of AWS security controls.


## <a id="section-3" ></a> **3 - Amazon GuardDuty**
O Amazon GuardDuty oferece detecção de ameaças e monitoramento contínuo de segurança para comportamento mal-intencionado ou não autorizado para ajudar a proteger suas contas e cargas de trabalho da AWS.

Serviço inteligente de detecção de ameaças.

Detecta comprometimento de conta, comprometimento de instância, reconhecimento malicioso e comprometimento de bucket.

Monitoramento contínuo de eventos em:
- Eventos de gerenciamento do AWS CloudTrail.
- Eventos de dados do AWS CloudTrail S3.
- Logs de fluxo da Amazon VPC.
- Registros DNS.


## <a id="section-4" ></a> **4 - AWS WAF & AWS Shield**
**WAF:**
- AWS WAF é um firewall de aplicativo web.
- Protege contra explorações comuns que podem comprometer a disponibilidade do aplicativo, comprometer a segurança ou consumir recursos excessivos.
- O WAF permite criar regras para filtrar o tráfego da Web com base em condições que incluem endereços IP, cabeçalhos e corpo HTTP ou URIs personalizados.
- O WAF facilita a criação de regras que bloqueiam explorações comuns da Web, como injeção de SQL e script entre sites.
- As regras são conhecidas como Web ACLs.

**AWS Shield**
- O AWS Shield é um serviço de proteção de negação de serviço distribuído (DDoS) gerenciado.
- Protege o aplicativo da web em execução na AWS com detecção sempre ativa e mitigações automáticas em linha.
Ajuda a minimizar o tempo de inatividade e a latência do aplicativo.
Dois níveis – Padrão e Avançado.

## <a id="section-5" ></a> **5 - AWS Key Management Service (AWS KMS)**
O AWS Key Management Service oferece controle centralizado sobre as chaves de criptografia usadas para proteger seus dados.

Você pode criar, importar, alternar, desabilitar, excluir, definir políticas de uso e auditar o uso de chaves de criptografia usadas para criptografar seus dados.

O AWS Key Management Service é integrado à maioria dos outros serviços da AWS, facilitando a criptografia dos dados armazenados nesses serviços com as chaves de criptografia que você controla.

O AWS KMS é integrado ao AWS CloudTrail, que oferece a capacidade de auditar quem usou quais chaves, em quais recursos e quando.

O AWS KMS permite que os desenvolvedores criptografem dados com facilidade, seja por meio de criptografia com um clique no Console de gerenciamento da AWS ou usando o AWS SDK para adicionar criptografia facilmente ao código do aplicativo.


## <a id="section-6" ></a> **6 - AWS CloudHSM**
O **AWS CloudHSM** é um módulo de segurança de hardware (HSM) baseado em nuvem que permite gerar e usar facilmente suas próprias chaves de criptografia na Nuvem AWS.

Com o CloudHSM, você pode gerenciar suas próprias chaves de criptografia usando HSMs validados para FIPS 140-2 Nível 3.

O CloudHSM oferece a flexibilidade de integração com seus aplicativos usando APIs padrão do setor, como PKCS#11, Java Cryptography Extensions (JCE) e bibliotecas Microsoft CryptoNG (CNG).


## <a id="section-7" ></a> **7 - AWS Certificate Manager**
O **AWS Certificate Manager** é um serviço que permite provisionar, gerenciar e implantar facilmente certificados Secure Sockets Layer/Transport Layer Security (SSL/TLS) públicos e privados para uso com serviços da AWS e seus recursos internos conectados.

Os certificados SSL/TLS são usados ​​para proteger as comunicações de rede e estabelecer a identidade de sites na Internet, bem como recursos em redes privadas.

O AWS Certificate Manager remove o demorado processo manual de compra, upload e renovação de certificados SSL/TLS.


## <a id="section-8" ></a> **8 - AWS Inspector and AWS Trusted Advisor**
**AWS Inspector:**

O **Inspector** é um serviço automatizado de avaliação de segurança que ajuda a melhorar a segurança e a conformidade de aplicativos implantados na AWS.
O **Inspector** avalia automaticamente os aplicativos quanto a vulnerabilidades ou desvios das melhores práticas.
Usa um agente instalado em instâncias do EC2.
As instâncias devem ser marcadas.

**Trusted Advisor**
O **Trusted Advisor** é um recurso online que ajuda a reduzir custos, aumentar o desempenho e melhorar a segurança otimizando seu ambiente AWS.
O **Trusted Advisor** fornece orientação em tempo real para ajudá-lo a provisionar seus recursos seguindo as práticas recomendadas.
O **Trusted Advisor** irá aconselhá-lo sobre otimização de custos, desempenho, segurança e tolerância a falhas.

O **Trusted Advisor** verifica sua infraestrutura da AWS e a compara com as melhores práticas da AWS em cinco categorias:
- Otimização de Custos.
- Performance.
- Segurança.
- Tolerância ao erro.
- Limites de serviço.

O Trusted Advisor vem em duas versões:
Core Checks and Recommendations (free):
- Acesso às 7 verificações principais para ajudar a aumentar a segurança e o desempenho.
- As verificações incluem:
     - S3 bucket permissions; 
     - Security Groups; 
     - IAM use;
     - MFA on root account;
     - EBS public snapshots; 
     - RDS public snapshots;

Benefícios Completos do Trusted Advisor (planos de suporte empresarial e empresarial):

Conjunto completo de verificações para ajudar a otimizar toda a sua infraestrutura da AWS.
Aconselha sobre segurança, desempenho, custo, tolerância a falhas e limites de serviço.
Os benefícios adicionais incluem notificações de atualização semanais, alertas, ações automatizadas com o CloudWatch e acesso programático usando a API do AWS Support.


## <a id="section-9" ></a> **9 - Penetration Testing**
O **Penetration Testing** é a prática de testar a segurança do próprio aplicativo em busca de vulnerabilidades, simulando um ataque.

A AWS permite **Penetration Testing**. Há um conjunto limitado de recursos nos quais o teste de penetração pode ser realizado.

Você não precisa de permissão para realizar testes de penetração nos seguintes serviços:
- Amazon EC2 instances, NAT Gateways, and Elastic Load Balancers.
- Amazon RDS.
- Amazon CloudFront.
- Amazon Aurora.
- Amazon API Gateways.
- AWS Lambda and Lambda Edge functions.
- Amazon LightSail resources.
- Amazon Elastic Beanstalk environments.

Você pode ler a política completa de suporte a testes de vulnerabilidade e penetração  [aqui](https://aws.amazon.com/pt/security/penetration-testing/) .

Caso uma conta esteja ou possa estar comprometida, a AWS recomenda que as seguintes etapas sejam executadas:
1. Change your AWS root account password.
2. Change all IAM user’s passwords.
3. Delete or rotate all programmatic (API) access keys.
4. Delete any resources in your account that you did not create.
5. Respond to any notifications you received from AWS through the AWS Support Center and/or contact AWS Support to open a support case.

## <a id="section-10" ></a> **10 - AWS Single Sign-On (AWS SSO)**
O **AWS Single Sign-On (AWS SSO)** é um serviço de logon único (SSO) baseado em nuvem que facilita o gerenciamento centralizado do acesso SSO a todas as suas contas da AWS e aplicativos de nuvem.

Ele ajuda você a gerenciar o acesso de SSO e as permissões de usuário em todas as suas contas da AWS no AWS Organizations.

O AWS SSO também ajuda a gerenciar o acesso e as permissões para aplicativos de software como serviço (SaaS) de terceiros comumente usados, aplicativos integrados ao AWS SSO, bem como aplicativos personalizados que oferecem suporte a Security Assertion Markup Language (SAML) 2.0.

O AWS SSO inclui um portal do usuário no qual seus usuários finais podem encontrar e acessar todas as contas atribuídas da AWS, aplicativos de nuvem e aplicativos personalizados em um só lugar.

## <a id="section-11" ></a> **11 - Amazon Cognito**
O Amazon Cognito permite que você adicione a inscrição, o login e o controle de acesso do usuário aos seus aplicativos web e móveis de maneira rápida e fácil.

O Amazon Cognito é dimensionado para milhões de usuários e oferece suporte ao login com provedores de identidade social, como Apple, Facebook, Google e Amazon, e provedores de identidade corporativa via SAML 2.0 e OpenID Connect.

Os dois principais componentes do AWS Cognito são grupos de usuários e grupos de identidades:
- **User pools** são diretórios de usuários que fornecem opções de inscrição e entrada para os usuários do seu aplicativo.
- Os **Identity pools** permitem que você conceda aos usuários acesso a outros serviços da AWS.

Você pode usar grupos de identidades e grupos de usuários separadamente ou em conjunto.


## <a id="section-12" ></a> **12 - AWS Directory Services**
A AWS fornece vários tipos de diretório.

Os três tipos a seguir aparecem atualmente no exame e serão abordados nesta página:
- Serviço Active Directory para Microsoft Active Directory.
- AD simples.
- Conector AD.

Como alternativa ao serviço AWS Directory, você pode criar seus próprios DCs do Microsoft AD na nuvem AWS (no EC2).

A tabela abaixo resume os serviços de diretório abordados nesta página, bem como alguns outros, e fornece alguns casos de uso típicos:

|Opção de serviço de diretório	|Descrição	|Caso de uso|
|-------------------------------|-----------|-----------|
|AWS Directory Service para Microsoft Active Directory	|Microsoft AD completo gerenciado pela AWS em execução no Windows Server 2012 R2	|Empresas que desejam o Microsoft AD hospedado ou você precisa de LDAP para aplicativos Linux|
|Conector AD	|Permite que os usuários locais façam login nos serviços da AWS com suas credenciais do AD existentes. Também permite que instâncias do EC2 ingressem no domínio AD	|Logon único para funcionários locais e para adicionar instâncias do EC2 ao domínio|
|AD simples	|Implementação de AD de baixa escala e baixo custo com base no Samba	|Diretório de usuário simples ou você precisa de compatibilidade com LDAP|


## <a id="section-13" ></a> **13 - AWS Systems Manager Parameter Store**
Fornece armazenamento seguro e hierárquico para gerenciamento de dados de configuração e gerenciamento de segredos.

É altamente escalável, disponível e durável.

Você pode armazenar dados como senhas, strings de banco de dados e códigos de licença como valores de parâmetro.

Você pode armazenar valores como texto simples (dados não criptografados) ou texto cifrado (dados criptografados).

Você pode então referenciar valores usando o nome exclusivo que você especificou quando criou o parâmetro.

## <a id="section-14" ></a> **14 - AWS Secrets Manager**

Como Loja de Parâmetros.

Permite rotação nativa e automática de chaves.

Permissões refinadas.

Auditoria central para rotação secreta.

## <a id="section-15" ></a> **15 -  How do I report abuse of AWS resources?**


### **I suspect that AWS resources are used for abusive or illegal purposes. How do I let AWS know?** [here](https://aws.amazon.com/pt/premiumsupport/knowledge-center/report-aws-abuse/)

**Resolution:**
The AWS Trust & Safety team can assist you when AWS resources are used to engage in the following types of abusive behavior:
- **Spam:** You are receiving unwanted emails from an AWS-owned IP address, or AWS resources are used to spam websites or forums.
- **Port scanning:** Your logs show that one or more AWS-owned IP addresses are sending packets to multiple ports on your server. You also believe this is an attempt to discover unsecured ports.
- **Denial-of-service (DoS) attacks:** Your logs show that one or more AWS-owned IP addresses are used to flood ports on your resources with packets. You also believe that this is an attempt to overwhelm or crash your server or the software running on your server.
- **Intrusion attempts:** Your logs show that one or more AWS-owned IP addresses are used to attempt to log in to your resources.
- **Hosting prohibited content:** You have evidence that AWS resources are used to host or distribute prohibited content, such as illegal content or copyrighted content without the consent of the copyright holder.
- **Distributing malware:** You have evidence that AWS resources are used to distribute software that was knowingly created to compromise or cause harm to computers or machines that it's installed on.

If you suspect that AWS resources are used for abusive purposes, contact the AWS Trust & Safety team using the Report Amazon AWS abuse form, or by contacting abuse@amazonaws.com. Provide all the necessary information, including logs in plaintext, email headers, and so on, when you submit your request.

The AWS Trust & Safety team will use the information that you provide in this form to investigate and attempt to resolve the incident you have reported. We might share your information, if it is necessary for the investigation of your report.

Note: AWS Support can't assist with reports of abuse or questions about notifications from the AWS Trust & Safety team. If you have questions for the AWS Trust & Safety team, reply directly to their email.

If you suspect that AWS resources are used for abusive purposes, contact the AWS Trust & Safety team using the Report Amazon AWS abuse form, or by contacting abuse@amazonaws.com. Provide all the necessary information, including logs in plaintext, email headers, and so on, when you submit your request.
AWS Trust & Safety team.


