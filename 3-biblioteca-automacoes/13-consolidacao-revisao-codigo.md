### 8. Consolidação de Revisão — Relatório único de pontos de atenção

**O que automatiza:** junta comentários de revisão de código vindos de fontes diferentes num relatório único e acionável para o desenvolvedor.

**Pré-requisitos:** exportação de comentários de PR, e-mails ou mensagens de Slack/Teams com o feedback de revisão, na pasta.

**Prompt:**
```
Leia os comentários de revisão de código nesta pasta — vindos do PR exportado, 
dos e-mails e das mensagens de Slack/Teams sobre [nome do módulo/feature]. 
Consolide tudo num relatório único de pontos de atenção para o desenvolvedor, 
organizado por:

1. Bloqueante — precisa ser corrigido antes do merge
2. Sugestão — melhoria recomendada, não bloqueante
3. Dúvida — pontos que precisam de esclarecimento antes de agir

Para cada item, cite a fonte original (quem comentou, onde) e o trecho de 
código ou linha referenciada, se identificável.

Salve como Relatorio_Revisao_[nome-do-módulo].docx nesta pasta.
```

**O que esperar de saída:** um único documento organizado por prioridade, em vez do desenvolvedor ter que abrir três ferramentas diferentes para juntar todo o feedback.

---