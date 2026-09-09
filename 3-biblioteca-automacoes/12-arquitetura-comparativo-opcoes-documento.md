### 7. Comparativo de Opções — Documento de decisão para comitê

**O que automatiza:** monta um comparativo estruturado para apresentação a um comitê técnico, antes de uma decisão de arquitetura ser formalizada.

**Pré-requisitos:** contexto já discutido (e-mails, atas, ou até uma conversa anterior no Chat/Cowork sobre o tema) disponível na pasta.

**Prompt:**
```
Monte um documento comparativo para apresentação ao comitê técnico sobre 
[ex.: "manter SAP ECC 6.0 vs. migrar para S/4HANA"] com base no que já foi 
discutido nesta pasta. Estruture como:

- Critérios de comparação (ex.: custo, prazo, risco, impacto operacional)
- Uma tabela cruzando cada opção contra cada critério
- Recomendação, se as fontes já apontarem uma direção clara — caso contrário, 
  deixe explícito que a decisão ainda está em aberto
- Riscos específicos de cada opção, não genéricos

Não invente números de custo ou prazo que não estejam nas fontes — marque 
como [A CONFIRMAR COM O CLIENTE] onde faltar dado real.

Salve como Comparativo_[tema-curto].pptx ou .docx, no formato que for mais 
adequado para apresentação (pergunte se não estiver claro).
```

**O que esperar de saída:** material pronto para levar a uma reunião de decisão, sem números inventados preenchendo lacunas reais.

---