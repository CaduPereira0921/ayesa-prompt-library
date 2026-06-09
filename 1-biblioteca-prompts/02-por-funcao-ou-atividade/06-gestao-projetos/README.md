# Gestão de Projetos
> Responsáveis: George; Moura; Eduardo Ribeiro; Bruno Lucena; Mariana

## Prompts disponíveis

| Prompt | Framework | Caminho |
|---|---|---|
| Análise de causa raiz (CAR) | 4Is | `frameworks/estruturais/01-4Is/exemplo-analise-causa-CAR.md` |
| Estimativa de esforço de projeto | RAIN | `frameworks/estruturais/02-RAIN/exemplo-estimativa-projeto.md` |
| Tomada de decisão (DAR) | FLOW | `frameworks/estruturais/05-FLOW/exemplo-tomada-decisao-DAR.md` |
| Comunicação de status ao cliente | RTF | `frameworks/estruturais/03-RTF/exemplo-comunicacao-status-cliente.md` |
| Comunicação de risco ao cliente | PIVO | `frameworks/estruturais/07-PIVO/exemplo-comunicacao-risco-cliente.md` |
| Gestão de conflito entre equipes | PIVO | `frameworks/estruturais/07-PIVO/exemplo-gestao-conflito-equipes.md` |
| Validação de estimativa de concorrente | Chain-of-Thought | `frameworks/cognitivos/01-chain-of-thought/exemplo-validacao-estimativa.md` |
| Questionamento de escopo | Socratic | `frameworks/cognitivos/02-socratic/exemplo-questionamento-escopo.md` |
| Auditoria de matriz de riscos | Meta-Cognition | `frameworks/cognitivos/03-meta-cognition/exemplo-auditoria-riscos.md` |
| Retrospectiva de projeto | Team Prompting | `frameworks/cognitivos/05-team-prompting/exemplo-retrospectiva-projeto.md` |
| Robustez de estimativa | Counter Example Hunt | `frameworks/verificacao/04-counter-example-hunt/exemplo-robustez-estimativa.md` |
| Contradições em proposta/cronograma | Contradiction Scan | `frameworks/verificacao/03-contradiction-scan/exemplo-proposta-escopo-cronograma.md` |

## Fluxo recomendado por situação

**Planejamento inicial:**
RAIN (estimativa) → FLOW (decisões) → Counter Example Hunt (validar estimativa)

**Durante o projeto:**
RTF (status semanal) → PIVO (comunicação de risco) → PIVO (conflitos)

**Encerramento:**
Team Prompting (retrospectiva) → 4Is (CAR pós-projeto)
