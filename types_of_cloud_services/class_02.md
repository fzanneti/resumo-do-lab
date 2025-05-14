# **Modelo de responsabilidade compartilhada**

**Imagina que você vai morar num prédio.**

O prédio (nuvem) é cuidado pelo síndico (Azure):  
> - segurança, portaria, elevador, água.

Mas dentro do seu apartamento (sua aplicação), você é o responsável:  
> - limpar, cozinhar, cuidar dos seus móveis.

Ou seja, cada um cuida de uma parte.

---

**O que é o modelo de responsabilidade compartilhada?**
> - É um acordo de quem cuida de quê entre o provedor de nuvem (Azure) e o cliente.

**Responsabilidades do Azure:**
> - Segurança física dos data centers
> - Energia, resfriamento e hardware
> - Virtualização e rede básica
> - Serviços de nuvem (dependendo do modelo: IaaS, PaaS, SaaS)

**Responsabilidades do cliente:**
> - Controle de identidade e acesso (IAM)
> - Segurança de dados e configurações
> - Gestão de usuários, senhas e permissões
> - Padrões de uso e conformidade

---

**Exemplo prático no Azure:**

|Serviço|Responsabilidade Azure|Responsabilidade cliente|
|:---:|:---:|:---:|
|IaaS|Hardware, rede, data center|Sistema operacional, dados, apps|
|PaaS|Infraestrutura + plataforma|Códigos e dados do app|
|SaaS|Tudo (infra, app, dados)|Uso e controle de acesso|

---