### 20. Nota de handoff
**Etapa:** 4 · Commit
**Ferramenta:** Claude Code

**Quando usar:** Ao encerrar o trabalho em uma implementação que outra pessoa vai continuar ou revisar.

**Prompt:**

```
Escreva uma nota de handoff para quem for continuar este trabalho, cobrindo:

1. O que já foi implementado e onde (arquivos).
2. O que ainda falta, segundo o plano original.
3. Qualquer decisão tomada no meio do caminho que fugiu do plano, e por quê.
4. Pendências de verificação, se houver (reaproveite o registro de evidências desta sessão).

A nota deve ser curta o suficiente para alguém que não acompanhou a sessão entender o estado atual em poucos minutos.
```

**O que esperar de saída:** Uma nota de handoff curta e objetiva cobrindo o que foi feito, o que falta, decisões fora do plano e pendências de verificação.

**O que conferir:** Se alguém que não participou da sessão conseguiria entender o estado atual só lendo essa nota, sem precisar abrir o código.
