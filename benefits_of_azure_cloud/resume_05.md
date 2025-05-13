## 1. **Disponibilidade – A Regra dos noves na Microsoft Azure**  

*O que é Disponibilidade?*  
Disponibilidade mede o tempo que um serviço está acessível e funcionando sem interrupções.
  
*O que é a Regra dos Noves?*  
É uma forma de representar a confiabilidade de um serviço com números 9 repetidos, quanto mais 9s, menor a chance de falha.  

---

### **Regra dos Noves: Tempo de Inatividade Permitido**

|SLA (Disponibilidade)|Por Dia|Por Mês (30 dias)|Por Ano|
|---|---|---|---|
|90% (1 nove)|2h 24min|72 horas|876 horas|
|99% (2 noves)|14 min 24s|7h 18min|87h 36min|
|99,9% (3 noves)|1 min 26s|43min 49s|8h 45min|
|99,99% (4 noves)|8,6 segundos|4min 22s|52min 33s|
|99,999% (5 noves)|0,86 segundos|26 segundos|5min 15s|  

---
  
### **Impactos de uma escolha incorreta de SLA:**  

|Escolha Incorreta|Possível Impacto|
|---|---|
|Usar SLA de 99% em sistema bancário|Perda de acesso por horas: prejuízo financeiro e reputacional|
|Usar SLA alto para app interno pouco usado|Gastos desnecessários com infraestrutura|
|Não considerar SLA em contrato|Você não tem direito a reembolso ou garantia se o sistema cair|  

---
  
### **Custos relacionados à Disponibilidade**

- Quanto maior o SLA, maior o custo.
- Ambientes com alta disponibilidade exigem redundância, balanceadores, múltiplas regiões.

Exemplo: 
> - Um banco paga mais para garantir mínimo de downtime, já uma padaria pode aceitar indisponibilidade por alguns minutos sem prejuízo.

---

## 2. **Armazenamento – SLA e implicações técnicas**

*O que é o SLA de Armazenamento na Azure?*
- É o compromisso da Microsoft com a durabilidade e disponibilidade dos dados armazenados.

---

**SLA de Durabilidade**

|Tipo de Redundância|SLA (Durabilidade)|Detalhes|
|---|---|---|
|LRS (Locally Redundant)|11 noves (99,999999999%)|Dados replicados 3 vezes no mesmo datacenter|
|GRS (Geo-Redundant)|16 noves (99,99999999999999%)|Dados replicados em outra região geográfica|  
  
Exemplo: 
>- Armazenar com GRS é ideal para backup crítico e recuperação de desastres.

---

**SLA de Disponibilidade de Armazenamento**

|Serviço|SLA|
|---|---|
|Azure Blob Storage|99,9% a 99,99%|
|Azure Files|99,99%|

---

> Varia conforme o tipo de redundância e o nível de desempenho (Standard x Premium).

---

**Impactos e Custos de Escolhas Incorretas**

|Escolha Errada|Impacto|Custo Gerado|
|---|---|---|
|Escolher LRS para backup crítico|Perda de dados em caso de desastre físico no datacenter|Perda financeira e de confiança|
|Escolher GRS para dados temporários|Gasto desnecessário com armazenamento caro|Aumento de custo sem retorno|
|Não considerar latência e redundância|Aplicações lentas ou com falhas de acesso|Insatisfação do cliente|

---

Resumo final: Boa escolha traz economia e segurança
> - A escolha do nível de SLA certo depende da importância do sistema para o negócio.
> - Nem sempre vale pagar mais por 5 noves se 3 já são suficientes para o seu uso.
> - Use Azure Advisor e Azure Cost Management para acompanhar e ajustar conforme necessidade.

---

## **Quadro de decisão – Escolha do SLA na Azure**

|Tipo de Aplicação / Sistema|Nível de Disponibilidade Recomendado|Tipo de Armazenamento Recomendado|Justificativa|
|:---:|:---:|:---:|:---:|
|Sistema Bancário / Financeiro|99,99% ou mais|GRS ou RA-GRS|Crítico, não pode parar nem perder dados.|Redundância geográfica é essencial.|
|E-commerce em horário comercial|99,9%|ZRS ou GRS|Deve ficar online durante vendas, mas pode ter breves pausas fora do pico.
|Aplicativo interno de RH|99%|LRS|Uso interno tolera pequenas interrupções.|GRS seria custo desnecessário.|
|Backup de documentos importantes|99,9% (acesso) / 16 noves (durabilidade)|GRS ou RA-GRS|Dados precisam ser preservados por anos.|Alta durabilidade é prioridade.|
|Projeto escolar / Estágio|90% – 99%|LRS|Tolerância alta a falhas e menor orçamento.|Pode ficar fora do ar sem grandes prejuízos.|
|Aplicações críticas em saúde|99,999%|GRS com failover automático|Nenhuma tolerância à falhas.|Vida e segurança dependem do sistema.|
|Site de Portfólio pessoal|99%|LRS|Downtime ocasional não afeta diretamente o negócio.|

**Legenda rápida**
- **LRS:** Locally Redundant Storage (3 cópias locais)
- **ZRS:** Zone-Redundant Storage (em múltiplas zonas da mesma região)
- **GRS:** Geo-Redundant Storage (outra região geográfica)
- **RA-GRS:** GRS com acesso de leitura na réplica  
