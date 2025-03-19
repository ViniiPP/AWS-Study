

##  O que é o IAM
- **Definição**: O AWS Identity and Access Management (IAM) é um serviço essencial da Amazon Web Services que permite gerenciar quem pode acessar os recursos da sua conta AWS e o que essas pessoas ou sistemas podem fazer com eles.
- **Objetivo**: Proteger a infraestrutura na nuvem ao garantir que apenas usuários autorizados realizem ações específicas, como criar servidores ou acessar dados sensíveis.
- **Componentes principais**: Inclui usuários (pessoas ou aplicativos), grupos (coleções de usuários), políticas (regras de permissão) e papéis (funções temporárias para serviços ou usuários externos).
- **Princípio**: Baseia-se no conceito de "menor privilégio", ou seja, dar às identidades apenas as permissões mínimas necessárias para suas tarefas, reduzindo riscos de segurança.
- **Custo**: O IAM é oferecido sem custo adicional, sendo uma ferramenta nativa e integrada à AWS.

##  Grupos
- **Conceito**: Grupos no IAM são coleções de usuários que compartilham as mesmas permissões, como acesso a determinados serviços ou recursos da AWS.
- **Benefício**: Em vez de configurar permissões individualmente para cada usuário, os grupos permitem aplicar regras de acesso de forma consistente e eficiente, ideal para equipes ou departamentos.
- **Característica**: As permissões são definidas por políticas (documentos JSON) que você associa ao grupo, especificando o que é permitido ou negado.
- **Exemplo**: Um grupo chamado "Admins" pode ter permissões amplas para gerenciar toda a conta, enquanto "Desenvolvedores" pode ter acesso apenas a serviços específicos, como o Amazon S3.

##  Criando Usuários
- **Definição**: Usuários são identidades únicas criadas no IAM para representar pessoas (como funcionários) ou sistemas (como aplicações) que interagem com a AWS.
- **Tipos de acesso**: Podem ter acesso programático, usando chaves de acesso (Access Key ID e Secret Access Key) para APIs, ou acesso ao console da AWS, com login e senha.
- **Prática**: Permissões podem ser atribuídas diretamente ao usuário ou, de forma mais prática, vinculando-o a um grupo com políticas predefinidas.
- **Recomendação**: O usuário root (criado ao abrir a conta AWS) tem acesso total e deve ser evitado para tarefas rotineiras, pois é um ponto de risco se comprometido.

##  O IAM Identity Center
- **Finalidade**: O IAM Identity Center é uma solução para gerenciar o acesso centralizado a várias contas AWS e aplicativos de negócios, eliminando a necessidade de credenciais separadas para cada sistema.
- **Recurso**: Oferece Single Sign-On (SSO), permitindo que os usuários façam login uma vez e acessem todos os recursos permitidos sem precisar se autenticar novamente.
- **Integração**: Pode se conectar a provedores de identidade externos, como Microsoft Active Directory ou serviços como Okta, sincronizando usuários existentes.
- **Aplicação**: É especialmente útil para organizações grandes que gerenciam dezenas ou centenas de contas AWS e precisam de uma gestão de acesso unificada.

##  Sobre o MFA
- **Conceito**: A Autenticação Multifator (MFA) é uma camada extra de segurança que exige, além da senha, uma segunda forma de verificação para confirmar a identidade do usuário.
- **Mecanismo**: Funciona combinando algo que você sabe (a senha) com algo que você possui (como um código gerado por um aplicativo ou uma chave física).
- **Opções**: Suporta dispositivos como aplicativos móveis (ex.: Google Authenticator, Authy) ou chaves de hardware (ex.: YubiKey), oferecendo flexibilidade ao usuário.
- **Valor**: Reduz drasticamente o risco de acesso não autorizado, mesmo que a senha seja roubada, sendo uma prática essencial para proteger contas críticas.

