### 22. Subagente explorador
**Etapa:** Variação · Entender o código
**Ferramenta:** Claude Code

**Quando usar:** Para explorar uma parte grande ou desconhecida do código sem o risco de uma edição acidental.

**Prompt:**

```
Crie um arquivo em .claude/agents/explorador.md para um subagente com ferramentas somente de leitura (Read, Grep, Glob), cuja instrução seja explorar e explicar código sem nunca editar nada.

Use esse subagente para explorar a pasta src/ completa e me trazer um resumo de como os objetos se relacionam entre si.
```

**O que esperar de saída:** O arquivo do subagente criado em .claude/agents/explorador.md e um resumo de como os objetos de src/ se relacionam.

**O que conferir:** Se o frontmatter do subagente realmente não inclui ferramentas de escrita (Edit, Write, Bash) e se o resumo cobre todos os arquivos de src/.

**Próximo passo:** Perguntar em camadas
