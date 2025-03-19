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