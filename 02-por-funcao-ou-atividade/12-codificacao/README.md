# Codificação
> Responsáveis: Alexandre Bispo; Gabriel Aleixo; Osmar; Marcelo Aciolly; Francisco; Fernando Flores; Victor

## Prompts disponíveis

| Prompt | Framework | Caminho |
|---|---|---|
| Geração de código incremental (ABAP) | Iterative Prompting | `frameworks/cognitivos/04-iterative/exemplo-geracao-codigo-incremental.md` |
| Debug de erro em ABAP | Chain-of-Thought | `frameworks/cognitivos/01-chain-of-thought/exemplo-debug-abap.md` |
| Diagnóstico de falha em integração | Chain-of-Thought | `frameworks/cognitivos/01-chain-of-thought/exemplo-diagnostico-integracao.md` |
| Melhoria de performance SAP | PLAN | `frameworks/estruturais/08-PLAN/exemplo-melhoria-performance-SAP.md` |

## Fluxo recomendado

1. **Iterative** → gere o código em camadas (estrutura → lógica → otimização → documentação)
2. **Chain-of-Thought** → use para debug — o raciocínio passo a passo evita soluções precipitadas
3. **PLAN** → quando o problema é performance, limite as alternativas e meça o impacto
