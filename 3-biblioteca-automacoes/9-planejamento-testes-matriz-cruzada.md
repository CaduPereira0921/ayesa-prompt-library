### 4. Planejamento de Testes — Matriz cruzada com critério de aceite

**O que automatiza:** gera os casos de teste e audita, na mesma tarefa, se cada critério de aceite da FS tem cobertura real.

**Pré-requisitos:** FS aprovada na pasta, com a seção de Critérios de Aceite preenchida.

**Prompt:**
```
A partir da FS [código-FS] nesta pasta, gere a matriz de casos de teste em 
Excel, cobrindo: caminho feliz, cada fluxo alternativo listado na FS, e casos 
de borda relevantes para o tipo de requisito.

Depois de gerar os casos, faça uma auditoria cruzada: liste cada critério de 
aceite mensurável da Seção 9 da FS e confirme se existe pelo menos um caso de 
teste cobrindo aquele critério especificamente. Se algum critério ficar sem 
cobertura, sinalize isso claramente numa aba separada "Gaps de Cobertura", sem 
inventar um caso de teste artificial só para preencher.

Salve como Plano_Testes_[código-FS].xlsx nesta pasta.
```

**O que esperar de saída:** planilha com casos de teste e uma segunda aba mostrando exatamente onde a cobertura está incompleta — não uma promessa vaga de "cobertura completa".