# **Como a computação em nuvem funciona?**

Imagina que você tem um videogame em casa.  
Quando quer jogar, você precisa de um console, de um jogo e da televisão.  
Isso é como ter tudo na sua casa: você cuida, paga, e conserta se quebrar.

Agora imagina que existe um videogame mágico que mora na nuvem (tipo no céu ☁️) e você pode jogar de qualquer lugar, só usando a internet.  
Você não precisa comprar o console, nem o jogo, nem consertar nada se quebrar.  
Você paga só quando usar.

*Isso é a computação em nuvem (ou Cloud Computing):* ao invés de ter tudo no seu computador ou empresa, você usa servidores e programas que ficam em centros de dados gigantes, na internet.  
Você só usa, como um serviço.

A computação em nuvem permite que empresas e pessoas utilizem recursos de TI (como servidores, bancos de dados, armazenamento e software) pela internet, sem precisar investir em infraestrutura física local.

Esses recursos são alocados sob demanda e pagos conforme o uso, por isso o modelo é chamado de "as a Service" (como serviço).

---

**“As a Service” – O que significa?**  
> - **IaaS (Infraestrutura como Serviço):** você aluga servidores, redes, e discos rígidos. Ex: Amazon EC2.
> - **PaaS (Plataforma como Serviço):** você usa uma plataforma completa para desenvolver aplicações. Ex: Google App Engine.
> - **SaaS (Software como Serviço):** você usa um software pronto, direto do navegador. Ex: Gmail, Microsoft 365.

---

**Custos do Modelo Local (On-Premise)** 


Quando a empresa opta por manter tudo local (On-Premise), os custos incluem:
> - Compra de servidores e licenças
> - Instalação e manutenção
> - Equipe técnica dedicada
> - Atualizações manuais
> - Energia e refrigeração

*Ou seja: alto investimento inicial (CapEx) e manutenção constante.*

---

## **vs ☁️ On-Premise x Cloud**

|Fator|On-Premise|Cloud|
|:---:|:---:|:---:|
|Custo Inicial|Alto|Baixo|
|Escalabilidade|Difícil|Fácil e rápida|
|Manutenção|Interna|Fornecedor|
|Segurança|Totalmente controlada pela empresa|	Compartilhada com o provedor|
|Flexibilidade|Limitada|Alta|

---

**Hybrid Model (Modelo Híbrido)**  

É quando a empresa usa parte dos recursos localmente e parte na nuvem.

Por exemplo:
> - Servidor de arquivos sensíveis na sede da empresa (on-premise)
> - Aplicações e backups na nuvem

*Esse modelo é usado para ganhar flexibilidade sem abrir mão da segurança local.*

---

**Qual Modelo Escolher?**  

Depende da necessidade da empresa:
> - Pequenas empresas ou startups: geralmente escolhem 100% cloud, pela agilidade e menor custo.
> - Grandes empresas: podem optar por modelo híbrido para manter o controle de dados críticos.
> - Ambientes com alta regulamentação (financeiro, saúde): costumam exigir mais controle local.

---

**Platform – O que é isso na nuvem?**  

É o conjunto de ferramentas, serviços e ambientes que você pode usar para desenvolver, hospedar e escalar aplicações.

Exemplo:
> - Google Cloud Platform (GCP)
> - Amazon Web Services (AWS)
> - Microsoft Azure

*Essas plataformas oferecem tudo: servidores, banco de dados, inteligência artificial, segurança, etc.*

---

**Regions & Zones – Como a nuvem se organiza fisicamente?**
 
As nuvens públicas têm data centers espalhados pelo mundo:
> - Regiões: grupos de data centers em uma área geográfica (ex: "São Paulo", "Londres", "Tóquio").
> - Zonas: subdivisões dentro das regiões (ex: SP-Zone-1, SP-Zone-2).

Isso ajuda a garantir:
> - Alta disponibilidade (se uma zona cair, outra assume)
> - Menor latência (usar servidores próximos a você)
> - Conformidade com leis locais de dados (LGPD no Brasil, por exemplo)

---