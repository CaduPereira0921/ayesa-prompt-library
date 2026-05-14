# 4Is — Intenção, Instrução, Informação, Interação

## O que é

O framework **4Is** estrutura um prompt em quatro camadas básicas, garantindo que a IA entenda não apenas *o que fazer*, mas *por que*, *com o quê* e *o que fazer depois*.

| Camada | Pergunta que responde |
|---|---|
| 🎯 **Intenção** | Qual é o objetivo do pedido? |
| 📋 **Instrução** | O que exatamente a IA deve fazer? |
| 📂 **Informação** | Quais dados, contexto ou referências ela precisa? |
| 🔄 **Interação** | O que deve acontecer depois da resposta? |

---

## Quando usar

- Tarefas com objetivo claro mas que exigem contexto específico
- Quando você quer controlar o próximo passo após a resposta
- Ponto de entrada recomendado antes de migrar para frameworks mais complexos

---

## Exemplos Ayesa

### 📄 Análise de Edital de Licitação
> Contexto: Grupo 5 — Elaboração de proposta técnica e comercial

```
🎯 Intenção
Avaliar se a Ayesa deve concorrer a um edital de licitação para
implementação SAP, identificando riscos, oportunidades e requisitos
obrigatórios antes de qualquer decisão.

📋 Instrução
Leia o edital abaixo e entregue:
1. Resumo executivo: escopo, prazo e valor estimado
2. Requisitos técnicos obrigatórios (eliminatórios)
3. Riscos e pontos de atenção
4. Recomendação final: concorrer ou não, com justificativa objetiva

📂 Informação
[Cole aqui o texto completo do edital]

🔄 Interação
Se recomendar concorrer → gere já um índice sugerido para a proposta técnica.
Se recomendar não concorrer → aponte o critério decisivo e sugira o que
monitorar para editais futuros semelhantes.
```

---

## Contribuindo

Adicione novos exemplos seguindo o padrão acima:
- Indique o **contexto** (Grupo + tema)
- Mantenha as 4 camadas separadas e visíveis
- Prefira casos reais ou próximos do dia a dia da Ayesa
