### 9. Estimativa e Cronograma — De escopo técnico a planilha de esforço

**O que automatiza:** transforma um escopo técnico já definido numa planilha de estimativa, pronta para o gerente de projeto revisar.

**Pré-requisitos:** TS ou documento de escopo técnico já aprovado na pasta.

**Prompt:**
```
Com base na TS [código-TS] nesta pasta, gere uma planilha de estimativa de 
esforço e cronograma. Para cada objeto técnico ou atividade identificada:

1. Estime o esforço em horas (baseado em complexidade indicada na TS: 
   baixa/média/alta)
2. Sugira uma sequência lógica de execução (o que depende do que)
3. Sinalize riscos que podem impactar o prazo (ex.: dependência de aprovação 
   externa, integração com sistema legado)

Marque toda estimativa como uma sugestão inicial, não um compromisso — o 
gerente de projeto ainda precisa validar antes de comunicar ao cliente.

Salve como Estimativa_[código-TS].xlsx nesta pasta.
```

**O que esperar de saída:** planilha de partida para a conversa com o gerente de projeto — não uma promessa de prazo já fechada.

---