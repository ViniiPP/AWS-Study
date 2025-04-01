# QUESTÕES PARA REVISÕES DENTRO DO SIMULADO 3 DA UDEMY 📊💡

#### **1 - Qual das seguintes opções NÃO está associada ao Amazon Cognito?**

*R: permite autenticação de APIs pela linha de comando*

---

#### **2 - Quais são os 6 pilares do AWS Well-Architected Framework?**

*R: Excelencia Operacional, Segurança, Confiabilidade, Eficiência e Desempenho, otimização de custos e sustentabilidade.*

---

#### **3 - Qual é a classe de armazenamento do S3 que pode diminuir os custos, à medida que move os objetos automaticamente entre camadas, de acordo com a frequência de uso?**

*R: S3 Intelligent-Tiering*

**Explicação:** O S3 Intelligent-Tiering é uma classe de armazenamento do Amazon S3 que otimiza automaticamente os custos ao mover dados entre camadas de acesso frequente e infrequente com base na frequência de acesso dos objetos, sem impacto na performance.

---

#### **4 - O departamento de marketing de uma empresa está elaborando uma campanha com duração de 12 meses. Antecipadamente, prevê-se um aumento no número de clientes no site, exigindo a adição de mais 3 instâncias EC2 para atender à demanda ao longo desse período. Qual tipo de instância apresentaria um custo mais vantajoso para esse cenário?**

*R: Reserved*

**Explicação:** Nestes cenários com previsão de tempo de uso e processamento, o uso de instâncias reservadas gera uma economia de até 72% em comparação ao modelo sob demanda (on demand) para períodos de 1 a 3 anos.

---

#### **5 - Qual é a maneira mais fácil de lançar rapidamente milhares de contêineres em uma ampla variedade de opções de computação da AWS, usando o seu CI/CD e ferramentas de automação de sua preferência?**

*R: Com o Amazon ECS*

**Explicação:** oferece integração com várias ferramentas de CI/CD, permitindo a orquestração eficiente e escalável de contêineres em serviços como EC2 e AWS Fargate.

**EXTRA:** É TAMBÉM um serviço de orquestração de containers da AWS que simplifica a implantação, gerenciamento e escalabilidade de aplicativos baseados em containers.

---

#### **6 - Qual serviço da AWS pode ser implantado para armazenar em cache esses resultados e reduzir os acessos ao banco de dados?**

*R: Amazon ElasticCache*

---

#### **7 - Uma empresa pretende incorporar testes automatizados em seu fluxo de desenvolvimento. Qual serviço da AWS pode ser empregado para atender a essa necessidade?**

*R: AWS CodeBuild*

**Explicação:** É um serviço gerenciado de compilação e teste contínuos que automatiza a criação, teste e validação de código-fonte.

---

#### **8 - Qual serviço oferece um grupo de ferramentas que podem ser usadas em conjunto ou individualmente para permitir que desenvolvedores de front-end da web e de dispositivos móveis criem aplicações seguras e escaláveis full-stack, com tecnologia desenvolvida pela AWS?**

*R: AWS Amplify*

**Explicação:** O AWS Amplify oferece um conjunto de ferramentas que ajudam desenvolvedores de front-end a criar aplicações web e móveis seguras e escaláveis utilizando tecnologia da AWS.

---

#### **9 - Uma startup deseja disponibilizar uma aplicação no endereço www.simuladoudemy.com. Qual serviço pode ser empregado para criar esse domínio?**

*R: **Route 53**   - é utilizado para registrar e gerenciar domínios, permitindo criar e configurar o domínio*

---

#### **10 - Uma organização pretende aprimorar a segurança de seus recursos na AWS, buscando uma solução que facilite o provisionamento, gerenciamento e implantação de certificados Secure Sockets Layer (SSL)/Transport Layer Security (TLS) a serem empregados nos serviços da AWS e nos recursos internos conectados.**

**Qual serviço pode ser empregado para atender a essa finalidade?**

*R: AWS Certificate Manager*

---

#### **11 - Usuários que utilizam aplicações em nuvem sem se preocuparem com sua construção e implementação estão usando qual tipo de nuvem?**

*R: SaaS*

**BREVE EXPLICAÇÃO:** 
- **BaaS**: Fornece backend pronto para apps (ex: Firebase).
- **IaaS**: Oferece infraestrutura de servidores e redes (ex: Amazon EC2).
- **PaaS**: Plataforma para desenvolver e hospedar apps (ex: Google App Engine).
- **SaaS**: Software acessível pela internet sem necessidade de instalação (ex: Gmail).

---

#### **12 - Qual plano de suporte oferece um gerente técnico de conta para monitorar o ambiente proativamente e sugerir melhorias para otimização dos serviços?**

*R: Enterprise*

---

#### **13 - Qual recurso da AWS permite o gerenciamento dos serviços através de uma interface web?**

*R: AWS Mangement Console*

---

#### **14 - Um objeto do S3 é composto por quais componentes?(selecione 3 alternativas)**

*R: Identificador exclusivo (chave), METADADOS E DADOS*

---

#### **15 - Uma empresa está desenvolvendo um aplicativo para enviar e-mails de aniversário para mais de 1000 clientes diariamente.**

**Qual serviço da AWS pode ser integrado a qualquer aplicativo para atender a esse requisito?**

*R: Amazon Simple Email Service (SES)*

---

#### **16 - Qual serviço de armazenamento de dados da Amazon é empregado pelas áreas de Business Intelligence, possibilitando a análise de dados estruturados e semi-estruturados para gerar insights para o negócio?**

*R: Amazon RedShift*

---

#### **17 - Qual é o serviço que, seguindo as melhores práticas, pode ser usado para identificar vulnerabilidades e desvios de segurança em aplicativos antes de serem implantados ou durante sua execução em ambiente de produção?**

*R: AWS Inspector*

---

#### **18 - Após avaliar diversos cenários para infraestrutura, uma empresa optou por não autorizar o uso de computação compartilhada. No entanto, ela busca uma solução na AWS que preserve as características de simplicidade, agilidade e elasticidade, enquanto utiliza servidores físicos dedicados.**

**Qual serviço atende a essa necessidade?**

*R: Hosts dedicados*

---

#### **19 - Qual ação é de responsabilidade dos clientes quando é preciso garantir que dados em volumes EBS  estejam seguros e com seus backups realizados?**

*R: Criar snapshots dos volumes EBS e replicá-los em outras regiões*

---

#### **20 - Qual serviço utiliza Inteligência Artificial e analisa dados gerados por eventos de diversos serviços e armazenados no S3, evitando que atividades maliciosas sejam realizadas?**

*R: AWS GuardDuty* 

---

#### MENÇÃO HONROSA A **AWS ElasticBeanStalk**

- O AWS Elastic Beanstalk é o serviço que simplifica a gestão da infraestrutura, balanceamento de carga, monitoramento e implantação de aplicações. Ele permite que desenvolvedores se concentrem no código e oferece suporte a várias linguagens de programação como .Net, Java, PHP, Node.js, Python, Ruby e Go.
