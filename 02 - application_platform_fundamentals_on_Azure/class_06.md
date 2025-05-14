# **Armazenamento**

**Domínio de Objeto**
- Armazena arquivos em formato de objeto. Ex: imagens, documentos.

**Redundância**
- Cópias dos dados em locais diferentes:
> - LRS: mesma região
> - GRS: outra região
> - RA-GRS: com acesso de leitura

**Serviços de armazenamento e pontos de extremidade**
- Blob, File, Queue, Table
- Pontos de acesso: URLs exclusivas para acessar arquivos

**Camadas de acesso**
- **Hot:** acessos frequentes
- **Cool:** acessos ocasionais
- **Archive:** acessos raros

**Azure Data Box**
- Aparelho físico para transferência de grandes volumes de dados

**Hands-On: Criar um Armazenamento de Blobs**
- Acesse o portal do Azure
- Clique em "Criar um recurso"
- Busque por "Storage Account"
- Configure nome, região, redundância
- Crie um contêiner e envie arquivos