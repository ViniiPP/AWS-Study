## 📌 Amazon Elastic Block Store (EBS)
#### O Amazon Elastic Block Store (EBS) é um serviço de armazenamento de alto desempenho oferecido pela AWS para uso com Amazon Elastic Compute Cloud (EC2). Ele foi projetado para aplicativos que exigem armazenamento de baixa latência para ler e escrever dados em blocos.

#

### 🔹 1. Desempenho de Armazenamento
#### EBS fornece armazenamento em bloco de alto desempenho que pode ser anexado a uma instância EC2. Os volumes EBS são otimizados para cargas de trabalho que exigem operações de E/S de baixa latência, como bancos de dados e aplicações com alta demanda de I/O.

### 🔹 2. Durabilidade
#### O EBS é projetado para alta durabilidade. Os volumes EBS são automaticamente replicados dentro da **zona de disponibilidade** para proteger contra falhas de componentes, garantindo alta disponibilidade e resistência a falhas.

### 🔹 3. Tipos de Volume
#### O EBS oferece diversos tipos de volumes para atender diferentes necessidades de desempenho e armazenamento:

- SSD-backed (Alta performance)

    - **gp2** e **gp3** → Para cargas de trabalho transacionais de uso geral.

    - **io1** e **io2** → Para aplicações que exigem alto desempenho de IOPS.

- HDD-backed (Throughput intensivo)

    - **st1** → Para cargas de trabalho que exigem alto throughput sequencial.

    - **sc1** → Para armazenar grandes volumes de dados com baixa frequência de acesso.

### 🔹 4. Backup com Snapshots
#### O EBS permite a criação de snapshots (cópias) dos volumes, armazenados no **Amazon S3** para maior durabilidade.

- Esses snapshots podem ser usados para criar novos volumes ou aumentar o tamanho de um volume existente.

### 🔹 5. Criptografia
#### O EBS oferece suporte a volumes criptografados utilizando o **AWS Key Management Service (KMS).**

- Isso possibilita maior segurança e conformidade regulatória, permitindo gerenciamento de chaves de criptografia.

### 🔹 6. Integração com a AWS
#### O EBS possui integração com diversos serviços da AWS, como:

- 📊 **Amazon CloudWatch** → Para monitoramento de métricas.

- 🔐 **AWS IAM** → Para controle de acesso.

- 📅 **AWS Snapshot Scheduler** → Para automação de backups.


#

## 🏁 Conclusão
#### O Amazon EBS é uma solução de armazenamento em bloco altamente eficiente, essencial para muitas aplicações na AWS devido à sua durabilidade, flexibilidade e integração com outros serviços. 🚀

#

# 📌 Amazon Elastic File System (EFS)

O **Amazon Elastic File System (EFS)** é um serviço de **armazenamento de arquivos totalmente gerenciado** que facilita a configuração e o dimensionamento de sistemas de arquivos em nuvem na **AWS**. Ele foi projetado para ser **altamente disponível, durável e seguro**, podendo ser utilizado com uma ampla gama de serviços da AWS e aplicações **on-premise**.

---

## 🔹 1. Escalabilidade
O **EFS** é projetado para **escalar automaticamente** conforme o crescimento dos dados, indo de alguns **gigabytes a petabytes** sem a necessidade de provisionamento manual de armazenamento.

---

## 🔹 2. Alta Disponibilidade e Durabilidade
O **EFS** armazena automaticamente os arquivos em **múltiplos dispositivos** dentro e entre **várias zonas de disponibilidade (AZs)**, garantindo **alta disponibilidade** e **durabilidade** dos dados.

---

## 🔹 3. Compartilhamento de Arquivos
O **EFS** permite que **várias instâncias do Amazon EC2** acessem um **sistema de arquivos simultaneamente**, tornando-se ideal para cenários onde múltiplos servidores precisam compartilhar dados.

---

