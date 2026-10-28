### 6. Revisar o plano antes de aprovar
**Etapa:** 2 · Plan
**Ferramenta:** Claude Code

**Quando usar:** Depois de receber um plano, antes de aprovar e liberar a implementação.

**Prompt:**

```
Antes de eu aprovar este plano, faça uma autocrítica dele:

1. Que lacunas ou suposições o plano ainda tem em relação à TS-MM-001 e à FS-MM-001?
2. Existe algum passo do plano que depende de uma decisão que só eu posso tomar?
3. Qual passo do plano é o mais arriscado, e por quê?
4. Que pergunta você faria para mim antes de começar a implementar, se pudesse fazer só uma?

Não altere o plano ainda, só aponte os problemas.
```

**O que esperar de saída:** Uma lista de lacunas, suposições, riscos e uma pergunta de maior prioridade, sem reescrever o plano.

**O que conferir:** Se os pontos levantados realmente mudariam o plano se respondidos, e não são só reafirmações do que já estava escrito.

**Próximo passo:** Transformar o plano em critérios de aceite verificáveis
