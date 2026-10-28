### 23. Perguntar em camadas
**Etapa:** Variação · Entender o código
**Ferramenta:** Claude Code

**Quando usar:** Para entender uma funcionalidade grande sem receber uma explicação só superficial ou só excessivamente detalhada.

**Prompt:**

```
Me explique o que o módulo [nome do processo ou funcionalidade] faz, em três camadas:

1. Uma frase, para alguém que não é técnico.
2. Um parágrafo, cobrindo as principais regras de negócio envolvidas.
3. Os detalhes técnicos: tabelas, objetos ABAP e fluxo de chamadas entre eles.

Pare depois da camada 1 e me pergunte se eu quero a próxima camada, em vez de entregar tudo de uma vez.
```

**O que esperar de saída:** A primeira camada da explicação (uma frase), seguida de uma pergunta se você quer avançar para a próxima camada.

**O que conferir:** Se a primeira camada realmente é compreensível sem conhecimento técnico, e se as camadas seguintes (quando pedidas) aprofundam sem repetir o que já foi dito.

**Próximo passo:** Registrar notas do que foi descoberto
