# Exemplo Iterative — Refinamento de Casos de Teste
> Grupo 3 · Testes · Perfil: Analista de QA

---

## 🔄 Rodada 1 — Cobertura básica

Gere os casos de teste principais para o processo de criação de ordem de compra no SAP MM. Foque no fluxo principal — sem exceções ainda.

---

## 🔄 Rodada 2 — Cobertura de exceções (usar após receber os casos básicos)

Agora adicione os cenários de exceção mais críticos:
- Fornecedor bloqueado
- Material sem estoque mínimo configurado
- Usuário sem alçada de aprovação para o valor do pedido
- Pedido duplicado dentro de 24 horas

---

## 🔄 Rodada 3 — Adaptação para automação (usar após validar todos os casos)

Reescreva os 5 casos de teste mais críticos no formato Gherkin (Given / When / Then) para que possam ser automatizados com Robot Framework ou similar.

---

## 🔄 Rodada 4 — Priorização para go-live (usar na reta final do projeto)

Com base nos casos gerados, selecione os 10 mais críticos para execução obrigatória antes do go-live, justificando a priorização por risco de negócio.
