### 2. Entender um objeto ABAP existente
**Etapa:** 1 · Explore
**Ferramenta:** Claude Code

**Quando usar:** Antes de alterar um objeto ABAP que você não escreveu ou não lembra em detalhe.

**Prompt:**

```
Leia o arquivo src/ZMM_NOTIF_GR_FI.abap e me explique, sem editar nada:

1. O que esse objeto faz, em linguagem simples.
2. Quais tabelas ele lê e quais ele grava.
3. Quais outros objetos do repositório chamam ou são chamados por ele (procure em src/ e em design/).
4. Quais parâmetros de entrada e saída ele tem.

Se encontrar alguma referência a REQ-MM-001, FS-MM-001 ou TS-MM-001 nos comentários do código, cite onde.
```

**O que esperar de saída:** Uma explicação do que o objeto faz, das tabelas envolvidas, das dependências com outros objetos e dos parâmetros, com referência aos requisitos ou especificações citados no código.

**O que conferir:** Se a explicação condiz com o que o código realmente faz (releia os trechos citados) e se alguma dependência relevante não foi encontrada.

**Próximo passo:** Levantar o impacto de uma mudança
