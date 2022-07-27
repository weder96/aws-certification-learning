<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]

[1]: https://github.com/weder96/aws-certification-learning

# Módulo 8: Bancos de dados

## Conteúdo
1. <a href="#section-1"> Casos de uso para diferentes tipos de banco de dados </a>
2. <a href="#section-2"> Amazon Relational Database Service (RDS) </a>
3. <a href="#section-3"> Amazon DynamoDB </a>
4. <a href="#section-4"> Amazon RedShift </a>
5. <a href="#section-5"> Amazon ElastiCache </a>
6. <a href="#section-6"> Amazon EMR </a>
7. <a href="#section-7"> Amazon (RDS) Pricing </a>
8. <a href="#section-8"> Amazon (RDS) Multiple Availability Zones (A-Z) </a>
9. <a href="#section-9"> Enable automatic patching for the instances using the Amazon RDS console </a>
10. <a href="#section-10"> Restoring a DB instance to a specified time </a>

***************************************************************************************************************
## <a id="section-1" ></a> **1 - Use Cases For Different Database Types**

A tabela abaixo fornece orientação sobre os casos de uso típicos para vários serviços de banco de dados/armazenamento de dados da AWS:

### **Banco de dados no EC2**
- Controle total sobre instância e banco de dados
- DB preferencial não disponível no RDS


### **Amazon RDS**
- Precisa de banco de dados relacional tradicional para OLTP
- Seus dados estão bem formados e estruturados
- Aplicativos existentes que requerem RDBMS

### **Amazon DynamoDB**
- Dados do par nome/valor
- Estrutura de dados imprevisível
- Desempenho na memória com persistência
- Altas necessidades de E/S
- Requer dimensionamento dinâmico


### **Amazon RedShift**
- Data warehouse para grandes volumes de dados agregados
- Principalmente cargas de trabalho OLAP

### **Amazon Neptuno**
- Relacionamentos entre objetos são de alto valor

### **Amazon ElastiCache**
- Armazenamento temporário rápido para pequenas quantidades de dados
- Dados altamente voláteis (não persistentes)

### **Amazon S3**
- Grandes objetos binários (BLOBs)
- Sites estáticos

Agora abordaremos vários desses tipos de banco de dados que podem surgir no exame.

***************************************************************************************************************
## <a id="section-2" ></a> **2 - Amazon Relational Database Service (RDS)**
O Amazon Relational Database Service (Amazon RDS) é um serviço gerenciado que facilita a configuração, operação e dimensionamento de um banco de dados relacional na nuvem.

Os bancos de dados relacionais são conhecidos como bancos de dados SQL (Structured Query Language).

Os bancos de dados não relacionais são conhecidos como bancos de dados NoSQL.

RDS é um tipo de banco de dados OLTP (Online Transaction Processing).

### **Recursos e benefícios do RDS:**
- Tipo de banco de dados SQL.
- Pode ser usado para realizar consultas e junções complexas.
- Fácil de configurar, altamente disponível, tolerante a falhas e escalável.
- Usado quando os dados são claramente definidos.
- Casos de uso comuns incluem lojas online e sistemas bancários.


### **O Amazon RDS oferece suporte aos seguintes mecanismos de banco de dados:**
- SQL Server.
- Oracle.
- MySQL Serber.
- PostgreSQL.
- Aurora.
- MariaDB.

**Aurora é o banco de dados proprietário da Amazon**.

O RDS é um serviço totalmente gerenciado e você não tem acesso à instância do EC2 subjacente (sem acesso root).

### **O serviço RDS inclui o seguinte:**
- Segurança e patching das instâncias de banco de dados.
- Backup automatizado para as instâncias de banco de dados.
- Atualizações de software para o mecanismo de banco de dados.
- Fácil dimensionamento para armazenamento e computação.
- Opção Multi-AZ com replicação síncrona.
- Failover automático para opção Multi-AZ.
- Opção de réplicas de leitura para cargas de trabalho pesadas de leitura.
- Uma instância de banco de dados é um ambiente de banco de dados na nuvem com os recursos de computação e armazenamento que você especifica.

### **Criptografia:**

- Você pode criptografar suas instâncias e snapshots do Amazon RDS em repouso ativando a opção de criptografia para sua instância de banco de dados do Amazon RDS.
- A criptografia em repouso é compatível com todos os tipos de banco de dados e usa o AWS KMS.
- Você não pode criptografar um banco de dados existente, você precisa criar um instantâneo, copiá-lo, criptografar a cópia e construir um banco de dados criptografado a partir do instantâneo.

