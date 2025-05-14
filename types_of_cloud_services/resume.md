# **Revisão geral**

**IaaS:** 
> - Você monta tudo do zero.
> - Infraestrutura bruta.

**PaaS:** 
> - Te entregam a estrutura pronta, só precisa colocar o conteúdo.
> - Plataforma montada.

**SaaS:** 
> - Tudo pronto, é só usar.
> - Software pronto.

---

|Tipo de serviço|Responsável pela infraestrutura|Foco do cliente|Exemplo|
|:---:|:---:|:---:|:---:|
|IaaS|Cliente|Sistema operacional, apps, dados|VM, VNet, Discos|
|PaaS|Azure|Códigos e dados da aplicação|Azure SQL, App Services|
|SaaS|Azure|Apenas uso do software|Outlook, Temas, Dynamics|

---

## **Melhores cenários:**

**Imagina que você quer fazer um bolo.**
> - **IaaS:** Você vai ao mercado, compra todos os ingredientes e faz o bolo do zero. Dá mais trabalho, mas você faz do seu jeito.
> - **PaaS:** Já te entregam a massa pronta e a forma, e você só coloca para assar e decorar.
> - **SaaS:** O bolo já vem pronto, você só precisa comer.

Cada situação pede um jeito diferente.

---

## **Quando usar IaaS (Infrastructure as a Service):**

**Cenários ideais:**
> - Projetos que exigem controle total sobre o ambiente.
> - Ambientes de desenvolvimento e teste personalizados.
> - Migração de servidores locais para a nuvem (lift and shift).
> - Quando você precisa configurar o SO, middleware, banco de dados manualmente.

*Uma empresa quer transferir seus servidores físicos para a nuvem, mantendo a mesma estrutura. Nesse caso, IaaS oferece a flexibilidade necessária.*

---

## **Quando usar PaaS (Platform as a Service):**

**Cenários ideais:**
> - Desenvolvimento de aplicações web ou mobile com rapidez.
> - Projetos com equipes que querem focar só no código.
> - Necessidade de integração com banco de dados, autenticação, notificações etc.
> - Projetos com atualização constante sem precisar gerenciar infraestrutura.

*Uma startup quer lançar um app com rapidez. Com Azure App Service e Azure SQL, eles criam, testam e escalam sem se preocupar com servidores ou segurança do sistema operacional.*

---

## **Quando usar SaaS (Software as a Service):**

**Cenários ideais:**
> - Uso imediato de ferramentas sem instalação ou configuração.
> - Empresas que querem reduzir custos com licenças, suporte e TI.
> - Ambientes com necessidade de colaboração (email, reuniões, CRM etc.)

*Um time de vendas usa o Microsoft 365 para reuniões, e-mails e relatórios, sem precisar instalar nada ou cuidar de servidores.*