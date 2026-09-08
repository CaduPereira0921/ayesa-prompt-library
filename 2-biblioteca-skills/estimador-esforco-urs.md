---
name: estimador-esforco-urs
description: "Ativar ao receber URS para dimensionamento de esforço. Para cada requisito, estima tipo de solução, complexidade e horas de análise/desenvolvimento/teste, entregando faixa de estimativa com sinalização de risco para requisitos incertos."
---

# Skill: Estimador de Esforço de URS — Ayesa Brasil
# Versão: 1.0 | Maintainer: Equipe de Qualidade Ayesa

## QUANDO ATIVAR
- "quanto esforço"
- "estime o URS"
- "sizing dos requisitos"
- "quantas horas isso vai levar?"

## COMPORTAMENTO FIXO

### PASSO 1 — CLASSIFICAÇÃO DO TIPO DE SOLUÇÃO
Para cada requisito, determinar:
- **Configuração (Customizing)**: ajuste de parâmetro SAP standard — menor esforço
- **Customização leve**: ajuste de layout, variante, relatório — esforço médio
- **Desenvolvimento Z**: programa, BAdI, user exit customizado — maior esforço
- **A verificar**: quando não há informação suficiente para classificar com segurança

### PASSO 2 — ATRIBUIÇÃO DE COMPLEXIDADE
Classificar como P (Pequeno) / M (Médio) / G (Grande) considerando:
- Quantidade de regras de negócio envolvidas
- Número de módulos SAP integrados
- Existência de exceções e fluxos alternativos
- Dependência de objetos não confirmados [VERIFICAR]

### PASSO 3 — ESTIMATIVA DE HORAS
Para cada requisito, estimar:
- Horas de análise/especificação
- Horas de desenvolvimento (se aplicável)
- Horas de teste unitário
- Total por requisito

Apresentar em 3 faixas: Conservadora (pior caso) / Base (mais provável) / Otimista (melhor caso)

### PASSO 4 — SINALIZAÇÃO DE RISCO DE ESTIMATIVA
Marcar requisitos com 🔴 Alta incerteza quando:
- Transação SAP está marcada [VERIFICAR]
- Requisito depende de decisão do cliente ainda não tomada
- Requisito tem múltiplas interpretações possíveis

### PASSO 5 — RESUMO EXECUTIVO
Gerar:
1. Tabela por requisito: REQ-ID | Tipo | Complexidade | Horas (faixa) | Risco da estimativa
2. Total geral do projeto nas 3 faixas
3. Lista de requisitos que precisam de validação técnica antes de fechar estimativa

## RESTRIÇÕES
❌ NUNCA estimar sem declarar a premissa usada
❌ NUNCA tratar requisito [VERIFICAR] como estimativa confiável
✅ SEMPRE separar estimativa de análise da estimativa de desenvolvimento
✅ SEMPRE indicar quando SAP standard pode reduzir o esforço estimado

## FORMATO DE SAÍDA
Tabela detalhada por requisito seguida de resumo executivo com totais e riscos.
