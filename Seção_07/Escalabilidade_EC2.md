# 📌 Amazon Auto Scaling

O **Amazon Auto Scaling** é um **serviço da AWS** que permite o **dimensionamento automático** de recursos para manter a **performance** e a **disponibilidade** de suas aplicações. Ele monitora continuamente suas aplicações e ajusta a capacidade para manter um desempenho **estável e previsível** ao **menor custo possível**.

---

## 🔹 1. Dimensionamento Automático
O **Auto Scaling** permite definir **políticas de dimensionamento** que ajustam automaticamente a **capacidade de recursos** com base em **condições predefinidas**.
- 🚀 Dimensiona automaticamente o número de **instâncias EC2** conforme a demanda de tráfego.
- ⚙️ Ajusta a capacidade de forma **inteligente e automatizada**.

---

## 🔹 2. Otimização de Custo e Performance
O **Auto Scaling** ajuda a melhorar a **disponibilidade** e reduzir **custos**.
- 📈 **Aumenta** os recursos quando a demanda sobe.
- 📉 **Diminui** os recursos quando a demanda cai, evitando desperdícios.

---

## 🔹 3. Balanceamento de Carga
O **Auto Scaling** pode ser utilizado com o **Elastic Load Balancing (ELB)** para:
- 🔄 Distribuir **tráfego de aplicações** entre várias instâncias **EC2**.
- ✅ Melhorar a **disponibilidade** e **tolerância a falhas**.

---

## 🔹 4. Saúde da Aplicação
O **Auto Scaling** realiza **verificações de saúde** nas instâncias **EC2** e:
- 🔍 Substitui **automaticamente** instâncias que não estão saudáveis.
- 🛡️ Mantém a **estabilidade** e **resiliência** da aplicação.

---

## 🔹 5. Integração com AWS
O **Auto Scaling** se integra com vários serviços da AWS, incluindo:
- 📊 **Amazon CloudWatch** → Para monitoramento e métricas.
- 🔔 **Amazon SNS** → Para notificações e alertas.
- 📦 **AWS CloudFormation** → Para provisionamento automatizado.

---

## 🔹 6. Flexibilidade
O **Auto Scaling** pode dimensionar **diferentes tipos de recursos**, não apenas **instâncias EC2**.
- 🗄️ **Amazon DynamoDB** → Dimensionamento de tabelas.
- 💾 **Amazon Aurora** → Ajuste de capacidade do banco de dados.
- 🚢 **Amazon ECS** → Escalabilidade de containers.
- 🛠️ **Amazon RDS** → Ajuste automático de instâncias de banco de dados.

---

## 🏁 Conclusão
O **Amazon Auto Scaling** é um serviço **essencial** para garantir a **performance, disponibilidade e otimização de custos** das suas aplicações na AWS. Ele assegura que você tenha o **número certo de recursos** no momento exato em que precisa. 🚀

#

# 📌 Elastic Load Balancing (ELB)

O **Elastic Load Balancing (ELB)** é um **serviço da AWS** que **distribui automaticamente** o tráfego de entrada de aplicações em várias instâncias **EC2**, contêineres, endereços IP e funções **Lambda**. Isso garante **alta disponibilidade** e **desempenho** para suas aplicações.

---

## 🔹 1. Tipos de Balanceador de Carga
O **ELB** oferece três tipos principais de balanceadores de carga, cada um projetado para diferentes necessidades:
- 🌐 **Application Load Balancer (ALB)** → Ideal para tráfego **HTTP/HTTPS** e roteamento baseado em conteúdo.
- 🔌 **Network Load Balancer (NLB)** → Projetado para tráfego **TCP, UDP e TLS** com baixa latência.
- ⚙️ **Classic Load Balancer (CLB)** → Suporte para tráfego **HTTP, HTTPS, TCP e SSL** (recomendado para legados).

---

## 🔹 2. Alta Disponibilidade
O **ELB** distribui automaticamente o tráfego entre várias instâncias em **múltiplas zonas de disponibilidade**.
- ✅ Mantém o serviço **ativo mesmo em caso de falha** de uma instância.
- 📈 Melhora a **resiliência** e **escalabilidade** da aplicação.

---

## 🔹 3. Escalabilidade Automática
O **ELB** ajusta automaticamente a sua capacidade para lidar com **variações no tráfego de entrada**.
- 📊 Se adapta **dinamicamente** conforme a demanda cresce ou diminui.
- 🔄 Trabalha em conjunto com **Amazon Auto Scaling** para **otimizar o desempenho**.

---

## 🔹 4. Integração com Auto Scaling
O **ELB** funciona perfeitamente com **Auto Scaling** para:
- 🔍 Garantir que há capacidade **suficiente para suportar o tráfego**.
- 🛠️ **Substituir automaticamente** instâncias com falha.

---

## 🔹 5. Segurança
O **ELB** oferece recursos de segurança avançados:
- 🔐 **Integração com AWS Certificate Manager** → Para gerenciamento de **certificados SSL/TLS**.
- 🔑 **Integração com AWS IAM** → Para controle de acesso granular.
- 🛡️ **Proteção contra ataques DDoS** via AWS Shield.

---

## 🔹 6. Monitoramento e Auditoria
O **ELB** permite **monitorar e registrar** atividades através de serviços da AWS:
- 📊 **Amazon CloudWatch** → Para métricas de desempenho.
- 📜 **AWS CloudTrail** → Para auditoria e rastreamento de ações.
- 🚨 **Amazon SNS** → Para notificações em tempo real.

---

## 🏁 Conclusão
O **Elastic Load Balancing (ELB)** é uma ferramenta essencial para **distribuição eficiente de tráfego**, garantindo **alta disponibilidade, escalabilidade e segurança** para suas aplicações na AWS. Ele otimiza o desempenho ao distribuir automaticamente as requisições e proteger contra falhas. 🚀