### **Grupos de sub-redes de banco de dados:**

- Um grupo de sub-redes de banco de dados é uma coleção de sub-redes (normalmente privadas) que você cria em uma VPC e designa para suas instâncias de banco de dados.
- Cada grupo de sub-redes de banco de dados deve ter sub-redes em pelo menos duas zonas de disponibilidade em cada região.
- Recomenda-se configurar um grupo de sub-redes com sub-redes em cada AZ (mesmo para instâncias independentes).

### **Cobrança da AWS por:**
- Horas da instância de banco de dados (horas parciais são cobradas como horas completas).
- Armazenamento GB/mês.
- Solicitações de E/S/mês – para armazenamento magnético.
- IOPS provisionado/mês – para SSD IOPS provisionado por RDS.
- Transferência de dados de saída.
- Armazenamento de backup (backups de banco de dados e instantâneos manuais).


### **Escalabilidade:**
- Você só pode aumentar o RDS (computação e armazenamento).
- Você não pode diminuir o armazenamento alocado para uma instância do RDS.
- Você pode dimensionar o armazenamento e alterar o tipo de armazenamento para todos os mecanismos de banco de dados, exceto MS SQL.

### **O RDS fornece multi-AZ para recuperação de desastres que oferece tolerância a falhas em zonas de disponibilidade:**
- O RDS Multi-AZ cria uma réplica em outra AZ e replica de forma síncrona para ela (somente DR).
- Há uma opção para escolher multi-AZ durante o assistente de inicialização.
- A AWS recomenda o uso de armazenamento IOPS provisionado para instâncias de banco de dados RDS multi-AZ.
- Cada AZ é executada em sua própria infraestrutura fisicamente distinta e independente e é projetada para ser altamente confiável.
- Você não pode escolher qual AZ na região será escolhida para criar a instância de banco de dados em espera.

### **Réplicas de leitura – fornecem desempenho aprimorado para leituras:**
- As réplicas de leitura são usadas para bancos de dados pesados ​​de leitura e a replicação é assíncrona.
- As réplicas de leitura são para compartilhamento e descarregamento de carga de trabalho.
- As réplicas de leitura fornecem DR somente leitura.
- As réplicas de leitura são criadas a partir de um instantâneo da instância mestre.
- Deve ter backups automatizados habilitados no primário (período de retenção > 0).

***************************************************************************************************************
## <a id="section-3" ></a> **3 - Amazon DynamoDB**
O Amazon DynamoDB é um serviço de banco de dados NoSQL totalmente gerenciado que oferece desempenho rápido e previsível com escalabilidade perfeita.

## **Recursos e benefícios do Dynamo DB:**
- Tipo de banco de dados NoSQL (não relacional).
- Rápido, altamente disponível e totalmente gerenciado.
- Usado quando os dados são fluidos e podem mudar.
- Casos de uso comuns incluem redes sociais e análise da web.

O dimensionamento por botão significa que você pode dimensionar o banco de dados a qualquer momento sem incorrer em tempo de inatividade.

Baseado em SSD e usa indexação limitada em atributos para desempenho.

O DynamoDB é um serviço da Web que usa HTTP sobre SSL (HTTPS) como transporte e JSON como formato de serialização de mensagens.

O Amazon DynamoDB armazena três réplicas distribuídas geograficamente de cada tabela para permitir alta disponibilidade e durabilidade dos dados.

Os dados são replicados de forma síncrona em 3 instalações (AZs) em uma região.

## **A replicação entre regiões permite replicar entre regiões:**
- As tabelas globais do Amazon DynamoDB fornecem uma solução totalmente gerenciada para implantar um banco de dados multirregional e multimestre.
- Ao criar uma tabela global, você especifica as regiões da AWS em que deseja que a tabela esteja disponível.
- O DynamoDB executa todas as tarefas necessárias para criar tabelas idênticas nessas regiões e propagar alterações de dados contínuas para todas elas.


Fornece baixa latência de leitura e gravação.

Aumente ou diminua o armazenamento e a taxa de transferência conforme necessário, sem alterações de código ou tempo de inatividade.

O DynamoDB não tem esquema.

O DynamoDB pode ser usado para armazenar o estado da sessão.

Fornece dois modelos de leitura.

## **Leituras eventualmente consistentes (Padrão):**
- A opção de consistência eventual maximiza seu rendimento de leitura (melhor desempenho de leitura).
- Uma leitura eventualmente consistente pode não refletir os resultados de uma gravação concluída recentemente.
- Consistência em todas as cópias alcançadas em 1 segundo.