## 🔹 4. Integração com AWS
O **EFS** pode ser integrado com outros serviços da AWS, como:
- 📌 **AWS Backup** → Para backups automatizados.
- 🔐 **AWS IAM** → Para controle de acesso e gerenciamento de permissões.

---

## 🔹 5. Tipos de Armazenamento
O **EFS** oferece diferentes **classes de armazenamento** para otimização de custos:
- **Standard** → Para arquivos acessados com frequência.
- **Infrequent Access (IA)** → Para arquivos acessados com menor frequência, reduzindo custos de armazenamento.

---

## 🔹 6. Segurança
O **EFS** inclui suporte para **criptografia de dados** tanto **em repouso** quanto **em trânsito**, além da integração com o **AWS Key Management Service (KMS)** para gerenciamento de **chaves de criptografia**.

---

## 🏁 Conclusão
O **Amazon EFS** é uma **solução de armazenamento de arquivos escalável, altamente disponível e segura**, facilitando o **compartilhamento de arquivos** entre instâncias **EC2** e outros serviços AWS. 🚀


#

# 📌 Amazon FSx 

O **Amazon FSx** é um **serviço de armazenamento de arquivos totalmente gerenciado** da AWS, que facilita o lançamento e a execução de **sistemas de arquivos de terceiros**. Ele fornece um **conjunto rico de recursos** e **alta performance**, suportando atualmente dois tipos de sistemas de arquivos: **Windows File Server** para aplicações baseadas em Windows e **Lustre** para cargas de trabalho de computação intensiva.

---

## 🔹 1. FSx para Windows File Server
O **FSx para Windows File Server** fornece um sistema de arquivos **nativamente compatível com o Windows**, permitindo **migrar** aplicações baseadas em Windows para a AWS sem dificuldades.
- Construído sobre o **Windows Server**.
- Suporte a **deduplicação de dados**.
- **Criptografia de dados em repouso**.
- Acesso via **SMB (Server Message Block)** e **NFS (Network File System)**.

---

## 🔹 2. FSx para Lustre
O **FSx para Lustre** é um sistema de arquivos otimizado para cargas de trabalho de **computação intensiva**, como:
- 🔍 **Análise de Big Data**.
- 🤖 **Modelagem de Machine Learning**.
- 🎬 **Processamento de mídia**.
- Totalmente **gerenciado pela AWS**, simplificando a configuração e execução de sistemas **Lustre**.

---

## 🔹 3. Desempenho
O **Amazon FSx** foi projetado para oferecer **alta performance**, fornecendo:
- **Baixa latência**.
- **Altas taxas de transferência de dados**.
- Capacidade para suportar **aplicações exigentes**.

---

## 🔹 4. Compatibilidade e Integração
O **Amazon FSx** é totalmente **compatível com os sistemas de arquivos suportados**, permitindo que você utilize suas **ferramentas e aplicações existentes** sem modificações. Além disso, ele se **integra** com diversos serviços AWS, como:
- 📌 **AWS Backup** → Para backups automatizados.
- 📊 **Amazon CloudWatch** → Para monitoramento de métricas.
- 🔒 **AWS IAM** → Para controle de acesso seguro.

---

## 🔹 5. Segurança
O **Amazon FSx** oferece diversas funcionalidades de **segurança**, incluindo:
- Armazenamento de dados em **Amazon VPCs (Virtual Private Clouds)**.
- Suporte a **ACLs (Access Control Lists)** para o Windows File Server.
- **Criptografia de dados em repouso e em trânsito**.
- Integração com **AWS Key Management Service (KMS)** para **gerenciamento de chaves de criptografia**.

---

## 🏁 Conclusão
O **Amazon FSx** é um serviço **poderoso e flexível** que permite a execução de **sistemas de arquivos totalmente gerenciados** na AWS. Com suporte para **Windows File Server** e **Lustre**, ele oferece **alta performance, segurança avançada e integração profunda** com outros serviços da AWS. 🚀
