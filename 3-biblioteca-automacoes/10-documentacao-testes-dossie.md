### 5. Documentação de Testes — Dossiê consolidado, com agendamento

**O que automatiza:** consolida toda a jornada de um requisito (URS → FS → TS → Testes) num único PDF de sign-off, podendo rodar automaticamente em cadência.

**Pré-requisitos:** URS, FS, TS e plano de testes do mesmo requisito, todos na mesma pasta.

**Prompt (consolidação pontual):**
```
Consolide a URS, a FS, a TS e o Plano de Testes do requisito [REQ-ID] nesta 
pasta num único documento PDF de sign-off. Inclua um sumário executivo de uma 
página no início, resumindo: o que foi solicitado, o que foi especificado, 
como será testado, e quais pontos ainda estão em aberto entre todos os 
documentos.

Salve como Dossie_SignOff_[REQ-ID].pdf nesta pasta.
```

**Prompt (para transformar em tarefa agendada — digite `/schedule` depois de rodar o prompt acima com sucesso):**
```
Toda sexta-feira às 17h, gere um dossiê consolidado (URS + FS + TS + Plano de 
Testes) para cada requisito desta pasta que tenha todos os quatro documentos 
completos desde a última execução, seguindo o mesmo formato já validado. 
Salve cada um numa subpasta /dossies-sign-off/ com o nome do REQ-ID e a data.
```

**O que esperar de saída:** um PDF único por requisito, pronto para apresentar ao cliente — e, com o agendamento, isso passa a acontecer sozinho sem ninguém lembrar de rodar manualmente.

---