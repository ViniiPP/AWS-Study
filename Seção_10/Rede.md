## Resumo sobre VPC e serviços relacionados na AWS

### 82. Sobre VPC
A Virtual Private Cloud (VPC) é uma rede privada dentro da AWS que permite isolar e controlar o tráfego de recursos na nuvem, como servidores e bancos de dados. Funciona como um ambiente de rede personalizado, onde você pode definir sub-redes, tabelas de roteamento e configurações de segurança.

### 83. Criando uma VPC
Criar uma VPC envolve configurar uma rede privada, definir intervalos de IPs, criar sub-redes e definir regras de segurança. Isso permite organizar melhor a infraestrutura na nuvem e garantir que os recursos tenham comunicação segura e eficiente.

### 84. Iniciando uma Instância com Elastic IP
Elastic IP é um endereço IP fixo que pode ser atribuído a uma instância EC2. Isso garante que a instância mantenha um IP público estático, mesmo após reinicializações, facilitando o acesso remoto e a configuração de serviços que exigem um IP fixo.

### 85. Sobre ACL
As Listas de Controle de Acesso (ACLs) são regras que controlam o tráfego de entrada e saída em sub-redes dentro da VPC. Diferente dos Security Groups, que são aplicados a instâncias, as ACLs são aplicadas a sub-redes inteiras e oferecem uma camada extra de segurança.

### 86. VPC Peering
O VPC Peering permite a conexão direta entre duas VPCs, facilitando a comunicação segura entre elas sem a necessidade de um gateway de internet ou VPN. Isso é útil para integrar sistemas distribuídos ou conectar diferentes ambientes de trabalho.

### 87. VPC Endpoints
VPC Endpoints permitem conectar serviços da AWS, como S3 e DynamoDB, diretamente à VPC sem passar pela internet. Isso melhora a segurança e o desempenho ao reduzir a necessidade de tráfego externo.

### 88. VPC Flow Logs
Os VPC Flow Logs registram informações sobre o tráfego de rede dentro da VPC. Isso ajuda a monitorar a comunicação entre instâncias, diagnosticar problemas de conectividade e melhorar a segurança.

### 89. Client e Site to Site VPN
- **Client VPN**: Permite que usuários individuais se conectem de forma segura à VPC a partir de seus dispositivos pessoais.
- **Site-to-Site VPN**: Conecta redes inteiras de empresas à VPC, permitindo a comunicação entre a infraestrutura local e a nuvem AWS.

### 90. AWS PrivateLink
O AWS PrivateLink permite que serviços dentro da AWS se comuniquem sem passar pela internet pública. Isso reduz riscos de segurança e melhora a performance ao usar redes privadas da AWS.

### 91. AWS Direct Connect
O Direct Connect é um serviço que estabelece uma conexão física dedicada entre a infraestrutura local e a AWS. Ele melhora a estabilidade e reduz a latência em comparação com conexões de internet tradicionais.

### 92. AWS Transit Gateway
O Transit Gateway facilita a conexão entre múltiplas VPCs e redes locais, funcionando como um hub centralizado para roteamento. Isso simplifica a gestão de redes complexas e melhora a eficiência da comunicação entre diferentes ambientes.

