### 14. Conferir contra o requisito
**Etapa:** 3 · Verificação
**Ferramenta:** Claude Code

**Quando usar:** Antes do commit, para garantir que a implementação resolve o requisito original, não só a especificação técnica.

**Prompt:**

```
Monte uma rastreabilidade simples entre requirements/REQ-MM-001.md, design/FS-MM-001.md, design/TS-MM-001.md e o código implementado nesta sessão:

1. Cada regra de negócio do REQ-MM-001 está refletida na FS-MM-001?
2. Cada item da FS-MM-001 está coberto por algo na TS-MM-001?
3. Cada item da TS-MM-001 tem um trecho de código correspondente?

Aponte qualquer item que quebre essa cadeia (existe no requisito, mas não chegou ao código, por exemplo).
```

**O que esperar de saída:** Uma tabela ou lista de rastreabilidade entre requisito, FS, TS e código, com qualquer quebra na cadeia destacada.

**O que conferir:** Se a rastreabilidade cobre os três documentos e o código, não só dois deles, e se as quebras apontadas são reais (vá direto ao trecho citado).

**Próximo passo:** Checar padrões Ayesa
