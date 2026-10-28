### 17. Revisar o diff antes do commit
**Etapa:** 4 · Commit
**Ferramenta:** Claude Code

**Quando usar:** Imediatamente antes de pedir o commit, para revisar exatamente o que vai ser gravado.

**Prompt:**

```
Antes de qualquer commit, use /diff para me mostrar exatamente o que foi alterado nesta sessão.

Depois, revise você mesmo esse diff e aponte: alguma alteração que não estava no plano aprovado, qualquer arquivo que não devia ter sido tocado, e qualquer resquício de dado de teste ou comentário temporário que deveria ser removido antes do commit.
```

**O que esperar de saída:** O diff completo da sessão (via /diff) seguido de uma autorrevisão apontando alterações fora do plano, arquivos indevidos ou resquícios a remover.

**O que conferir:** Se o diff mostrado é realmente o diff completo da sessão (compare com git status) e se a autorrevisão não deixou passar nada óbvio.

**Próximo passo:** Mensagem de commit e descrição do PR ligando REQ e ET
