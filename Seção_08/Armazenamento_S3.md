 Sobre o S3
O Amazon S3 (Simple Storage Service) é um serviço de armazenamento na nuvem que permite guardar arquivos de forma segura, escalável e acessível de qualquer lugar. Ele funciona como uma "nuvem de arquivos" onde você pode armazenar documentos, imagens, vídeos e muito mais.

 Criando uma Bucket
Uma Bucket é como uma pasta principal dentro do S3, onde você armazena seus arquivos. Para criar uma, basta acessar o S3 no console da AWS, escolher um nome único e configurar permissões e regiões de armazenamento.

 Classes do S3
O S3 oferece diferentes classes de armazenamento, cada uma com um custo e nível de acesso diferente:

Standard: Acesso frequente, mais caro.

Intelligent-Tiering: Alterna entre acessos frequentes e raros automaticamente.

Standard-IA e One Zone-IA: Para arquivos menos acessados, mais barato.

Glacier e Glacier Deep Archive: Arquivos raramente acessados, custo muito baixo.

Cada classe é ideal para diferentes necessidades, como backups ou arquivos de uso contínuo.

 Valores do S3
O custo do S3 depende de três fatores principais:

Espaço usado: Quanto maior o armazenamento, maior o custo.

Transferência de dados: Baixar arquivos pode gerar custos adicionais.

Operações realizadas: Ações como leitura e escrita também podem influenciar no preço.

A AWS fornece uma calculadora de preços para estimar os custos antes de usar.

 Hospedando um site em S3
É possível hospedar um site estático no S3, ou seja, páginas HTML, CSS e JavaScript sem backend. Basta:

Criar uma Bucket com o nome do domínio.

Ativar a opção de hospedagem estática.

Fazer upload dos arquivos do site.

Configurar permissões para torná-lo público.

(Opcional) Usar o CloudFront para melhorar o desempenho.

Essa solução é barata e escalável.

 Habilitando Versionamento
O versionamento permite manter diferentes versões de um arquivo dentro da mesma Bucket. Isso é útil para recuperação de arquivos apagados por engano ou controle de alterações. Para ativar:

Vá até a configuração da Bucket.

Habilite a opção de versionamento.

Com isso, o S3 salva todas as versões de um arquivo, mesmo se for sobrescrito.

 Replicação de Buckets
A replicação de Buckets permite copiar arquivos de uma Bucket para outra automaticamente. Isso é útil para backup e alta disponibilidade.

Replicação dentro da mesma região: Para redundância local.

Replicação entre regiões (CRR - Cross-Region Replication): Para cópias em diferentes locais do mundo.

É necessário ativar essa configuração e definir regras para quais arquivos serão replicados.

. Sobre Criptografia S3
O S3 permite armazenar arquivos de forma segura, protegendo-os com criptografia. Existem três opções principais:

Criptografia do lado do servidor (SSE) – O próprio S3 protege os arquivos automaticamente.

Criptografia do lado do cliente – O usuário encripta os dados antes de enviá-los para o S3.

Chaves gerenciadas pelo KMS – Uso do serviço AWS KMS para controle avançado de chaves.

Isso garante proteção contra acessos não autorizados.

 Sobre Storage Gateway
O AWS Storage Gateway é um serviço que conecta ambientes locais com o armazenamento na AWS. Ele permite que empresas usem a nuvem como um disco virtual, facilitando backups e migração de dados.
Existem três tipos principais:

File Gateway: Para armazenar arquivos no S3 como se fosse um servidor local.

Volume Gateway: Para criar discos na nuvem que podem ser usados em máquinas locais.

Tape Gateway: Para substituir fitas físicas por backups na nuvem.

Isso ajuda empresas a reduzirem custos e melhorarem a disponibilidade dos dados.

. A família Snow da AWS
A Família Snow é um conjunto de dispositivos físicos da AWS usados para transferir grandes volumes de dados para a nuvem sem depender da internet. Os principais membros são:

AWS Snowcone: Pequeno e portátil, ideal para transferências menores.

AWS Snowball: Para volumes médios de dados, como dezenas de terabytes.

AWS Snowmobile: Caminhão que transporta exabytes de dados, usado por grandes empresas.

Essa solução é útil quando a conexão com a internet é lenta ou inviável para grandes migrações.