## **Infra Global**
A infraestrutura global da AWS é a base sobre a qual os serviços da AWS são construídos. Ela consiste em uma série de Regiões e Zonas de Disponibilidade espalhadas pelo mundo, projetadas para fornecer um serviço seguro, confiável e escalável.

- -Regiões: Uma região da AWS é uma área geográfica que contém pelo menos duas Zonas de Disponibilidade. Cada região é completamente independente das outras regiões, o que ajuda a isolar falhas e evitar a propagação de problemas de uma região para outra. Em setembro de 2021, a AWS tinha 25 regiões geográficas ao redor do mundo.

- Zonas de Disponibilidade (AZs): Cada região da AWS é dividida em Zonas de Disponibilidade. Cada AZ é um centro de dados separado dentro de uma região, mas todas as AZs dentro de uma região estão conectadas através de redes de alta velocidade, de baixa latência e totalmente redundantes. As AZs fornecem uma maneira de construir aplicativos altamente disponíveis e tolerantes a falhas.

- Zonas Locais: As zonas locais da AWS aproximam a computação, o armazenamento, o banco de dados e outros produtos da AWS selecionados dos usuários finais. Com as zonas locais da AWS, você pode executar facilmente aplicativos altamente exigentes que exigem latências em milissegundos de um dígito para seus usuários finais, como criação de conteúdo de mídia e entretenimento, jogos em tempo real, simulações de reservatórios, automação de projetos eletrônicos e machine learning.

- Wavelenght: O AWS Wavelength permite que os desenvolvedores criem aplicações com latências de um dígito para dispositivos móveis e usuários finais. Os desenvolvedores da AWS podem implantar seus aplicativos nas Zonas do Wavelength, implantações de infraestrutura da AWS que incorporam serviços de computação e armazenamento da AWS aos datacenters dos provedores de telecomunicações na borda das redes 5G e acessam facilmente a variedade de serviços da AWS na região. Isso permite que os desenvolvedores forneçam aplicativos que exigem latências inferiores a 10 milissegundos, como streaming de jogos e vídeos ao vivo, inferência de machine learning na borda e realidade aumentada e virtual (AR/VR).

- OutPosts: O AWS Outposts leva produtos, infraestrutura e modelos operacionais nativos da AWS a praticamente qualquer datacenter, espaço de colocalização ou instalações on-premises. Você pode usar as mesmas APIs, ferramentas e infraestrutura da AWS no local e na Nuvem AWS para oferecer uma experiência híbrida verdadeiramente consistente. O AWS Outposts foi projetado para ambientes conectados e pode ser usado para oferecer suporte a workloads que precisam permanecer on-premises devido à baixa latência ou às necessidades de processamento de dados locais.

- A infraestrutura global da AWS permite que os usuários implantem seus aplicativos e serviços de maneira flexível, resiliente e eficiente em termos de latência, onde quer que seus clientes estejam localizados no mundo. Isso significa que, como usuário da AWS, você pode oferecer uma experiência de usuário mais rápida e melhor para seus clientes, independentemente de sua localização geográfica.









## **Share Model**
O Modelo de Responsabilidade Compartilhada da AWS é uma estrutura de governança que delineia a divisão de responsabilidades de segurança entre a Amazon Web Services (AWS) e o usuário (cliente). Essa divisão de responsabilidades permite que a AWS se concentre na segurança da infraestrutura de computação em nuvem, enquanto o usuário se concentra na segurança dos dados e recursos que colocam na nuvem.

Aqui está uma visão geral das responsabilidades compartilhadas:



Segurança "da" nuvem: A AWS é responsável pela proteção da infraestrutura que executa todos os serviços oferecidos na AWS Cloud. Isso inclui hardware, software, redes e instalações que sustentam os serviços AWS Cloud.

Segurança "na" nuvem: O cliente é responsável pela segurança de qualquer coisa que coloque "na" nuvem ou conecte "à" nuvem. Isso pode incluir a configuração correta de controles de segurança e conformidade em serviços da AWS, gerenciamento de dados (incluindo criptografia e backups), classificação de ativos e outras várias tarefas de segurança de TI.

Serviços de Infraestrutura, Contêiner e Abstração: Dependendo do tipo de serviço da AWS que está sendo usado (por exemplo, uma instância EC2 versus um banco de dados RDS), a AWS e o cliente compartilharão diferentes partes da responsabilidade de segurança. Por exemplo, para um serviço de infraestrutura como o EC2, a AWS fornece a segurança física, a do hypervisor e a da rede, enquanto o cliente é responsável pelo sistema operacional e pelas aplicações. Para um serviço de contêiner como o RDS, a AWS também é responsável pela segurança do sistema operacional e do serviço de banco de dados, enquanto o cliente ainda é responsável pelas aplicações e dados.

A compreensão e a aplicação adequada do Modelo de Responsabilidade Compartilhada da AWS são fundamentais para garantir a segurança e a conformidade ao usar a AWS. Isso requer que os clientes estejam cientes de suas responsabilidades de segurança e implementem práticas de segurança robustas ao usar serviços da AWS.

# Resumo didatico

## ShareModel

Imagina que a AWS é como um prédio alugado e você é um inquilino que mora nele. A AWS cuida da estrutura do prédio – as paredes, o teto, a segurança da entrada – para garantir que tudo esteja seguro e funcionando. Isso é a segurança "da" nuvem.

Agora, dentro do seu apartamento (sua conta na AWS), a responsabilidade é sua! Você precisa trancar as portas, guardar bem seus pertences e configurar as fechaduras do jeito certo. Isso é a segurança "na" nuvem.

Ou seja:
🔹 AWS protege a infraestrutura (prédios, servidores, redes).
🔹 Você protege o que coloca na nuvem (dados, configurações, acessos).

Se você configurar errado, pode deixar sua "porta aberta" e qualquer um pode entrar. Por isso, é importante seguir boas práticas para manter seus dados seguros! 😊

--- 

## Infra Global
🌍 Regiões → Pense nas regiões da AWS como cidades diferentes. Cada cidade tem seus próprios prédios e funciona de forma independente. Se uma cidade tiver um problema, as outras continuam funcionando normalmente.

🏢 Zonas de Disponibilidade (AZs) → Dentro de cada cidade (região), existem vários prédios (Zonas de Disponibilidade). Esses prédios são conectados por internet super rápida, garantindo que, se um der problema, os outros continuem funcionando.

📍 Zonas Locais → Imagine que a AWS construiu escritórios menores mais perto dos usuários para que tudo funcione mais rápido, sem atrasos. Isso é ótimo para jogos e vídeos ao vivo.

📶 Wavelength → É como colocar mini escritórios da AWS dentro das operadoras de celular 5G. Isso faz com que apps como jogos online e realidade aumentada funcionem sem travar.

🏠 Outposts → Às vezes, empresas querem usar a AWS, mas sem sair do próprio escritório. O AWS Outposts é como trazer uma parte da AWS para dentro da empresa.

➡️ Resumo geral: A AWS funciona como uma rede de cidades e prédios bem organizados, garantindo que tudo funcione rápido, sem falhas e de forma eficiente para qualquer pessoa no mundo! 🚀