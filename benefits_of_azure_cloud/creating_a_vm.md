# **Criar uma máquina virtual no Azure** ![🖥️](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)

**1. Acessar o portal do Azure**
- Vá até: https://portal.azure.com
- Login com conta corporativa vinculada à assinatura.

![login](https://github.com/fzanneti/resumo-do-lab/blob/ca93de6bf6203baf528ab4b3a4509ad3161f117d/assets/images/login.png)

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
  
![config1](https://github.com/fzanneti/resumo-do-lab/blob/7fb517052dcee633fad0d9e28e821a2650e06bec/assets/images/create_vm_part_11.png)
  
![config2](https://github.com/fzanneti/resumo-do-lab/blob/2ef3d4658e993f8458529e5b4386c7cf60778a0e/assets/images/create_vm_part_2.png)

**4. Aba "Discos" – Escolha do disco de sistema**
- Tipo de disco do SO: escolha SSD (mais rápido) ou HDD (mais barato).
- Deixe o restante como padrão.

![disc](https://github.com/fzanneti/resumo-do-lab/blob/main/assets%2Fimages%2Fdisc.png)

**5. Aba "Rede" – Configurações de acesso**
IP público: sim (para acessar de fora).
Portas de entrada: habilite RDP (Windows) ou SSH (Linux), dependendo do sistema.

