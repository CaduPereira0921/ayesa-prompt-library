### 1.1b — CHAT (pontual) · framework DMAIC + estimativas (Iterative Prompting)

**Quando usar:** quando o gerente precisa transformar fatos dispersos de um atraso
em diagnóstico estruturado para apresentar ao comitê. Usar em 4 passos iterativos.

**Passo 1 — Diagnóstico inicial (DMAIC)**
Sou gerente de um projeto de [tipo de projeto] para um cliente [setor],
porte [pequeno/médio/grande]. Equipe de [N] pessoas ([composição]).
O projeto tem [N] sprints, estamos na sprint [N].

O seguinte desvio ocorreu: [descreva o que atrasou, quanto, quem foi afetado
e qual o impacto para o cliente].

O que sei até agora:
- [Fato 1]
- [Fato 2]
- [Fato 3]

Use o método DMAIC e entregue:
1) As causas-raiz mais prováveis com nível de confiança e o que ainda falta
   confirmar para cada uma
2) Ações corretivas priorizadas por impacto × facilidade de implementação
3) Indicadores de controle semanal
4) Tabela de riscos: descrição | probabilidade | impacto | severidade |
   mitigação | contingência | owner
Sinalize quando faltar dado em vez de preencher.
Termine com "Decisão recomendada (requer validação humana)".

**Passo 2 — Refinamento (após ler a resposta)**
[Corrija o que a IA entendeu errado ou acrescente contexto que faltou.]
Ex.: "A integração com tesouraria não foi surpresa — foi mencionada no
kick-off mas não documentada. Ajuste a causa raiz para falha de documentação
de escopo, não requisito novo."

**Passo 3 — Cenários de estimativa**
Com base nessa análise, gere 3 cenários para as [N] sprints restantes:
otimista, base e pessimista. Para cada um, explicite as premissas e o
prazo adicional em semanas.

**Passo 4 — Tabela de risco final**
Monte a tabela de riscos completa para o restante do projeto com os campos:
descrição | probabilidade | impacto | severidade | mitigação | contingência
| owner. Use os riscos que emergiram da análise.