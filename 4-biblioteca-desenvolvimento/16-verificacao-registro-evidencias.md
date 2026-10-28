### 16. Registro de evidências de verificação
**Etapa:** 3 · Verificação
**Ferramenta:** Claude Code

**Quando usar:** Ao final do ciclo de verificação de um passo ou de uma entrega, para deixar rastro do que foi checado.

**Prompt:**

```
Monte um registro de evidências de verificação para o que foi implementado nesta sessão, em formato de lista:

1. O que foi checado (revisão estática, testes ABAP Unit, rastreabilidade, padrões Ayesa).
2. O resultado de cada checagem.
3. Pendências que ficaram sem resposta ou sem checagem, se houver.

Esse registro é para acompanhar o commit ou o PR, não precisa ser um documento formal.
```

**O que esperar de saída:** Uma lista objetiva com o que foi checado, o resultado de cada checagem e as pendências em aberto.

**O que conferir:** Se o registro cobre todas as checagens feitas nesta sessão, não só a última, e se as pendências realmente estão sem resposta, não esquecidas.

**Próximo passo:** Revisar o diff antes do commit
