### 12. Resumo Semanal Automático

**O que automatiza:** consolida o que avançou na semana e entrega um recap de uma página, em cadência, sem disparo manual.

**Pré-requisitos:** conectores de e-mail e Slack/Teams ativos para o projeto.

**Prompt (configurar via `/schedule`):**
```
Toda sexta-feira às 16h, consolide o que foi decidido e avançado esta semana 
no e-mail e no Teams sobre o projeto [nome-do-projeto]. Gere um recap de uma 
página com: principais avanços, decisões tomadas, e o que ficou pendente para 
a próxima semana. Envie por e-mail para [destinatários] com o assunto "Recap 
Semanal — [projeto] — [data]".
```

**O que esperar de saída:** um e-mail de recap chegando sozinho toda sexta, sem ninguém precisar lembrar de escrever.

---