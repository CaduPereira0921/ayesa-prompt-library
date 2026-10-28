### 11. Registrar o aprendizado no CLAUDE.md
**Etapa:** 3 · Code
**Ferramenta:** Claude Code

**Quando usar:** Depois de descobrir, durante a implementação, uma regra ou particularidade do projeto que não estava documentada.

**Prompt:**

```
Durante esta sessão descobrimos uma regra que não estava no CLAUDE.md: [descreva a regra ou particularidade descoberta, por exemplo "o campo X da tabela Y nunca pode ser alterado diretamente, só pela função Z"].

Adicione essa regra ao CLAUDE.md, na seção apropriada, com uma frase curta e objetiva. Não reescreva o restante do arquivo.
```

**O que esperar de saída:** Uma nova linha ou bullet no CLAUDE.md, na seção correta, sem alterações no restante do conteúdo do arquivo.

**O que conferir:** Se a regra ficou clara e objetiva, e se nada mais no CLAUDE.md foi alterado além do necessário (confira com /diff).

**Próximo passo:** Rodar as checagens e trazer evidência
