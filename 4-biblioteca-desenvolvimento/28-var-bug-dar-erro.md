### 28. Dar o erro
**Etapa:** Variação · Corrigir bug
**Ferramenta:** Claude Code

**Quando usar:** Ao reportar um bug para o Claude investigar, logo no início do atendimento.

**Prompt:**

```
Encontramos um erro em produção. Segue o dump anonimizado (ST22) e o contexto:

[Cole aqui o dump ST22 anonimizado, sem nomes de cliente ou dados reais]

Contexto: módulo [MM ou FI], objeto provável [nome do objeto, se souber], frequência do erro [sempre / às vezes / só em um cenário específico], e o que o usuário estava fazendo quando o erro ocorreu.

Antes de propor qualquer correção, me diga qual hipótese de causa você considera mais provável e por quê.
```

**O que esperar de saída:** Uma hipótese de causa provável para o erro, com justificativa baseada no dump e no contexto, antes de qualquer tentativa de correção.

**O que conferir:** Se a hipótese realmente explica o erro do dump, e não é um chute genérico, e se ela é testável no próximo passo.

**Próximo passo:** Reproduzir e corrigir com mudança mínima
