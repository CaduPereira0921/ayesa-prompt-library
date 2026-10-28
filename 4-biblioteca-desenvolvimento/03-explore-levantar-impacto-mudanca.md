### 3. Levantar o impacto de uma mudança
**Etapa:** 1 · Explore
**Ferramenta:** Claude Code

**Quando usar:** Antes de aceitar um pedido de mudança, para saber o que mais seria afetado.

**Prompt:**

```
Quero alterar o objeto src/ZFM_VALIDA_FORNECEDOR_MM001.abap para incluir uma nova regra de validação (vou detalhar a regra depois). Antes disso, sem editar nada, levante o impacto dessa mudança:

1. Quais outros objetos do repositório chamam essa função.
2. Quais tabelas e campos esse objeto usa hoje, que poderiam ser afetados por uma regra nova.
3. Se existe algum caso de teste, especificação (design/) ou requisito (requirements/) que já descreve esse comportamento e precisaria ser atualizado junto.
4. Qualquer risco de regressão que você identifique.

Apresente o resultado como uma lista de impactos, do mais crítico para o menos crítico.
```

**O que esperar de saída:** Uma lista de impactos priorizada, cobrindo chamadores do objeto, tabelas e campos afetados, documentos que precisariam ser atualizados e riscos de regressão.

**O que conferir:** Se a lista cobre as pastas requirements/ e design/, não só o código, e se os riscos apontados fazem sentido para a mudança que você tem em mente.

**Próximo passo:** Entrevista antes do plano
