### 1. Mapear o repositório
**Etapa:** 1 · Explore
**Ferramenta:** Claude Code

**Quando usar:** Ao abrir um repositório novo ou desconhecido, antes de pedir qualquer mudança.

**Prompt:**

```
Leia o CLAUDE.md na raiz do repositório e depois mapeie a estrutura do projeto, sem editar nada.

Quero entender:
1. Como as pastas requirements/, design/ e src/ estão organizadas e o que cada uma contém.
2. Quais convenções de nomenclatura os objetos ABAP seguem (prefixo Z, sufixos, padrão de nomes de função).
3. Quais dependências existem entre os arquivos de src/ (quem chama quem, quais tabelas são usadas).
4. Qualquer regra de projeto registrada no CLAUDE.md.

Não altere nenhum arquivo. Ao final, apresente um resumo em tópicos e aponte qualquer coisa que pareça inconsistente ou sem documentação suficiente.
```

**O que esperar de saída:** Um resumo da estrutura do repositório, das convenções de nomenclatura identificadas e das dependências entre os objetos ABAP, sem nenhuma edição de arquivo.

**O que conferir:** Se o resumo bate com o que você já sabe do repositório e se o Claude realmente não editou nada (confirme com git status).

**Próximo passo:** Plano de implementação a partir da ET aprovada
