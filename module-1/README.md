<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50> [Conteudo Geral AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning


# Módulo 1: Visão geral dos conceitos de nuvem


## Conteúdo
1. <a href="#section-1"> Introdução à computação em nuvem </a>
2. <a href="#section-2"> Vantagens da computação em nuvem </a>
3. <a href="#section-3"> Introdução à Amazon Web Services (AWS) </a>
4. <a href="#section-4"> Mudança para a Nuvem AWS – AWS Cloud Adoption Framework (AWS CAF)</a>
5. <a href="#section-5"> AWS Shared Responsibility Model</a>

## <a id="section-1" ></a> Seção 1 - Introdução à computação em nuvem

O que é computação em nuvem?

- É a entrega sob demanda de poder computacional, banco de dados, armazenamento, aplicativos e outros recursos de TI pela Internet com uma definição de preço conforme o uso.
- Servidores em grandes datacenters
- Pensar na infraestrutura como um software

Infraestrutura como hardware:

- Exigem espaço, equipe, segurança física, planejamento, despesas de capital
- Têm um ciclo longo de aquisição de hardware
- Exigem provisionamento de capacidade por meio da tentativa de adivinhar os picos máximos teóricos

Infraestrutura como software:

- São flexíveis
- Podem mudar com mais rapidez
- Eliminam as tarefas monolíticas de trabalho pesado

**Tipos de Serviços Cloud - (Iass x Paas x Saas x Caas)**

### Há três principais modelos de implantação de computação em nuvem:

- **Infrastructure as a Service (IaaS)** - Serviços que fornecem conexão de rede, SOs, armazenamento, alta flexibilidade de utilização. Costumam ser genéricos, podem ser utilizados para vários fins. Ex:  [EC2](https://aws.amazon.com/pt/ec2/) da AWS [instance-types](<https://aws.amazon.com/pt/ec2/instance-types/>).
- **Platform as a Service (PaaS)** - Serviços que fornecem uma plataforma para deployment, restauração, manutenção de dados, mas não te dão acesso ao SO diretamente, Ex: Elastic BeanStalk, [S3](https://aws.amazon.com/pt/s3/).
- **Software as a Service (SaaS)** - Serviços que atuam como uma aplicação na nuvem gerenciada pela AWS que você chama da sua aplicação para algum fim, Ex: Rekognition, Polly, Translate.
- **Code as a Service (Caas)** ou Function as a Service (FaaS) - Serviços orientados a evento que executam uma função simples na núvem em um ambiente serverless, Ex: [Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html).

### **TIPOS DE COMPUTAÇÃO EM NUVEM**

3 tipos de modelo de computação em nuvem: 
- Infraestrutura como serviço (IaaS) 
- Plataforma como serviço (PaaS) 
- Software como serviço (SaaS)

**TIPOS DE IMPLANTAÇÃO DE NUVEM**

Existem 4 tipos de implantação na nuvem:
- **Nuvem pública ou simples** “nuvem” – ex. AWS, Azure, GCP
- **Nuvem Híbrida** – mistura de nuvens públicas e privadas
- **Multi Cloud** - usando mais de 1 nuvem pública em uma implantação.
- **Nuvem privada (on-premise)** – gerenciada em seu próprio data center, por exemplo, Hyper-V, OpenStack, VMware

**Nuvem Pública**

Um aplicativo baseado em nuvem é totalmente implantado na nuvem e todas as partes do aplicativo são executadas na nuvem. Os aplicativos na nuvem foram criados na nuvem ou migrados de uma infraestrutura existente para aproveitar os benefícios da computação em nuvem. Os aplicativos baseados em nuvem podem ser criados em peças de infraestrutura de baixo nível ou podem usar serviços de nível superior que fornecem abstração dos requisitos de gerenciamento, arquitetura e dimensionamento da infraestrutura principal.

**Híbrido**

Uma implantação híbrida é uma maneira de conectar infraestrutura e aplicativos entre recursos baseados em nuvem e recursos existentes que não estão localizados na nuvem.

O método mais comum de implantação híbrida é entre a nuvem e a infraestrutura local existente para estender e expandir a infraestrutura de uma organização para a nuvem enquanto conecta os recursos da nuvem ao sistema interno.

**Nuvem privada (on-premise)**

A implantação de recursos no local usando ferramentas de virtualização e gerenciamento de recursos às vezes é chamada de “nuvem privada”. A implantação no local não oferece muitos dos benefícios da computação em nuvem, mas às vezes é procurada por sua capacidade de fornecer recursos dedicados.

Na maioria dos casos, esse modelo de implantação é o mesmo que a infraestrutura de TI herdada, usando tecnologias de gerenciamento e virtualização de aplicativos para tentar aumentar a utilização de recursos.
Há muitas semelhanças entre a AWS e uma implementação de TI tradicional. 

**Multi Cloud** - 
A linha entre nuvem híbrida e multicloud está embaçada neste momento. A nuvem híbrida é certamente mais expansiva em sua definição (pública, local, borda). 

A multinuvem geralmente se refere a várias nuvens públicas. O que o torna embaçado é que a nuvem é uma mentalidade - não um local físico. Como resultado, vemos os termos usados alternadamente nos dias de hoje.

Uma coisa é clara, no entanto, é que, independentemente das definições - os primeiros princípios necessários para o sucesso em ambos são notavelmente semelhantes.

***************************************************************************************************************************

## <a id="section-2" ></a> Seção 2 - Vantagens da computação em nuvem
- Troque despesas de capital por despesas variáveis
- Grande economia de escala
- Pare de tentar adivinhar a capacidade
- Aumente a velocidade e a agilidade
- Pare de gastar dinheiro com a operação e manutenção de datacenters
- Tenha alcance global em minutos

**Por que a computação em nuvem é tão popular?**

Dependendo de para quem você pergunta, algumas estimativas apontam o mercado global de computação em nuvem em cerca de US$ 370 bilhões em 2020, crescendo para cerca de US$ 830 bilhões em 2025.

Isso implica uma taxa de crescimento anual composta (CAGR) de cerca de 18% para o período. 

Existem várias razões pelas quais o mercado de nuvem está crescendo tão rápido. Alguns deles são: 

- Elasticidade
- Segurança
- Disponibilidade
- Ciclos de hardware mais rápidos
- Pessoal de administração do sistema
- Tempo de comercialização mais rápido

## Os seis pilares de uma estrutura bem arquitetada

<a href="https://aws.amazon.com/blogs/apn/the-6-pillars-of-the-aws-well-architected-framework/" target="_blank"> 
    Os seis pilares de uma estrutura bem arquitetada
</a>

Acesso em: Junho de 2022.

Criar um sistema de software é muito parecido com construir um edifício. Se a fundação não for sólida, problemas estruturais podem prejudicar a integridade e a função do edifício.

Ao criar soluções de tecnologia na Amazon Web Services (AWS), se você negligenciar os seis pilares de excelência operacional, segurança, confiabilidade, eficiência de desempenho, otimização de custos e sustentabilidade, pode se tornar um desafio criar um sistema que atenda às suas expectativas e requisitos.

Incorporar esses pilares em sua arquitetura ajuda a produzir sistemas estáveis ​​e eficientes. Isso permite que você se concentre em outros aspectos do design, como requisitos funcionais.

O AWS Well-Architected Framework ajuda os arquitetos de nuvem a criar a infraestrutura mais segura, de alto desempenho, resiliente e eficiente possível para seus aplicativos. A estrutura oferece uma abordagem consistente para que clientes e parceiros da AWS avaliem arquiteturas e fornece orientação para implementar designs que se adaptam às necessidades do seu aplicativo ao longo do tempo.

Fornecemos uma visão geral dos seis pilares do Well-Architected Framework e exploramos os princípios de design e as melhores práticas. Você pode encontrar mais detalhes, incluindo definições, perguntas frequentes e recursos, no whitepaper de cada pilar ao qual linkamos abaixo.

<a href="https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html" target="_blank"> 
    Whitepaper - visão geral dos seis pilares do Well-Architected Framework
</a>
<br/><br/><br/>

**1. Excelência Operacional**

O pilar Excelência Operacional inclui a capacidade de dar suporte ao desenvolvimento e executar cargas de trabalho de forma eficaz, obter informações sobre sua operação e melhorar continuamente os processos e procedimentos de suporte para fornecer valor comercial. 

Você pode encontrar orientações prescritivas sobre implementação no whitepaper do Pilar de Excelência Operacional.

### Princípios de design

Existem cinco princípios de design para excelência operacional na nuvem:
- Executar operações como código
- Faça mudanças frequentes, pequenas e reversíveis
- Refine os procedimentos de operações com frequência
- Antecipar falha
- Aprenda com todas as falhas operacionais


### Melhores Práticas
- As equipes de operações precisam entender suas necessidades de negócios e clientes para que possam oferecer suporte aos resultados de negócios. 
- O Operador cria e usa procedimentos para responder a eventos operacionais e valida sua eficácia para atender às necessidades de negócios. 
- O Operador também coleta métricas que são usadas para medir a obtenção dos resultados de negócios desejados.
- Tudo continua a mudar - seu contexto de negócios, prioridades de negócios e necessidades do cliente. 
- É importante projetar operações para apoiar a evolução ao longo do tempo em resposta à mudança e incorporar as lições aprendidas por meio de seu desempenho.

**2. Segurança**

O pilar Segurança inclui a capacidade de proteger dados, sistemas e ativos para aproveitar as tecnologias de nuvem para melhorar sua segurança. Você pode encontrar orientações prescritivas sobre implementação no whitepaper do Pilar de Segurança.


## Princípios de design

Existem sete princípios de design para segurança na nuvem:

- Implemente uma base de identidade forte
- Ativar rastreabilidade
- Aplique segurança em todas as camadas
- Automatize as melhores práticas de segurança
- Proteja os dados em trânsito e em repouso
- Mantenha as pessoas longe dos dados
- Prepare-se para eventos de segurança

### Melhores Práticas

Antes de arquitetar qualquer carga de trabalho, você precisa implementar práticas que influenciem a segurança. 

Você vai querer controlar quem pode fazer o quê. Além disso, você deseja identificar incidentes de segurança, proteger seus sistemas e serviços e manter a confidencialidade e a integridade dos dados por meio da proteção de dados.

Você deve ter um processo bem definido e praticado para responder a incidentes de segurança. Essas ferramentas e técnicas são importantes porque dão suporte a objetivos como evitar perdas financeiras ou cumprir obrigações regulatórias.

O modelo de responsabilidade compartilhada da AWS permite que as organizações que adotam a nuvem atinjam suas metas de segurança e conformidade. 

Como a AWS protege fisicamente a infraestrutura que dá suporte aos nossos serviços de nuvem, como cliente da AWS, você pode se concentrar no uso de serviços para atingir suas metas. 

A Nuvem AWS também oferece maior acesso aos dados de segurança e uma abordagem automatizada para responder a eventos de segurança.

**3. Confiabilidade**

O pilar Confiabilidade abrange a capacidade de uma carga de trabalho de executar sua função pretendida de forma correta e consistente quando se espera. 

Isso inclui a capacidade de operar e testar a carga de trabalho durante todo o seu ciclo de vida. Você pode encontrar orientações prescritivas sobre implementação no whitepaper do Pilar de Confiabilidade.

### Princípios de design

Existem cinco princípios de design para confiabilidade na nuvem:

Recuperar automaticamente de falhas:
- Procedimentos de recuperação de teste
- Dimensione horizontalmente para aumentar a disponibilidade da carga de trabalho agregada
- Pare de adivinhar a capacidade
- Gerenciar mudanças na automação

### Melhores Práticas
Antes de construir qualquer sistema, os requisitos fundamentais que influenciam a confiabilidade devem estar em vigor. 

Por exemplo, você deve ter largura de banda de rede suficiente para seu data center. Esses requisitos às vezes são negligenciados (porque estão além do escopo de um único projeto). 

Com a AWS, no entanto, a maioria dos requisitos fundamentais já está incorporada ou pode ser abordada conforme necessário.

A nuvem foi projetada para ser quase ilimitada, portanto, é responsabilidade da AWS atender ao requisito de rede e capacidade de computação suficientes, deixando você livre para alterar o tamanho e as alocações de recursos sob demanda.

Uma carga de trabalho confiável começa com decisões iniciais de design para software e infraestrutura. 

Suas escolhas de arquitetura afetarão o comportamento da carga de trabalho em todos os seis pilares do AWS Well-Architected. 

Para confiabilidade, há padrões específicos que você deve seguir, como dependências fracamente acopladas, degradação normal e tentativas limitantes.

As alterações em sua carga de trabalho ou em seu ambiente devem ser antecipadas e acomodadas para obter uma operação confiável da carga de trabalho.

 As alterações incluem aquelas impostas à sua carga de trabalho, como picos de demanda, bem como aquelas internas, como implantações de recursos e patches de segurança.

Falhas de componentes de hardware de baixo nível são algo a ser tratado todos os dias em um data center local. 

Na nuvem, no entanto, eles geralmente são abstraídos. Independentemente do seu provedor de nuvem, existe a possibilidade de falhas afetarem sua carga de trabalho. 

Portanto, você deve tomar medidas para implementar a resiliência em sua carga de trabalho, como isolamento de falhas, failover automatizado para recursos íntegros e uma estratégia de recuperação de desastres.

**4. Eficiência de Desempenho**

O pilar Eficiência de Desempenho inclui a capacidade de usar recursos de computação com eficiência para atender aos requisitos do sistema e manter essa eficiência à medida que a demanda muda e as tecnologias evoluem. 

Você pode encontrar orientações prescritivas sobre implementação no whitepaper do Pilar de Eficiência de Desempenho.

### Princípios de design

Existem cinco princípios de design para eficiência de desempenho na nuvem:

Democratizar tecnologias avançadas:
- Torne-se global em minutos
- Use arquiteturas sem servidor
- Experimente com mais frequência
- Considere a simpatia mecânica

### Melhores Práticas

Adote uma abordagem orientada por dados para criar uma arquitetura de alto desempenho. Reúna dados sobre todos os aspectos da arquitetura, desde o design de alto nível até a seleção e configuração de tipos de recursos.

Revisar suas escolhas regularmente garante que você aproveite a constante evolução da Nuvem AWS. O monitoramento garante que você esteja ciente de qualquer desvio do desempenho esperado. Faça compensações em sua arquitetura para melhorar o desempenho, como usar compactação ou armazenamento em cache ou relaxar os requisitos de consistência

A solução ideal para uma carga de trabalho específica varia e as soluções geralmente combinam várias abordagens. As cargas de trabalho AWS Well-Architected usam várias soluções e habilitam diferentes recursos para melhorar o desempenho


**5. Otimização de Custos**

O pilar Otimização de Custos inclui a capacidade de executar sistemas para fornecer valor comercial ao menor preço. Você pode encontrar orientações prescritivas sobre implementação no whitepaper do Pilar de Otimização de Custos.

### Princípios de design

Existem cinco princípios de design para otimização de custos na nuvem:
- Implemente o gerenciamento financeiro na nuvem
- Adote um modelo de consumo
- Meça a eficiência geral
- Pare de gastar dinheiro em trabalho pesado indiferenciado
- Analisar e atribuir despesas

### Melhores Práticas
Tal como acontece com os outros pilares, existem trade-offs a serem considerados. 

Por exemplo, você deseja otimizar a velocidade de lançamento no mercado ou o custo? Em alguns casos, é melhor otimizar a velocidade – entrar no mercado rapidamente, enviar novos recursos ou simplesmente cumprir um prazo – em vez de investir na otimização de custos inicial.

As decisões de design às vezes são direcionadas pela pressa em vez de dados, e como sempre existe a tentação de supercompensar em vez de gastar tempo fazendo benchmarking para a implantação com o melhor custo-benefício. 
Isso pode levar a implantações superprovisionadas e subotimizadas.

Usar os serviços, recursos e configurações apropriados para suas cargas de trabalho é fundamental para a economia de custos

**6. Sustentabilidade**

A disciplina de sustentabilidade aborda o impacto ambiental, econômico e social de longo prazo de suas atividades de negócios. Você pode encontrar orientações prescritivas sobre implementação no whitepaper do Pilar de Sustentabilidade.

### Princípios de design

Existem seis princípios de design para sustentabilidade na nuvem:
- Entenda seu impacto
- Estabeleça metas de sustentabilidade
- Maximizar a utilização
- Antecipar e adotar novas ofertas de hardware e software mais eficientes
- Usar serviços gerenciados
- Reduza o impacto downstream de suas cargas de trabalho na nuvem

### Melhores Práticas

Escolha as regiões da AWS onde você implementará cargas de trabalho com base em seus requisitos de negócios e metas de sustentabilidade.

Os padrões de comportamento do usuário podem ajudá-lo a identificar melhorias para atingir as metas de sustentabilidade. Por exemplo, reduza a infraestrutura quando não for necessária, posicione recursos para limitar a rede necessária para que os usuários os consumam e remova ativos não utilizados.

Implemente padrões de software e arquitetura para realizar a suavização de carga e manter a alta utilização consistente dos recursos implantados. 

Entenda o desempenho de seus componentes de carga de trabalho e otimize os componentes que consomem mais recursos.

Analise os padrões de dados para implementar práticas de gerenciamento de dados que reduzem o armazenamento provisionado necessário para dar suporte à sua carga de trabalho. Use os recursos do ciclo de vida para mover dados para um armazenamento mais eficiente e de menor desempenho quando os requisitos diminuirem e excluir dados que não são mais necessários.

Analise os padrões de hardware para identificar oportunidades que reduzem os impactos de sustentabilidade da carga de trabalho, minimizando a quantidade de hardware necessária para provisionar e implantar. Selecione o hardware mais eficiente para sua carga de trabalho individual.

Em seu processo de desenvolvimento e implantação, identifique oportunidades para reduzir seu impacto de sustentabilidade fazendo mudanças, como atualizar sistemas para obter eficiências de desempenho e gerenciar impactos de sustentabilidade. Use a automação para gerenciar o ciclo de vida de seus ambientes de desenvolvimento e teste e use farms de dispositivos gerenciados para teste.


## CONCEITOS GERAIS DE COMPUTAÇÃO EM NUVEM
A computação em nuvem é a entrega sob demanda de poder de computação, armazenamento de banco de dados, aplicativos e outros recursos de TI por meio de uma plataforma de serviços em nuvem pela Internet com preços pagos conforme o uso.

A computação em nuvem fornece uma maneira simples de acessar servidores, armazenamento, bancos de dados e um amplo conjunto de serviços de aplicativos pela Internet.

Uma plataforma de serviços em nuvem, como a Amazon Web Services, possui e mantém o hardware conectado à rede necessário para esses serviços de aplicativos, enquanto você provisiona e usa o que precisa por meio de um aplicativo da web.

### **AS SEIS VANTAGENS**

A AWS promove as [seis vantagens](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html) da nuvem:
1. **Trocar despesas de capital por despesas variáveis** 
**(Trade fixed expense for variable expense)** ​​– Em vez de ter que investir pesadamente em data centers e servidores antes de saber como usá-los, você pode pagar apenas quando consumir recursos de computação e pagar apenas por quanto consumir .

2. **Beneficie-se de enormes economias de escala (Benefit from massive economies of scale)** – Ao usar a computação em nuvem, você pode obter um custo variável mais baixo do que poderia obter por conta própria. Como o uso de centenas de milhares de clientes é agregado na nuvem, provedores como a AWS podem obter maiores economias de escala, o que se traduz em preços mais baixos de pagamento conforme o uso.

3. **Pare de adivinhar sobre a capacidade (Stop guessing capacity)** – Elimine adivinhações sobre suas necessidades de capacidade de infraestrutura. Quando você toma uma decisão de capacidade antes de implantar um aplicativo, geralmente acaba ficando com recursos ociosos caros ou lidando com capacidade limitada. Com a computação em nuvem, esses problemas desaparecem. Você pode acessar o máximo ou o mínimo de capacidade que precisar e aumentar e diminuir conforme necessário com apenas alguns minutos de antecedência.

4. **Aumente a velocidade e a agilidade(Increase speed and agility)** – Em um ambiente de computação em nuvem, novos recursos de TI estão a apenas um clique de distância, o que significa que você reduz o tempo para disponibilizar esses recursos para seus desenvolvedores de semanas para apenas alguns minutos. Isso resulta em um aumento dramático na agilidade da organização, pois o custo e o tempo necessários para experimentar e desenvolver são significativamente menores.

5. **Pare de gastar dinheiro executando e mantendo data centers(Stop spending money running and maintaining data centers )** – Concentre-se em projetos que diferenciam seus negócios, não a infraestrutura. A computação em nuvem permite que você se concentre em seus próprios clientes, e não no trabalho pesado de armazenamento em rack, empilhamento e alimentação de servidores.

6. **Torne-se global em minutos(Go global in minutes)** – Implante facilmente seu aplicativo em várias regiões do mundo com apenas alguns cliques. Isso significa que você pode fornecer menor latência e uma melhor experiência para seus clientes a um custo mínimo.

<a href="https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html" target="_blank"> 
    Whitepaper - Six advantages of cloud computing
</a>
<br/><br/><br/>


**DESPESAS DE CAPITAL DE COMÉRCIO PARA DESPESAS VARIÁVEIS**
Em vez de ter que investir pesadamente em data centers e servidores antes de saber como usá-los, você pode pagar apenas quando consumir recursos de computação e pagar apenas por quanto consumir.

**BENEFÍCIOS DE ECONOMIAS MASSIVAS DE ESCALA**
Ao usar a computação em nuvem, você pode obter um custo variável mais baixo do que pode obter por conta própria. À medida que o uso de centenas de milhares de clientes é agregado na nuvem, provedores como a AWS podem obter maiores economias de escala, o que se traduz em preços mais baixos de pagamento conforme o uso.

**PARE DE SUGERIR SOBRE A CAPACIDADE**
Quando você toma uma decisão de capacidade antes de implantar um aplicativo, geralmente acaba ficando com recursos ociosos caros ou lidando com capacidade limitada. Com a computação em nuvem, você elimina as suposições sobre suas necessidades de capacidade de infraestrutura. Você pode acessar o máximo ou o mínimo de capacidade que precisar e aumentar e diminuir conforme necessário com apenas alguns minutos de antecedência.

**AUMENTAR VELOCIDADE E AGILIDADE**
Em um ambiente de computação em nuvem, novos recursos de TI estão a apenas um clique de distância, o que significa que você reduz o tempo para disponibilizar esses recursos para seus desenvolvedores de semanas para apenas alguns minutos. Isso resulta em um aumento dramático na agilidade da organização, pois o custo e o tempo necessários para experimentar e desenvolver são significativamente menores

**PARAR DE GASTAR DINHEIRO EXECUTAR E MANTER DATA CENTERS**
Concentre-se em projetos que diferenciam seu negócio, não na infraestrutura. A computação em nuvem permite que você se concentre em seus próprios clientes, e não no trabalho pesado de armazenamento em rack, empilhamento e alimentação de servidores.

**GLOBAL EM MINUTOS**
Implante facilmente seu aplicativo em várias regiões do mundo com apenas alguns cliques. Isso significa que você pode fornecer menor latência e uma melhor experiência para seus clientes a um custo mínimo.

***************************************************************************************************************************

## <a id="section-3" ></a> Seção 3 - Introdução à Amazon Web Services (AWS)

O que são serviços web?

- É qualquer software disponibilizado pela Internet que usa um formato padronizado, como XML ou JSON, para a solicitação e resposta de uma interação de API.

O que é a AWS?

- Uma plataforma de nuvem segura que oferece um amplo conjunto de produtos globais baseados na nuvem.
- Oferece acesso sob demanda a recursos de computação, armazenamento, rede, banco de dados e outros recursos de TI e ferramentas de gerenciamento.
- Oferece flexibilidade.
- Você paga apenas pelos serviços individuais de que precisa, pelo tempo que os utilizar.
- Os serviços da AWS funcionam juntos como componentes básicos.

Maneiras de interagir com a AWS

- Console de Gerenciamento da AWS: interface gráfica fácil de usar
- Interface da linha de comando (CLI da AWS): acesso a serviços por comandos ou scripts específicos
- Kits de desenvolvimento de software (SDKs): acesse serviços diretamente do seu código (como Java, Python e outros)

## <a id="section-4" ></a> Seção 4 - Mudança para a Nuvem AWS – AWS Cloud Adoption Framework (AWS CAF) 

AWS Cloud Adoption Framework: é um documento criado para ajudar as organizações a projetar e percorrer um caminho acelerado para uma adoção bem-sucedida da nuvem

- Oferece orientações e melhores práticas para ajudar as organizações a criar uma abordagem abrangente para a computação em nuvem em toda a organização e durante todo o ciclo de vida de TI para acelerar a adoção bem-sucedida da nuvem
- Está organizado em seis perspectivas
- As perspectivas consistem em conjuntos de recursos

Perspectivas:

- Foca nos recursos empresariais: negócios, pessoas e governança
- Foca nos recursos técnicos: plataforma, segurança e operações



## <a id="section-5" ></a> **5 - AWS Shared Responsibility Model**
The [AWS shared responsibility model](https://aws.amazon.com/compliance/shared-responsibility-model/) defines what you (as an AWS account holder/user) and AWS are responsible for when it comes to security and compliance.

Security and Compliance is a shared responsibility between AWS and the customer. This shared model can help relieve customer’s operational burdens as AWS operates, manages, and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates.

The customer assumes responsibility and management of the guest operating system (including updates and security patches), other associated application software as well as the configuration of the AWS provided security group firewall.

AWS are responsible for “Security of the Cloud” .

    AWS is responsible for protecting the infrastructure that runs all the services offered in the AWS Cloud.
    This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services.

Customers are responsible for “Security in the Cloud”.

    For EC2 this includes network level security (NACLs, security groups), operating system patches and updates, IAM user access management, and client and server-side data encryption.

The following diagram shows the split of responsibilities between AWS and the customer:


<img src="../images/extra/aws-shared-responsibility-model.jpeg" alt="aws-shared-responsibility-model" width=80% /> 


Inherited Controls – Controls which a customer fully inherits from AWS.

    Physical and Environmental controls.

Shared Controls – Controls which apply to both the infrastructure layer and customer layers, but in separate contexts or perspectives.

In the AWS shared security model, a shared control, AWS provides the requirements for the infrastructure and the customer must provide their own control implementation within their use of AWS services.

Examples  of shared controls include:

    Patch Management – AWS is responsible for patching and fixing flaws within the infrastructure, but customers are responsible for patching their guest OS and applications.
    Configuration Management – AWS maintains the configuration of its infrastructure devices, but a customer is responsible for configuring their own guest operating systems, databases, and applications.
    Awareness & Training – AWS trains AWS employees, but a customer must train their own employees.

Customer Specific – Controls which are solely the responsibility of the customer based on the application they are deploying within AWS services. .

Examples of customer specific controls include:

    Service and Communications Protection or Zone Security which may require a customer to route or zone data within specific security environments.