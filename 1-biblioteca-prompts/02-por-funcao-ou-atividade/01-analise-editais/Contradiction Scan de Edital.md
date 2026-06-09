NOME DO PROMPT: Contradiction Scan de Edital
QUANDO USAR: após a leitura inicial do edital, antes de
qualquer decisão de concorrer ou de montar proposta.
FRAMEWORK: Fact-Checklist + Contradiction Scan combinados.

─────────────────────────────────────────────────────────

PROMPT:

Você recebeu o edital [NOME/NÚMERO] para análise.
Antes de qualquer recomendação, execute um
Contradiction Scan sistemático em três camadas:

CAMADA 1 — NARRATIVA vs. NÚMERO
Procure divergências entre o texto corrido e
os valores, percentuais ou prazos em tabelas
ou fórmulas do mesmo documento.

Para cada divergência encontrada, informe:
· Trecho A: [texto exato + cláusula]
· Trecho B: [valor/tabela + cláusula]
· Impacto estimado: financeiro ou operacional
· Ação recomendada: solicitar esclarecimento
  formal antes da sessão de disputa

CAMADA 2 — CLÁUSULA vs. CLÁUSULA
Procure requisitos que se contradizem entre si
dentro do mesmo instrumento. Exemplos típicos:
· Prazo de execução na cláusula X vs.
  cronograma no Anexo Y
· Vedação de subcontratação vs. exigência
  de perfil que a empresa não pode ter sozinha
· Penalidade definida em dois valores diferentes
  em seções distintas

Para cada contradição, informe:
· Cláusula A: [número + trecho relevante]
· Cláusula B: [número + trecho relevante]
· Qual prevalece (se há hierarquia indicada)
· Risco se não esclarecido antes da proposta

CAMADA 3 — EDITAL vs. ANEXOS
Compare as exigências do corpo do edital com
os documentos anexos (TR, memorial descritivo,
minuta de contrato, cronograma).

Para cada divergência, informe:
· O que o edital diz: [cláusula]
· O que o anexo diz: [referência]
· Qual documento prevalece hierarquicamente
· Impacto na precificação ou na habilitação

─────────────────────────────────────────────────────────

FORMATO DE SAÍDA:

Tabela por camada:
Contradição | Cláusula A | Cláusula B |
Impacto (🔴 Alto / 🟡 Médio / 🟢 Baixo) |
Ação recomendada

Ao final: total de contradições por camada
e prazo limite para protocolar esclarecimentos.

─────────────────────────────────────────────────────────

EXEMPLO DE USO (baseado no edital SESI-SP 804/2025):

Input:
"Execute o Contradiction Scan no edital anexo."

Output esperado — Camada 1:
Contradição: teto de glosa mensal
Cláusula A: 3.3.29.1 narrativa — "vinte por cento"
Cláusula B: 3.3.29.1 tabela — "25%"
Impacto: 🔴 Alto — diferença de R$ 347k/ano
          no pior cenário de SLA acumulado
Ação: protocolar esclarecimento formal até
      [data limite do edital]

─────────────────────────────────────────────────────────

RESTRIÇÃO:
Nenhuma contradição deve ser assumida como
"erro óbvio" sem esclarecimento formal.
O órgão pode ter intenção em qualquer das versões.
A ação correta é sempre protocolar a dúvida —
nunca interpretar sozinho e precificar com base
na versão mais favorável sem registro.