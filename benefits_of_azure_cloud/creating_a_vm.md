# **Criar uma máquina virtual no Azure**

**1. Acessar o portal do Azure**
- Vá até: https://portal.azure.com
- Login com conta corporativa vinculada à assinatura.

![login](https://github.com/fzanneti/resumo-do-lab/blob/004563efd3c0c41d1b5de4a680063ac0a8bb8450/assets/images/login.png)

**2. Iniciar o processo de criação da máquina**
- Clique no menu esquerdo em Máquinas Virtuais.
- Selecione + Criar > Máquina virtual.

![vm](https://github.com/fzanneti/resumo-do-lab/blob/cdc455c1efe3d1c5c1b895ca50e2e065fe2ac2fc/assets/images/vm.png)

**3. Aba "Básico" – Configuração inicial**
Preencha os seguintes campos:
- **Assinatura:** selecione a disponível (ex: Gratuita ou Paga).
- **Grupo de Recursos:** clique em “Criar novo” e nomeie (ex: GrupoVM-Teste).
- **Nome da Máquina Virtual:** vm-exemplo
- **Região:** escolha a mais próxima (ex: Brazil South).
- **Disponibilidade:** selecione “Sem redundância de infraestrutura” (para fins de teste).
- **Imagem:** selecione o SO desejado, ex: Windows 10 Pro ou Ubuntu 20.04 LTS.
- **Tamanho:** clique em “Alterar tamanho” e escolha um gratuito ou de baixo custo (ex: B1s).
- **Usuário e Senha:** crie um login administrativo para acessar a VM.

![config]
