### 15. Checar padrões Ayesa
**Etapa:** 3 · Verificação
**Ferramenta:** Claude Code

**Quando usar:** Antes do commit, para checar problemas recorrentes de qualidade em código ABAP.

**Prompt:**

```
Revise o código implementado nesta sessão procurando especificamente por:

1. SELECT dentro de loop (deveria ser SELECT ... FOR ALL ENTRIES ou equivalente).
2. Ausência de AUTHORITY-CHECK em operações que deveriam ter controle de autorização.
3. Valores fixos no código (datas, códigos de empresa, nomes de tabela Z) que deveriam estar em uma tabela de configuração ou constante.

Para cada ocorrência, cite o arquivo, a linha (ou o trecho) e sugira a correção. Não corrija automaticamente, só liste.
```

**O que esperar de saída:** Uma lista de ocorrências dos três problemas, cada uma com arquivo, trecho e sugestão de correção, sem nenhuma edição automática.

**O que conferir:** Se as ocorrências listadas realmente existem no código (confira ao menos uma manualmente) e se nenhuma ocorrência real ficou de fora.

**Próximo passo:** Registro de evidências de verificação