## **Leituras fortemente consistentes:**
- Uma leitura fortemente consistente retorna um resultado que reflete todas as gravações que receberam uma resposta bem-sucedida antes da leitura (consistência mais rápida).

O Amazon DynamoDB Accelerator (DAX) é um cache de memória totalmente gerenciado e altamente disponível para o DynamoDB que oferece uma melhoria de desempenho de até 10 vezes – de milissegundos a microssegundos – mesmo com milhões de solicitações por segundo.

***************************************************************************************************************
## <a id="section-4" ></a> **4 - Amazon RedShift**

O Amazon Redshift é um data warehouse rápido e totalmente gerenciado que torna simples e econômica a análise de todos os seus dados usando SQL padrão e ferramentas de Business Intelligence (BI) existentes.

RedShift é um data warehouse baseado em SQL usado para aplicativos de análise.

RedShift é um banco de dados relacional usado para casos de uso de OLAP (Online Analytics Processing).

O RedShift é usado para executar consultas analíticas complexas em petabytes de dados estruturados, usando otimização de consulta sofisticada, armazenamento colunar em discos locais de alto desempenho e execução de consulta maciçamente paralela.

O RedShift é ideal para processar grandes quantidades de dados para inteligência de negócios.

RedShift é 10x mais rápido que um banco de dados SQL tradicional.

## **RedShift usa armazenamento de dados colunar:**
- Os dados são armazenados sequencialmente em colunas em vez de linhas.
- O banco de dados baseado em colunas é ideal para armazenamento e análise de dados.
- Requer menos I/Os, o que aumenta muito o desempenho.

## **RedShift fornece compactação avançada:**
- Os dados são armazenados sequencialmente em colunas, o que permite um desempenho muito melhor e menos espaço de armazenamento.
- RedShift seleciona automaticamente o esquema de compressão.

O RedShift usa replicação e backups contínuos para aumentar a disponibilidade e a durabilidade e pode se recuperar automaticamente de falhas de componentes e nós.

## **RedShift sempre mantém três cópias de seus dados:**
- O original.
- Uma réplica em nós de computação (dentro do cluster).
- Uma cópia de backup no S3.

## **RedShift fornece backups contínuos/incrementais:**
- Várias cópias dentro de um cluster.
- Backups contínuos e incrementais para S3.
- Backups contínuos e incrementais entre regiões.
- Restauração de streaming.

## **RedShift fornece tolerância a falhas para as seguintes falhas:**
- Falhas de disco.
- Falhas de nós.
- Falhas de rede.
- Desastres em nível AZ/região.

***************************************************************************************************************
## <a id="section-5" ></a> **5 - Amazon ElastiCache**
O ElastiCache é um serviço da Web que facilita a implantação e a execução de nós de servidor compatíveis com o protocolo Memcached ou Redis na nuvem.

O cache na memória fornecido pelo ElastiCache pode ser usado para melhorar significativamente a latência e a taxa de transferência para muitas cargas de trabalho de aplicativos de leitura intensa ou cargas de trabalho de computação intensiva.

Melhor para cenários em que a carga do banco de dados é baseada em transações OLAP (Online Analytics Processing).

## **A tabela a seguir descreve alguns casos de uso típicos do ElastiCache:**
### **Web session store**
- Em casos com servidores da Web com balanceamento de carga, armazene as informações da sessão da Web no Redis para que, se um servidor for perdido, as informações da sessão não sejam perdidas e outro servidor da Web possa recuperá-lo

### **Database caching**
- Use o Memcached na frente do AWS RDS para armazenar em cache consultas populares para descarregar o trabalho do RDS e retornar resultados mais rapidamente aos usuários

### **Leaderboards**
- Use o Redis para fornecer uma tabela de classificação ao vivo para milhões de usuários do seu aplicativo móvel

### **Streaming data dashboards**
- Fornecer um ponto de aterrissagem para transmitir dados do sensor no chão de fábrica, fornecendo exibições de painel ao vivo em tempo real


Os nós do ElastiCache EC2 não podem ser acessados ​​pela Internet nem por instâncias do EC2 em outras VPCs.

Também podem ser instâncias sob demanda ou reservadas (mas não instâncias spot).

O ElastiCache pode ser usado para armazenar o estado da sessão.

