### 5. Plano de implementação a partir da ET aprovada
**Etapa:** 2 · Plan
**Ferramenta:** Claude Code

**Quando usar:** Com a Especificação Técnica (ET) já aprovada, antes de começar a codificar.

**Prompt:**

```
Ative o Plan mode (Shift+Tab no terminal, pode ser necessário apertar mais de uma vez até aparecer "plan"; ou o seletor de modo no Claude Code Desktop).

Leia requirements/REQ-MM-001.md, design/FS-MM-001.md, design/TS-MM-001.md e design/ARQ-MM-001.md. Depois, monte um plano de implementação para o que a TS-MM-001 descreve, contendo:

1. Lista dos arquivos que serão criados ou alterados.
2. Ordem recomendada de implementação, com justificativa.
3. Riscos técnicos e de regressão.
4. Critério de sucesso objetivo para cada etapa do plano.

Não implemente nada ainda. Esse plano é para eu revisar e aprovar antes de qualquer edição.
```

**O que esperar de saída:** Um plano estruturado com arquivos afetados, ordem de implementação, riscos e critério de sucesso por etapa, sem nenhuma edição de código.

**O que conferir:** Se o plano cobre todos os objetos citados na TS, se a ordem evita retrabalho e se os critérios de sucesso são verificáveis, não apenas "funciona".

**Próximo passo:** Revisar o plano antes de aprovar
