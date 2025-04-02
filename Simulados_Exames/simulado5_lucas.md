# QUESTÕES PARA REVISÕES DENTRO DO SIMULADO 4 DA UDEMY 📊💡

#### **1 - Uma empresa quer alocar custos de serviços por departamento, aplicar taxas personalizadas e distribuir créditos conforme o consumo compartilhado da AWS.**

**Qual serviço permite exibir custos de forma personalizada e suporta fluxos de trabalho de cobrança e relatórios?**

*R: **AWS Billing Conductor** (permite personalizar a alocação de custos por departamento, aplicar taxas específicas e distribuir créditos conforme o consumo.)*

---

#### **2 - Um time de desenvolvimento deseja supervisionar as atividades de projetos desde a concepção até a entrega do software na plataforma, além de utilizar modelos pré-definidos de projetos na linguagem de programação que utilizam.**

**Que serviço possibilita esse nível de facilitação?**

*R: AWS CodeStar*

**Explicação:** O AWS CodeStar é um serviço da Amazon Web Services (AWS) projetado para simplificar e acelerar o processo de desenvolvimento de software. Ele facilita a integração de várias ferramentas essenciais para o desenvolvimento, como ambientes de desenvolvimento integrado (IDEs), pipelines de integração contínua/entrega contínua (CI/CD) e ferramentas de gerenciamento de projetos. Com o CodeStar, os desenvolvedores podem configurar rapidamente um ambiente de desenvolvimento completo, permitindo que eles se concentrem na criação de software em vez de lidar com a configuração e integração de várias ferramentas.

---

#### **3 - Como o AWS IoT Core utiliza múltiplos mecanismos de segurança para assegurar a integridade e confidencialidade das comunicações entre dispositivos IoT e a nuvem?**

*R: O AWS IoT Core utiliza certificados de dispositivo para autenticação mútua, criptografia TLS para proteger dados em trânsito e políticas de acesso baseadas em identidade para controlar o acesso e garantir a segurança das comunicações entre dispositivos e a nuvem.*

---

#### **4 - Você precisa permitir que os seus clientes acessem a sua aplicação web através de um domínio amigável com o nome da sua empresa. Como isso pode ser implementado?**

*R: Com o registro no Route53*

**Explicação: Para permitir que seus clientes acessem sua aplicação web através de um domínio amigável, registre um nome de domínio e configure o DNS usando o Amazon Route 53. O Route 53 permite associar seu domínio personalizado ao endpoint da sua aplicação. Isso direciona o tráfego para sua aplicação web usando um endereço fácil de lembrar.** 

---

#### **5 - Uma organização pretende disponibilizar aplicativos SaaS e ambientes de trabalho virtual para seus usuários finais.**

**Como o AWS AppStream 2.0 pode ser uma contribuição significativa nesse contexto?**

*R: Fornecendo streaming de aplicativos.*

**Explicação: O AWS AppStream 2.0 é um serviço projetado para fornecer streaming de aplicativos na nuvem. Ele permite a execução de aplicativos de desktop na nuvem, transmitindo a saída para dispositivos dos usuários, garantindo uma experiência consistente em diversos dispositivos e sistemas operacionais.** 

---

#### **6 -Para manter uma arquitetura híbrida, uma empresa precisa integrar sistemas legados que utilizam serviços tradicionais de mensagens no ambiente on-premises com serviços desacoplados na AWS.**

**Qual serviço de mensageria permite essa integração?**

*R: Amazon MQ*

**Explicação:** O Amazon MQ é um serviço gerenciado de mensagens baseado no Apache ActiveMQ, ideal para integrar sistemas on-premises com a AWS. Ele suporta protocolos padrão da indústria, como MQTT e AMQP, facilitando a troca de mensagens entre diferentes sistemas. Essa flexibilidade torna o Amazon MQ a escolha mais adequada para integrar sistemas de mensagens tradicionais com serviços na nuvem da AWS.

---

#### **7 - Uma empresa está desenvolvendo uma plataforma de Machine Learning e requer a transformação de dados provenientes de arquivos de diversas fontes antes de serem analisados.**

**Quais processos precisam ser implementados para alcançar esse objetivo?**

*R: extração, transformação e carregamento de dados com o AWS Glue*

**Explicação: O AWS Glue é um serviço gerenciado para integração de dados, facilitando o processo de ETL (Extração, Transformação e Carga) antes de serem consumidos por outros serviços.** 

---

#### **8 - Uma empresa tem uma extensa base de dados, tanto estruturados quanto não estruturados, e busca processá-la por meio de ferramentas de Big Data.**

