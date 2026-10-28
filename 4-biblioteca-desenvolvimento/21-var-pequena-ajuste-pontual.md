### 21. Pedir direto um ajuste pontual
**Etapa:** Variação · Tarefa pequena
**Ferramenta:** Claude Code

**Quando usar:** Para um ajuste pequeno e bem definido, que não justifica passar pelo fluxo completo de Explore e Plan.

**Prompt:**

```
No arquivo src/ZFM_VALIDA_FORNECEDOR_MM001.abap, ajuste [descreva o ajuste pontual, por exemplo "a mensagem de erro quando o fornecedor está bloqueado, para incluir o código do bloqueio"]. É um ajuste pequeno e isolado, não precisa de plano.

Ao terminar, me mostre o /diff da alteração.
```

**O que esperar de saída:** O ajuste pontual implementado direto, com o /diff mostrando exatamente o que mudou.

**O que conferir:** Se a alteração ficou restrita ao que foi pedido (confira pelo /diff) e se nenhum outro comportamento do objeto foi afetado.

**Próximo passo:** Revisar o diff antes do commit
