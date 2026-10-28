### 27. Resumo para a sua decisão
**Etapa:** Variação · Revisão de código
**Ferramenta:** Claude Code

**Quando usar:** Ao final da revisão de um PR, para decidir entre aprovar, pedir ajustes ou recusar.

**Prompt:**

```
Com base em tudo que revisamos neste PR, me dê um resumo final para eu decidir: aprovar, pedir ajustes ou recusar.

O resumo deve ter, no máximo, os 3 pontos que realmente pesam na decisão (não repita a lista inteira de achados) e terminar com sua recomendação objetiva entre as três opções, com uma frase de justificativa.
```

**O que esperar de saída:** Um resumo com os três pontos mais relevantes da revisão e uma recomendação objetiva (aprovar, pedir ajustes ou recusar) com justificativa.

**O que conferir:** Se os três pontos escolhidos são realmente os que mais pesam, não os mais fáceis de explicar, e se a recomendação é coerente com a gravidade apontada na etapa anterior.
