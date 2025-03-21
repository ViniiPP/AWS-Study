# Resumo - EC2
O Amazon Elastic Compute Cloud (EC2) é um componente central da plataforma de computação em nuvem da Amazon. O EC2 permite aos usuários alugar máquinas virtuais usando a infraestrutura da Amazon. Ele foi projetado para tornar a computação em escala na web mais acessível para os desenvolvedores.

Aqui estão alguns pontos-chave sobre o Amazon EC2:



**Máquinas Virtuais:** EC2 fornece instâncias, que são máquinas virtuais executando os sistemas operacionais que você escolher.

**Escalabilidade:** Você pode dimensionar a capacidade de computação facilmente, criando e lançando novas instâncias conforme necessário, o que é útil para lidar com picos de demanda e escala.

**Controle Completo:** Os usuários têm controle total sobre as instâncias do EC2. Eles têm acesso de root, e podem interagir com elas como fariam com qualquer máquina.

**Várias Regiões e Zonas de Disponibilidade:** As instâncias do EC2 podem ser implantadas em várias regiões geográficas e zonas de disponibilidade. Isso ajuda a reduzir latência, aumentar a tolerância a falhas e cumprir os requisitos de residência de dados.

**Modelos de Instância:** O EC2 fornece uma variedade de tipos de instâncias otimizadas para diferentes casos de uso, garantindo que você tenha os recursos de que precisa para o aplicativo que está executando.

**Preços Flexíveis:** O EC2 oferece várias opções de preços, incluindo On-Demand (pague pelo que usar), Reservado (reserve uma instância por um período e obtenha um desconto) e Spot (licitação por capacidade não utilizada a preços mais baixos).

**Armazenamento Integrado:** As instâncias do EC2 podem ser integradas com outros serviços da AWS para fornecer armazenamento (por exemplo, Amazon EBS), bancos de dados (por exemplo, Amazon RDS), e redes (por exemplo, Amazon VPC).

**Segurança:** O EC2 trabalha com o Amazon VPC para fornecer segurança e robustez por meio de grupos de segurança e redes isoladas.

Em resumo, o Amazon EC2 é um serviço poderoso e flexível que forma a espinha dorsal da computação na plataforma AWS, permitindo que as empresas executem e dimensionem aplicativos na nuvem de forma eficiente e segura.

## Amazon EC2 - TIPOS DE EC2


O Amazon EC2 oferece uma variedade de tipos de instâncias otimizados para atender diferentes casos de uso. Os tipos de instâncias compreendem combinações variadas de capacidade de CPU, memória, armazenamento e rede e proporcionam a flexibilidade para escolher a combinação apropriada de recursos para seus aplicativos. Os principais tipos de instâncias do Amazon EC2 incluem:



Instâncias de Uso Geral (A, T, M): Essas instâncias proporcionam um bom equilíbrio de computação, memória e rede e são uma boa escolha para muitas cargas de trabalho que não requerem especificações de hardware específicas.

Instâncias Otimizadas para Computação (C): Essas instâncias são otimizadas para cargas de trabalho que exigem alta performance de CPU, como computação científica, modelagem e análise financeira, e renderização de mídia.

Instâncias Otimizadas para Memória (R, X, Z): Essas instâncias são projetadas para cargas de trabalho que processam grandes conjuntos de dados na memória, como bancos de dados em memória, caches distribuídos, análise em memória e aplicações de big data.

Instâncias Otimizadas para Armazenamento (D, I, H): Essas instâncias são projetadas para cargas de trabalho que requerem alto desempenho de armazenamento local, como bancos de dados escalonáveis, processamento de dados em escala de petabytes e aplicações de data warehousing.

Instâncias Otimizadas para GPU (P, G, F, Inf): Essas instâncias são projetadas para cargas de trabalho de computação gráfica, como aprendizado de máquina, mineração de criptomoedas, renderização 3D, e aplicações de streaming de jogos.

