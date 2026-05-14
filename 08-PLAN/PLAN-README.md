# PLAN — Problem, Limit, Action, Number

## O que é

O framework **PLAN** estrutura o prompt para resolução de problemas com **alternativas limitadas** e um **indicador de impacto**. Força a priorização — em vez de listar tudo que é possível, define quantas soluções e qual o número que prova que funcionou.

| Elemento | Pergunta que responde |
|---|---|
| ⚠️ **Problem** | Qual questão precisa ser resolvida? |
| 🔒 **Limit** | Quantas alternativas ou soluções devem ser propostas? |
| ⚡ **Action** | Qual ação concreta o modelo deve tomar para cada alternativa? |
| 🔢 **Number** | Qual o indicador que mede o impacto de cada solução? |

---

## Quando usar

- Quando você quer soluções **priorizadas**, não listas exaustivas
- Situações de melhoria de processo onde o impacto precisa ser quantificado
- Quando o tomador de decisão precisa escolher entre opções limitadas
- Reuniões de apresentação onde "menos é mais"

## Diferencial em relação ao RAIN

| | RAIN | PLAN |
|---|---|---|
| Numeric Target | Mede o **tamanho do output** (ex: 5 riscos, 200 palavras) | Mede o **impacto da solução** (ex: redução de X dias) |
| Limit | Não tem | Define o **número de alternativas** propostas |
| Melhor para | Análises com output delimitado | Resolução de problemas com soluções priorizadas |

---

## Exemplos Ayesa

→ Veja os arquivos de exemplo nesta pasta.

---

## Contribuindo

- O *Limit* deve ser um número pequeno (2 a 5) — mais do que isso perde o foco
- O *Number* deve ser um indicador real e mensurável, não estimativa vaga
- Prefira problemas onde a priorização é genuinamente necessária