## Habilitando o MFA
- **Objetivo**: Ativar o MFA no IAM para aumentar a segurança de usuários, especialmente aqueles com permissões sensíveis, como administradores.
- **Ferramentas**: Pode ser configurado com aplicativos que geram códigos temporários ou dispositivos físicos que produzem autenticação baseada em toque ou inserção.
- **Foco**: É altamente recomendado para o usuário root, que tem controle total da conta, e para qualquer usuário com acesso a recursos críticos, como bancos de dados ou configurações de segurança.
- **Funcionalidade**: Após ativação, o login exige um código único gerado em tempo real, renovado geralmente a cada 30 segundos.

##  Organizações AWS
- **Definição**: AWS Organizations é um serviço que permite gerenciar várias contas AWS sob uma estrutura centralizada, simplificando a administração em ambientes complexos.
- **Vantagens**: Oferece faturamento consolidado (uma única fatura para todas as contas) e a capacidade de aplicar políticas de controle de serviço (SCPs) para limitar ações em contas específicas.
- **Estrutura**: Organiza-se em torno de uma conta mestre (management account), que controla as contas membros, formando uma hierarquia lógica.
- **Uso**: Ideal para empresas com múltiplos projetos, departamentos ou unidades de negócios, permitindo governança centralizada e segura.

## Habilitando as Organizações
- **Propósito**: Criar uma organização AWS para unificar o gerenciamento de contas, começando pela conta mestre que será o ponto de controle.
- **Recurso**: Permite adicionar contas existentes (via convite) ou criar novas contas dentro da organização, todas vinculadas à estrutura central.
- **Controle**: Usa Service Control Policies (SCPs) para definir limites de permissões em nível organizacional, complementando as políticas do IAM.
- **Escopo**: Recomenda-se começar com uma estrutura pequena e simples, expandindo conforme a organização cresce, para evitar complexidade inicial.





# 🔐 Políticas de Senhas

A política de senhas do AWS IAM estabelece regras para fortalecer a segurança das credenciais dos usuários. Em resumo, ela permite que você defina:

-   **Tamanho mínimo:** Geralmente exige um número mínimo de caracteres (por exemplo, 8 ou mais);
-   **Complexidade:** A senha deve incluir, conforme configurado, letras maiúsculas, letras minúsculas, números e símbolos;
-   **Restrições:** Pode impedir que a senha contenha partes do nome do usuário ou outras informações pessoais;
-   **Expiração:** Define um período após o qual a senha deve ser alterada (por exemplo, a cada 90 dias);
-   **Histórico:** Impede a reutilização das últimas senhas (como as últimas 5 senhas, por exemplo);
-   **Idade mínima:** Pode exigir um intervalo mínimo entre as alterações de senha para evitar mudanças muito frequentes.

---
# ☁️ CloudShell e CLI
Na AWS, você tem duas formas principais de usar a linha de comando:

-   **AWS CLI:** Essa é uma ferramenta que você instala no seu computador para interagir com os serviços AWS via comandos. Após configurá-la com suas 
    credenciais (por exemplo, via aws configure), você pode executar comandos para criar, listar e gerenciar recursos de forma programática.

-   **AWS CloudShell:** É um terminal acessível diretamente pelo navegador, integrado ao Console AWS. O CloudShell já vem com o AWS CLI pré-instalado e 
    configurado automaticamente com as suas credenciais do Console. Assim, você pode executar comandos sem precisar instalar nada no seu computador. 
    Ele oferece um ambiente seguro, com um diretório persistente para seus scripts e arquivos.


---
# AWS Access Key e SDK

### **AWS Access Key**
-   As AWS Access Keys são um par de credenciais (ID da Chave de Acesso e Chave de Acesso Secreta) que permitem a autenticação programática 
    em serviços da AWS. Você as gera no IAM e as utiliza para assinar chamadas à API, seja via AWS CLI ou SDK. É essencial protegê-las, pois 
    qualquer pessoa com essas chaves pode acessar seus recursos na AWS.

### **AWS SDK**
-   O AWS SDK é um conjunto de bibliotecas para diversas linguagens de programação (como Python, JavaScript, Java, etc.) que facilita a 
    integração das suas aplicações com os serviços da AWS. Ele cuida de detalhes como autenticação (usando as Access Keys), formatação de requisições 
    e tratamento de erros, permitindo que você interaja com a AWS de maneira mais simples e eficiente.