**Qual serviço da AWS você recomendaria para essa finalidade?**

*R: Amazon EMR*

**Explicação: O Amazon EMR (Elastic MapReduce) é uma solução de Big Data em nuvem líder no setor para processamento de dados em grande escala, análise interativa e machine learning.** 

---

#### **9 - O time de desenvolvedores da sua empresa criou uma aplicação em Java e gostaria de disponibilizá-la na AWS. Uma vez que o time não possua muito conhecimento sobre resiliência, balanceadores de carga, monitoramento e outras questões de infraestrutura, qual serviço poderá ajudá-los?**

*R: AWS ElasticBeanStalk*

**Explicação:** Com o AWS Elastic Beanstalk, é possível implantar e gerenciar rapidamente aplicações na Nuvem AWS sem precisar se preocupar com a infraestrutura que executa essas aplicações. O AWS Elastic Beanstalk reduz a complexidade do gerenciamento sem restringir as opções ou o controle. Basta fazer upload da sua aplicação e o AWS Elastic Beanstalk automaticamente gerencia os detalhes de provisionamento de capacidade, balanceamento de carga, escalabilidade e monitoramento da integridade da aplicação.

---

#### **10 - Considerando o uso de tags associadas aos serviços e recursos da AWS, qual das seguintes descrições NÃO representa uma função aplicável para tags?**

*R: Gerenciamento de permissões e controle de acesso (Tags não gerenciam permissões nem controlam o acesso diretamente.)*

---

#### **11 - A infraestrutura global da AWS é composta por Regiões, Zonas de Disponibilidade e Redes de Borda.**

**Qual destes componentes é utilizado para alocar os serviços de cache ofertados pelo CloudFront e pelo API Gateway?**

*R: Redes de Borda*

**Explicação:** Redes de borda, ou "edge locations", são projetadas para aproximar serviços e dados dos usuários finais, reduzindo a latência e melhorando a performance das aplicações. Elas posicionam recursos e servidores em locais geograficamente distribuídos, próximos aos pontos de acesso dos usuários.

---

#### **12 - Uma empresa mantém arquivos contendo dados financeiros em um bucket do S3. Como é viável consultar informações nestes arquivos utilizando a linguagem SQL?**

*R: Com o Athena*

**Explicação:** O Amazon Athena é um serviço de análise interativo que permite consultar e analisar grandes volumes de dados armazenados no Amazon S3 usando a linguagem SQL padrão.

---

#### **13 - Durante uma migração de banco de dados para a AWS, a equipe encarregada identificou a necessidade de transferir dados de um banco Oracle on-premises para um banco Oracle no RDS.**

**Como esse procedimento pode ser executado?**

*R: Implementando o AWS DMS*

**Explicação:** O AWS DMS - Database Migration Service é um serviço utilzado para migrar dados de bancos de dados on-premises, para uma instância de banco de dados do Amazon Relational Database Service (Amazon RDS) em qualquer um dos mecanismos de bancos de dados disponíveis no serviço, como o Oracle.

---

#### **14 - Sua empresa precisa criar um chat interativo de alta qualidade com uma central de atendimento "omnichannel" para oferecer suporte aos seus clientes de qualquer lugar do mundo.**

**Com qual serviço isso é possível?**

*R: Amazon Connect*

**Explicação:** Com o Amazon Connect, você pode configurar uma central de contato em questão de minutos, e ela pode ser dimensionada para oferecer suporte a milhões de clientes.

---

#### **15 - Com o objetivo de reduzir a carga de trabalho para os desenvolvedores de microsserviços, uma startup deseja implementar contêineres sem depender de instâncias EC2 como infraestrutura base. Como isso pode ser realizado?**

*R: Com o uso de computação sem servidor com o Fargate*

---

#### **16 - Um sistema de comércio eletrônico utiliza microsserviços independentes e desacoplados, permitindo escalabilidade independente para cada um deles. Como os microsserviços podem ser integrados e comunicar entre si de maneira eficaz?**

*R: Com filas SQS*

**Explicação:** O Amazon Simple Queue Service (SQS) é um serviço de filas de mensagens gerenciado que permite o desacoplamento e a escalabilidade de microsserviços, sistemas distribuídos e aplicações sem servidor.

---

#### **17 - A área de Business Intelligence (BI) de uma organização tem a necessidade de fazer o cruzamento de dados estruturados e semi-estruturados para produzir insights para uma campanha de vendas. Que serviço pode ser empregado para essa finalidade?**

*R: Amazon RedShift*

