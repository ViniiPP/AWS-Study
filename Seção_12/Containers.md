# 📌 CONTAINERS 

Este documento abrange conceitos essenciais sobre **Docker**, **Amazon Elastic Container Registry (ECR)** e **Amazon Elastic Kubernetes Service (EKS)**, facilitando a implantação e gerenciamento de contêineres na AWS.

---

## 🐳 1. O que é Docker?

O **Docker** é uma plataforma que permite criar, empacotar e executar aplicações em contêineres. Ele simplifica o desenvolvimento e a implantação, garantindo que os aplicativos sejam executados de forma consistente em diferentes ambientes.

### 🔹 Vantagens do Docker:
✅ **Portabilidade** → Execute sua aplicação em qualquer ambiente que suporte Docker.
✅ **Isolamento** → Cada contêiner possui seu próprio ambiente independente.
✅ **Eficiência** → Utiliza menos recursos que máquinas virtuais (VMs).
✅ **Escalabilidade** → Facilita a replicação e escalabilidade de aplicações.

| 🏗️ Componente | 📌 Descrição |
|--------------|------------|
| **Imagem** | Modelo de um contêiner que inclui código, dependências e configurações. |
| **Contêiner** | Instância em execução de uma imagem Docker. |
| **Dockerfile** | Arquivo de configuração para criar imagens personalizadas. |
| **Registry** | Armazém para imagens de contêineres, como Docker Hub e AWS ECR. |

---

## 📦 2. Amazon Elastic Container Registry (Amazon ECR)

O **Amazon Elastic Container Registry (ECR)** é um **serviço gerenciado da AWS** para armazenar, gerenciar e implantar imagens de contêineres de forma segura e escalável.

### 🔹 Benefícios do ECR:
🔐 **Segurança** → Integração com IAM para controle de acesso a imagens.
🚀 **Alto desempenho** → Carregamento e recuperação rápida de imagens.
📊 **Gerenciamento eficiente** → Suporte a versionamento de imagens.
🛠️ **Integração com AWS** → Funciona perfeitamente com **ECS**, **EKS** e **Lambda**.

| 🔍 Recurso | 📌 Descrição |
|----------|------------|
| **Repositórios privados** | Armazene e compartilhe imagens de contêineres com controle de acesso. |
| **Escaneamento de imagens** | Verifique vulnerabilidades de segurança nas imagens armazenadas. |
| **Autenticação com IAM** | Controle permissões de usuários e serviços AWS. |
| **Suporte a multi-arquitetura** | Armazene imagens compatíveis com diferentes plataformas (x86, ARM). |

---

## ☸️ 3. Amazon Elastic Kubernetes Service (Amazon EKS)

O **Amazon EKS** é um serviço gerenciado que facilita a execução, escalabilidade e monitoramento de aplicações baseadas em **contêineres** usando o **Kubernetes**.

### 🔹 Características do EKS:
🛠️ **Gerenciamento automatizado** → Remove a complexidade da configuração e operação do Kubernetes.
🔄 **Compatibilidade total** → Funciona com qualquer aplicação Kubernetes padrão.
🔗 **Integração com AWS** → Trabalha com serviços como **RDS, S3, ELB e Lambda**.
🔒 **Segurança robusta** → Automatiza a rotação de chaves e protege dados.
📈 **Escalabilidade** → Ajusta recursos dinamicamente para lidar com variações de tráfego.
📊 **Monitoramento integrado** → Compatível com **CloudWatch** e **CloudTrail** para logs e métricas.

---

### 🐳 O que é Kubernetes?

**O Kubernetes (K8s)** é um sistema open-source para orquestração de contêineres, originalmente desenvolvido pelo Google e agora mantido pela Cloud Native Computing Foundation (CNCF). Ele automatiza a implantação, o escalonamento e a operação de aplicações em contêineres.

---

## 🏁 Conclusão

Com **Docker**, **Amazon ECR** e **Amazon EKS**, você pode criar, armazenar e escalar aplicações baseadas em contêineres na **AWS** com facilidade e segurança. 🚀
