### 7. Transformar o plano em critérios de aceite verificáveis
**Etapa:** 2 · Plan
**Ferramenta:** Claude Code

**Quando usar:** Depois de aprovar o plano, antes de começar a implementação, para travar o que significa "pronto".

**Prompt:**

```
Com o plano aprovado, transforme cada etapa dele em um critério de aceite verificável, no formato "dado X, quando Y, então Z". Cada critério precisa poder ser confirmado por um teste ABAP Unit ou por uma inspeção direta do código, não por uma opinião.

Numere os critérios e relacione cada um com o trecho da FS-MM-001 ou TS-MM-001 que ele cobre.
```

**O que esperar de saída:** Uma lista numerada de critérios de aceite no formato dado/quando/então, cada um relacionado a um trecho da FS ou TS.

**O que conferir:** Se cada critério é realmente testável, não vago, e se, juntos, cobrem todo o escopo do plano aprovado.

**Próximo passo:** Implementar um passo do plano, um de cada vez
