### 12. Rodar as checagens e trazer evidência
**Etapa:** 3 · Verificação
**Ferramenta:** Claude Code

**Quando usar:** Depois de qualquer implementação, antes de considerar o passo concluído.

**Prompt:**

```
Rode as checagens disponíveis para o que foi implementado neste passo: revisão estática do ABAP (sintaxe, convenções) e os testes ABAP Unit escritos para este passo.

Como este repositório não tem conexão com um sistema SAP, não me diga apenas "passou". Me mostre: o comando ou a revisão que você fez, e o resultado exato dela (trecho revisado, teste e o motivo de passar ou falhar).
```

**O que esperar de saída:** Evidência concreta da verificação: qual revisão ou teste foi feito e o resultado exato, não apenas a afirmação de que passou.

**O que conferir:** Se a evidência apresentada realmente corresponde ao código implementado neste passo, e não a um trecho antigo ou genérico.

**Próximo passo:** Revisor independente