Instâncias Arm (A1, M6g, C6g, R6g): Essas instâncias são baseadas na arquitetura Arm e são uma opção de baixo custo para cargas de trabalho que requerem um bom desempenho de CPU e suportam a arquitetura Arm.

Os tipos de instâncias do Amazon EC2 são constantemente atualizados e ampliados para suportar uma gama cada vez maior de casos de uso. É importante verificar a documentação mais recente da AWS para obter as informações mais atualizadas.

# Amazon EC2 (didatico)
📌 Amazon EC2
Pense no EC2 como computadores na nuvem que você pode alugar. Mas cada computador tem um "superpoder" diferente. Vamos ver quais são:

🟢 Instâncias de Uso Geral (A, T, M)
👉 São os computadores "equilibrados", que fazem um pouco de tudo. Se você precisa de um computador para tarefas comuns, como rodar sites e aplicativos simples, esses são ideais!

⚡ Instâncias Otimizadas para Computação (C)
👉 Esses computadores são super-rápidos no cérebro (CPU)! Se você precisa fazer contas complicadas, como cálculos científicos, simulações ou renderização de vídeos, eles são a melhor escolha.

🧠 Instâncias Otimizadas para Memória (R, X, Z)
👉 Imagine um computador que consegue lembrar de muitas coisas ao mesmo tempo. Se você precisa trabalhar com grandes bancos de dados ou muita informação na memória, esses são os melhores.

💾 Instâncias Otimizadas para Armazenamento (D, I, H)
👉 Esses computadores são como grandes baús cheios de espaço! Se você precisa guardar MUITOS arquivos e acessá-los rapidamente, como em bancos de dados gigantes ou análise de dados, use esses.

🎮 Instâncias Otimizadas para GPU (P, G, F, Inf)
👉 Esses computadores têm placas de vídeo superpoderosas! São ótimos para jogos, inteligência artificial (machine learning), edição de vídeos e até mineração de criptomoedas.

🔵 Instâncias Arm (A1, M6g, C6g, R6g)
👉 Esses computadores usam uma tecnologia diferente (chamada Arm) e gastam menos energia. São bons para quem quer economizar dinheiro e precisa rodar aplicativos otimizados para essa tecnologia.

#

## Security Groups

Os Security Groups atuam como um firewall virtual para as suas instâncias Amazon EC2 para controlar o tráfego de entrada e saída. Eles operam ao nível da instância, o que significa que você pode associar diferentes security groups a diferentes instâncias, o que é útil para configurar a segurança a um nível granular.

Aqui estão algumas características principais dos Security Groups na AWS:

**Regras de entrada e saída:** Cada security group consiste em um conjunto de regras de entrada e saída. As regras de entrada controlam o tráfego que é permitido chegar à instância associada ao security group, enquanto as regras de saída controlam o tráfego permitido para sair da instância.

**Estado de conexão:** Os security groups são "stateful", o que significa que se você enviar uma solicitação de uma instância, a resposta é permitida automaticamente, independentemente das regras de saída.

**Permissões por protocolo:** As regras em um security group permitem especificar protocolos permitidos, portas e origem (para tráfego de entrada) ou destino (para tráfego de saída). Isso permite que você restrinja o tráfego para um protocolo ou porta específicos e controle de onde o tráfego é originado ou para onde ele é direcionado.

**Flexibilidade e controle:** Você pode associar diferentes security groups a diferentes instâncias e também pode modificar as regras de um security group a qualquer momento. As novas regras são aplicadas automaticamente a todas as instâncias associadas ao security group.

**Isolamento de instâncias:** Os security groups ajudam a isolar suas instâncias de outras instâncias na mesma rede, uma vez que as regras são aplicadas por instância e não por sub-rede.

Em resumo, os Security Groups são uma ferramenta crucial para gerenciar a segurança na AWS, permitindo que você controle e restrinja o tráfego de entrada e saída para suas instâncias do EC2 de uma maneira muito granular e específica.