## **Existem dois tipos de mecanismo ElastiCache:**
- **Memcached** – modelo mais simples, pode executar nós grandes com vários núcleos/threads, pode ser dimensionado para dentro e para fora, pode armazenar em cache objetos como bancos de dados.
- **Redis** – modelo complexo, suporta criptografia, replicação mestre/escravo, cross AZ (HA), failover automático e backup/restauração.

***************************************************************************************************************
## <a id="section-6" ></a> **6 - Amazon EMR**

O **Amazon EMR** é um serviço da web que permite que empresas, pesquisadores, analistas de dados e desenvolvedores processem grandes quantidades de dados de maneira fácil e econômica.

O EMR utiliza uma estrutura do Hadoop hospedada em execução no Amazon EC2 e no Amazon S3.

Estrutura gerenciada do Hadoop para processar grandes quantidades de dados.

Também suporta **Apache Spark, HBase, Presto e Flink**.

Mais comumente usado para análise de log, análise financeira ou atividades de extração, tradução e carregamento (ETL).



## <a id="section-7" ></a> **7 - Amazon (RDS) Pricing**

[Amazon (RDS) Pricing](https://aws.amazon.com/rds/pricing/?nc1=h_ls)


Amazon Relational Database Service (Amazon RDS) is a managed, highly available, and secure database service that makes it simple to set up, operate, and scale databases in the cloud. Amazon RDS is free to try and you pay only for what you use with no minimum fees. You can pay for Amazon RDS using On-Demand or Reserved Instances. Estimate your monthly bill using the AWS Pricing Calculator.

Amazon RDS provides a selection of instance types optimized to fit different relational database use cases. Select one of the Amazon RDS database engines below to view pricing. See Previous Generation Instances for previous instance pricing not listed here.

For Amazon RDS feature-level pricing, see RDS Performance Insights and RDS Proxy pricing pages.

As part of the AWS Free Tier, Amazon RDS helps new AWS customers get started for free with a managed database service in the cloud. Each calendar month, the 

**Amazon RDS Free Tier allows you to use:**
- 750 hours of Amazon RDS Single-AZ db.t2.micro, db.t3.micro, and db.t4g.micro Instances usage running MySQL, MariaDB, PostgreSQL databases each month. If running more than one instance, usage is aggregated across instance classes.
- 750 hours of Amazon RDS Single-AZ db.t2.micro Instance usage running Oracle BYOL or SQL Server (running SQL Server Express Edition). Oracle BYOL db.t3.micro  Single-AZ Instance usage is also included as part of the Amazon RDS free tier. If running both a db.t2.micro Single-AZ Instance and a db.t3.micro Single-AZ Instance on Oracle BYOL, usage is aggregated across Instance classes.
- 20 GB of General Purpose (SSD) DB storage.
- 20 GB of storage for your automated database backups and any user-initiated DB Snapshots.


With Amazon RDS you are charged for the type and size of database, the uptime, any additional storage of backup (above the DB size), requests, deployment type (e.g. you pay for multi AZ), and data transfer outbound.


***************************************************************************************************************
## <a id="section-8" ></a> **8 - Amazon (RDS) Multiple Availability Zones (A-Z)**
[Amazon (RDS) Multiple Availability Zones](https://aws.amazon.com/rds/features/multi-az/)


Multi AZ provides a mechanism to failover the RDS database to another synchronously replicated copy in the event of the failure of an AZ. The endpoint address for the RDS instances gets remapped to the standby instance as can be seen in the image below:

<img src="../images/extra/rds_multiply_a_z.png" alt="rds_multiply_a_z" width=80% />



## <a id="section-9" ></a> **9 - Enable automatic patching for the instances using the Amazon RDS console**

[Enable automatic patching](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_UpgradeDBInstance.Maintenance.html)

Periodically, Amazon RDS performs maintenance on Amazon RDS resources. Maintenance most often involves updates to the DB instance's underlying hardware, underlying operating system (OS), or database engine version. Updates to the operating system most often occur for security issues and should be done as soon as possible.

Required patching is automatically scheduled only for patches that are related to security and instance reliability. Such patching occurs infrequently (typically once every few months) and seldom requires more than a fraction of your maintenance window.



## <a id="section-10" ></a> **10 - Restoring a DB instance to a specified time**

[Restoring a DB instance](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_PIT.html)

You can restore an Amazon RDS database instance to a specific point in time with a granularity of 5 minutes. Amazon RDS uses transaction logs which it uploads to Amazon S3 to do this.

**To restore a DB instance to a specified time in aws console:**
 - Restore to point in time.
 - The Restore to point in time window appears.


