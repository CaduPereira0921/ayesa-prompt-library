### 3. Especificação Técnica — Cruzando FS com histórico do projeto

**O que automatiza:** gera a TS já considerando decisões e dependências entre módulos registradas anteriormente no projeto, evitando retrabalho de integração.

**Pré-requisitos:** FS aprovada na pasta. Idealmente, também outras FS/TS já existentes do mesmo projeto, para permitir a checagem de dependência cruzada.

**Prompt:**
```
Com base na FS [código-FS] nesta pasta, gere a Especificação Técnica 
correspondente. Antes de escrever, revise as demais FS e TS já existentes 
nesta pasta e identifique se este requisito depende de, ou impacta, algum 
módulo já especificado anteriormente — cite explicitamente qual documento e 
qual ponto de dependência, se houver.

Estruture a TS cobrindo: objetos técnicos envolvidos (tabelas, programas, 
exits, BAdIs), complexidade estimada, e uma seção específica de "Integrações 
e Dependências" caso alguma tenha sido identificada no passo anterior.

Marque qualquer transação, tabela ou objeto técnico que você não tenha certeza 
absoluta como [VERIFICAR COM CONSULTOR TÉCNICO] — nunca invente nome de 
programa ou tabela Z.

Salve como TS-[MÓDULO]-[SEQ]_[nome-descritivo].docx nesta pasta.
```

**O que esperar de saída:** TS que já nasce ciente do contexto do projeto, não isolada — reduz a chance de descobrir uma dependência de integração só na fase de teste.