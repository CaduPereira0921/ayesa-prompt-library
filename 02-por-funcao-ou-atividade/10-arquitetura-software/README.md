# Arquitetura e Projeto de Software
> Responsáveis: Alexandre Bispo; Gabriel Aleixo; Osmar

## Prompts disponíveis

| Prompt | Framework | Caminho |
|---|---|---|
| Proposta de arquitetura de software | FLOW | `frameworks/estruturais/05-FLOW/exemplo-arquitetura-software.md` |
| Decisão de arquitetura de integração | FLOW | `frameworks/estruturais/05-FLOW/exemplo-tomada-decisao-DAR.md` |
| Validação de decisão de arquitetura | Socratic | `frameworks/cognitivos/02-socratic/exemplo-validacao-decisao-arquitetura.md` |
| Avaliação multi-perspectiva de arquitetura | Team Prompting | `frameworks/cognitivos/05-team-prompting/exemplo-decisao-arquitetura.md` |
| Diagnóstico de falha em integração | Chain-of-Thought | `frameworks/cognitivos/01-chain-of-thought/exemplo-diagnostico-integracao.md` |
| Refutação de decisão arquitetural | Counter Example Hunt | `frameworks/verificacao/04-counter-example-hunt/exemplo-decisao-arquitetura.md` |

## Fluxo recomendado

1. **FLOW** → proponha a arquitetura com win metric definido
2. **Socratic** → questione as premissas da decisão
3. **Team Prompting** → avalie pelos olhos do arquiteto, GP e cliente
4. **Counter Example Hunt** → tente refutar a decisão antes de fechar
