### 19. Retomar a sessão de um PR
**Etapa:** 4 · Commit
**Ferramenta:** Claude Code

**Quando usar:** Ao voltar para revisar ou ajustar um PR depois de um tempo, ou ao retomar uma sessão anterior sem PR.

**Prompt:**

```
Preciso retomar o contexto da sessão que gerou o PR [número do PR]. Use claude --from-pr [número do PR] para abrir o seletor de sessões vinculadas a esse PR e retome a sessão correta.

Se não houver PR (foi uma sessão só local), use /resume para abrir o seletor de conversas anteriores e escolha a sessão certa pelo nome ou pela data.
```

**O que esperar de saída:** A sessão anterior retomada, com o Claude relembrando o contexto do PR ou da conversa escolhida.

**O que conferir:** Se o contexto retomado é realmente o da implementação certa (confirme pedindo um resumo do que foi feito até agora) antes de pedir qualquer ajuste novo.

**Próximo passo:** Nota de handoff para o time e para o próximo desenvolvedor
