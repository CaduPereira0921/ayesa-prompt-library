### 10. Escrever os testes ABAP Unit primeiro
**Etapa:** 3 · Code
**Ferramenta:** Claude Code

**Quando usar:** Antes de implementar a lógica de um objeto, para travar o comportamento esperado primeiro.

**Prompt:**

```
Antes de implementar a lógica do passo atual do plano, escreva os testes ABAP Unit que vão validar os critérios de aceite [números dos critérios relacionados a este passo]. Os testes devem falhar agora, porque a lógica ainda não existe.

Não implemente a lógica ainda. Só os testes, e me mostre por que cada um falha no estado atual.
```

**O que esperar de saída:** Uma classe de teste ABAP Unit cobrindo os critérios de aceite indicados, que falha no estado atual do código, com explicação do motivo da falha.

**O que conferir:** Se cada teste corresponde a um critério de aceite específico e se o motivo da falha apontado é o esperado (ausência da lógica), não um erro de sintaxe no teste.

**Próximo passo:** Implementar um passo do plano, um de cada vez
