### 13. Revisor independente
**Etapa:** 3 · Verificação
**Ferramenta:** Claude Code

**Quando usar:** Antes de considerar a implementação pronta para commit, para uma segunda opinião isenta.

**Prompt:**

```
Crie um arquivo em .claude/agents/revisor-independente.md para um subagente que só tem acesso de leitura (ferramentas Read, Grep e Glob), com a instrução de revisar o código implementado contra a design/TS-MM-001.md, sem poder editar nada.

Depois, use esse subagente para revisar o que foi implementado nesta sessão e me traga o parecer dele: o que atende à TS, o que não atende, e o que está ambíguo.
```

**O que esperar de saída:** O arquivo do subagente criado em .claude/agents/, e o parecer desse subagente sobre a aderência do código à TS-MM-001.

**O que conferir:** Se o subagente realmente não tem ferramentas de escrita no frontmatter do arquivo, e se o parecer aponta trechos específicos do código e da TS, não uma opinião genérica.

**Próximo passo:** Conferir contra o requisito
