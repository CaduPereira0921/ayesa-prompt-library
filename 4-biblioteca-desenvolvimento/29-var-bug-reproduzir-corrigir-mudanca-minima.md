### 29. Reproduzir e corrigir com mudança mínima
**Etapa:** Variação · Corrigir bug
**Ferramenta:** Claude Code

**Quando usar:** Depois de ter uma hipótese de causa, para confirmar o bug e corrigi-lo sem abrir escopo demais.

**Prompt:**

```
Com base na hipótese de causa levantada, escreva um teste ABAP Unit que reproduza o bug (o teste deve falhar hoje, confirmando o problema).

Depois, implemente a correção mínima necessária para esse teste passar, sem alterar nenhum outro comportamento do objeto. Se a correção exigir uma mudança maior do que isso, pare e me explique por quê antes de continuar.
```

**O que esperar de saída:** Um teste que reproduz o bug e falha antes da correção, seguido de uma correção mínima que faz esse teste passar, sem alterações fora do necessário.

**O que conferir:** Se o teste realmente reproduz o cenário do dump original, e se a correção não alterou nada além do necessário (confira com /diff).

**Próximo passo:** Verificar a correção e registrar
