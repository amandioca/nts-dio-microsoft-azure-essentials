# Benefícios da Nuvem

**→ Alta disponibilidade:** recursos disponíveis sempre que necessário. **`faz parte do Azure SLA`**
* Há uma tabela com a porcentagem VS tempo de indisponibilidade previsto de cada recurso (minutos, horas/semana, mês). 
* Se passar do tempo previsto, a Microsoft irá ressarcir com estorno no pagamento original.

---
**→ Escalabilidade e Elasticidade:**
* `Escalabilidade`: subir a capacidade **manualmente**.
	* Escalonamento
	*  Manual
		
1. ***Scale UP*** (Mesmo RECURSO): como dar upgrade no seu PC (mais RAM, CPU melhor) para suportar mais carga. 
2. ***Scale OUT*** (Mais RECURSOS): adicionar mais máquinas, instâncias, recursos... para suportar a demanda. 

* `Elasticidade`: multiplicar a quantidade de um recurso **automaticamente**, conforme necessário. Recursos extras que entram e somem automaticamente de acordo com a demanda.
	* Flexível /Multiplicar
	* Automático

---
**→ Confiabilidade:** capacidade do sistema continuar funcionando mesmo se houver alguma falha. O design descentralizado permite isso, mesmo em situações de catástrofe. 
* Escala global: regiões e zonas de disponibilidade.
* Serviços gerenciados com redundância.
* Replicação de dados.
* Balanceamento de carga.
* Recuperação de falhas (Failover, Disaster Recovery).

> **A confiabilidade** não vem automaticamente. Depende da sua arquitetura.

---
**→ Previsibilidade:** capacidade de prever custo e comportamento do ambiente cases de sucesso, casos que funcionaram e serve de exemplo. Planejamento e Controle.

1. **Custos:** estima gastos e evita "sustos". 
	- Calculadora de custos
	- Orçamentos e alertas.
2. **Performance:**
	- Planos/tamanhos de recursos definem o "nível" de performance. 
	- Você sabe o que esperar de cada SKU/tier.

> Não é segurança 
> Não é garantia de *uptime* (SLA)!

---
**→ Segurança:** conjunto de mecanismos disponíveis para proteger dados, acessos e infraestrutura.
Proteger contra ataque, vazamento e acesso indevido.
* Controle de identidade e acesso (RBAC).
* Autenticação e autorização. 
* Criptografia de dados em trânsito e em Repouso.
* Firewall, NSG (Network Security Group), Regras de Rede.
* Monitoramento de ameaças.

> Segurança é responsabilidade compartilhada. 
> - Azure protege a infraestrutura
> - Cliente protege usuários, senhas, acessos, permissões, configs.

---
**→ Governança:** conjunto de regras, políticas e controles para dar ler que o uso do Azure esteja organizado, seguro e dentro do que a empresa permite. **`REGRAS!`**

> **Leis**: sem leis, vira bagunça
> A diretoria da empresa define as regras, padrões e políticas.

* **Padronização:** todo ambiente precisa de tag.
* **Controle de acesso:** dev não cria recurso em PRD.
* **Controle de custos:** bloquear criação de VM muito cara.
* **Conformidade:** seguir regras de segurança/compliance da empresa.
* **Evitar bagunça:** nada de recurso "solto", sem dono, sem tag.

Exs. prático na ***Azure***:
* Políticas que bloqueiam certos tipos de recursos.
* Regras de *naming*.
* Limites de quem pode apagar/criar coisas.
* Organização de grupos de recursos, assinaturas, ambientes.

> Regras do Jogo.
> Boa governança = **organização**!

---
**→ Gerenciabilidade:** capacidade de monitorar, operar, automatizar e manter o ambiente no dia a dia. **`OPERAÇÃO!`**

> **Manutenção**: sem isso, tudo quebra
> A operação executa e mantém tudo funcionando dentro dessas regras.

* **Monitoramento e alertas:** saber que algo está lento e quando caiu.
* **Automação de tarefas:** Rotinas de manutenção, subir/descer Recursos.
* **Visibilidade do ambiente:** ver o que está rodando, quem usa, quanto custa.
* **Operação mais simples:** menos traz alto manual.
* **Resposta mais rápida a incidentes.**

> Bom gerenciamento = **fácil de manter**!
