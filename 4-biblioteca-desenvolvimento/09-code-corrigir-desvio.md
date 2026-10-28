### 9. Corrigir um desvio
**Etapa:** 3 · Code
**Ferramenta:** Claude Code

**Quando usar:** Quando o Claude começa a implementar algo diferente do plano ou do critério de aceite combinado.

**Prompt:**

```
Pare. Isso não é o que foi combinado no plano: [descreva em uma frase o que saiu do combinado, por exemplo "você alterou a tabela errada" ou "isso não estava no passo atual"].

Desfaça essa parte com /rewind (ou me explique o que seria necessário desfazer manualmente) e volte para o passo correto do plano, respeitando o critério de aceite [número do critério].
```

**O que esperar de saída:** O Claude reconhecendo o desvio, desfazendo a parte incorreta com /rewind e retomando o passo certo do plano.

**O que conferir:** Se o /rewind realmente removeu a mudança indesejada (confira com /diff ou git status) e se a nova tentativa segue o critério de aceite citado.

**Próximo passo:** Escrever os testes ABAP Unit primeiro, a partir dos critérios de aceite
