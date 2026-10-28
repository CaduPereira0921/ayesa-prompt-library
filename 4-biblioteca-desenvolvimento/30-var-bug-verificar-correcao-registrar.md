### 30. Verificar a correção e registrar
**Etapa:** Variação · Corrigir bug
**Ferramenta:** Claude Code

**Quando usar:** Depois de corrigir um bug, antes de considerar o atendimento encerrado.

**Prompt:**

```
Rode as checagens disponíveis sobre a correção deste bug (revisão estática e o teste ABAP Unit que reproduz o caso) e me traga a evidência exata, não só "corrigido".

Depois, registre num formato curto: qual era o bug, qual foi a causa raiz, o que foi alterado e como foi verificado, para ficar relacionado ao chamado original.
```

**O que esperar de saída:** Evidência da verificação da correção (teste passando, revisão feita) seguida de um registro curto ligando bug, causa raiz, correção e verificação.

**O que conferir:** Se a evidência mostrada é do teste que reproduz este bug especificamente, e se o registro permitiria a outra pessoa entender o caso sem reabrir o chamado.
