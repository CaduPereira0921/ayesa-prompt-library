### 4. Entrevista antes do plano
**Etapa:** 2 · Plan
**Ferramenta:** Claude Code

**Quando usar:** Antes de pedir um plano de implementação, quando o requisito ainda tem pontos em aberto.

**Prompt:**

```
Antes de montar qualquer plano de implementação, leia requirements/REQ-MM-001.md e design/FS-MM-001.md.

Não monte o plano ainda. Primeiro, me faça as perguntas que você precisa ter respondidas para planejar essa implementação com segurança: pontos ambíguos no requisito, decisões técnicas que dependem de mim, e qualquer suposição que você teria que assumir sem perguntar.

Liste as perguntas numeradas, da mais crítica para a mais secundária. Espere minhas respostas antes de propor o plano.
```

**O que esperar de saída:** Uma lista numerada de perguntas sobre o requisito e a especificação, sem nenhum plano ainda.

**O que conferir:** Se as perguntas realmente destravam decisões de implementação, e não são só uma repetição do que já está escrito na FS.

**Próximo passo:** Plano de implementação a partir da ET aprovada
