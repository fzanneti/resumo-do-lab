# **Criar uma máquina virtual no Azure**   

> https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal

**1. Acessar o portal do Azure**
- Vá até: https://portal.azure.com
- Login com conta corporativa vinculada à assinatura.

<img src="https://github.com/fzanneti/resumo-do-lab/blob/3fea88b8de96e661f5823d2f863253e1c317f9fd/00%20-%20assets/images/login.png" alt="login" width="50%">

**2. Iniciar o processo de criação da máquina**
- Clique no menu esquerdo em Máquinas Virtuais.
- Selecione + Criar > Máquina virtual.

<img src="https://github.com/fzanneti/resumo-do-lab/blob/3fea88b8de96e661f5823d2f863253e1c317f9fd/00%20-%20assets/images/vm.png" alt="login" width="50%">

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

<img src="https://github.com/fzanneti/resumo-do-lab/blob/3fea88b8de96e661f5823d2f863253e1c317f9fd/00%20-%20assets/images/create_vm_part_1.png" alt="login" width="50%">

<img src="https://github.com/fzanneti/resumo-do-lab/blob/3fea88b8de96e661f5823d2f863253e1c317f9fd/00%20-%20assets/images/create_vm_part_2.png" alt="login" width="50%">

**4. Aba "Discos" – Escolha do disco de sistema**
- Tipo de disco do SO: escolha SSD (mais rápido) ou HDD (mais barato).
- Deixe o restante como padrão.

<img src="https://github.com/fzanneti/resumo-do-lab/blob/3fea88b8de96e661f5823d2f863253e1c317f9fd/00%20-%20assets/images/disc.png" alt="login" width="50%">

**5. Aba "Rede" – Configurações de acesso**  
IP público: sim (para acessar de fora).  
Portas de entrada: habilite RDP (Windows) ou SSH (Linux), dependendo do sistema.  

<img src="https://github.com/fzanneti/resumo-do-lab/blob/3fea88b8de96e661f5823d2f863253e1c317f9fd/00%20-%20assets/images/network.png" alt="login" width="50%">
