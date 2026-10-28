### 18. Mensagem de commit e descrição do PR
**Etapa:** 4 · Commit
**Ferramenta:** Claude Code

**Quando usar:** Ao preparar o commit final de uma implementação, para documentar a rastreabilidade.

**Prompt:**

```
Com base no diff revisado, escreva:

1. Uma mensagem de commit objetiva, no padrão deste repositório, citando REQ-MM-001 e TS-MM-001.
2. Uma descrição de PR com: o que foi implementado, por que (ligando ao REQ-MM-001), como foi verificado (cite a etapa de Verificação) e qualquer risco remanescente.

Não inclua dados fictícios como se fossem reais; mantenha os identificadores REQ-MM-001 e TS-MM-001 como estão.
```

**O que esperar de saída:** Uma mensagem de commit objetiva e uma descrição de PR estruturada, ambas citando o requisito e a especificação técnica envolvidos.

**O que conferir:** Se a mensagem de commit segue o padrão do repositório e se a descrição do PR realmente liga o que foi feito ao motivo (REQ) e à verificação, não só ao "o que".

**Próximo passo:** Retomar a sessão de um PR
