### 26. Revisar contra a ET, segurança e performance
**Etapa:** Variação · Revisão de código
**Ferramenta:** Claude Code

**Quando usar:** Durante a revisão de um PR, para um parecer técnico estruturado.

**Prompt:**

```
Revise este PR contra a design/TS-MM-001.md e aponte, separadamente:

1. Aderência à especificação técnica: o que atende, o que não atende ou está ambíguo.
2. Segurança: ausência de AUTHORITY-CHECK, exposição de dados sensíveis, validações de entrada faltando.
3. Performance: SELECT dentro de loop, acessos a tabela sem índice adequado, lógica redundante.

Para cada ponto, cite o arquivo e o trecho, e classifique a gravidade (🔴 Crítico / 🟡 Atenção / 🟢 Sugestão).
```

**O que esperar de saída:** Um parecer dividido em aderência à TS, segurança e performance, com cada ponto classificado por gravidade e referenciado ao trecho do código.

**O que conferir:** Se os pontos 🔴 Crítico realmente impedem a aprovação do PR, e se nenhuma das três categorias ficou sem nenhum apontamento, mesmo que seja "nada encontrado".

**Próximo passo:** Resumo para a sua decisão
