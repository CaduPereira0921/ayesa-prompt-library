### 1. Requisitos — Consolidação a partir de fontes dispersas

**O que automatiza:** transforma e-mails, atas e transcrições espalhadas numa URS estruturada única, sinalizando divergências entre fontes.

**Pré-requisitos:** pasta do projeto com os arquivos de e-mail/ata relevantes (ou conectores de e-mail/Teams ativos). Template URS da Ayesa disponível na mesma pasta.

**Prompt:**
```
Leia todos os e-mails e atas de reunião relacionados ao [nome do requisito ou 
módulo] nesta pasta do projeto [nome-do-projeto]. Para cada demanda encontrada:

1. Classifique como Funcional ou Não-Funcional
2. Estruture no formato REQ-[MÓDULO]-[SEQ com 3 dígitos]
3. Identifique o módulo SAP mais provável
4. Gere um critério de aceite mensurável (nunca vago)
5. Marque transações SAP como [VERIFICAR] quando não tiver certeza
6. Gere no mínimo 3 perguntas em aberto por requisito

Compare as demandas entre os diferentes arquivos-fonte e sinalize explicitamente 
qualquer conflito ou contradição encontrada, citando os dois arquivos de origem 
em conflito.

Preencha o arquivo URS_Template_Ayesa.xlsx com uma linha por requisito, incluindo 
a coluna "Origem (arquivo)" com o nome do documento de onde veio cada requisito. 
Salve como URS_[nome-do-projeto]_consolidado.xlsx na mesma pasta.
```

**O que esperar de saída:** planilha Excel com uma aba de requisitos estruturados e uma aba separada listando conflitos identificados entre fontes, cada um com recomendação de próximo passo (ex.: "realizar workshop de alinhamento entre Área X e Área Y").