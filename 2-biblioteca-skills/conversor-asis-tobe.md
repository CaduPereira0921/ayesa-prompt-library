---
name: conversor-asis-tobe
description: "Ativar ao receber descrição de processo atual (AS-IS) do cliente — texto, ata ou transcrição. Mapeia o processo atual com gaps identificados, propõe processo TO-BE no SAP e deriva requisitos da diferença entre os dois, classificados por impacto."
---

# Skill: Conversor AS-IS → TO-BE — Ayesa Brasil
# Versão: 1.0 | Maintainer: Equipe de Qualidade Ayesa

## QUANDO ATIVAR
- "processo atual do cliente"
- "AS-IS"
- "como funciona hoje"
- "mapeamento de processo"
- Descrição narrativa de um processo de negócio existente

## COMPORTAMENTO FIXO

### PASSO 1 — MAPEAR O AS-IS
A partir do texto recebido, estruturar o processo atual em etapas sequenciais:
- Etapa | Responsável | Sistema usado | Tempo médio | Problema relatado

Identificar explicitamente: retrabalho, etapas manuais, pontos de erro frequente e reclamações mencionadas.

### PASSO 2 — PROPOR O TO-BE
Para cada etapa do AS-IS, propor a versão equivalente no SAP, priorizando SAP standard:
- Etapa TO-BE | Transação/processo SAP | O que muda em relação ao AS-IS | Tipo de solução (Standard/Customizing/Z)

### PASSO 3 — ANÁLISE DE GAP
Comparar AS-IS e TO-BE e classificar cada diferença:
- **Gap de processo**: o SAP standard já resolve, só precisa de adoção
- **Gap de configuração**: precisa de Customizing específico
- **Gap de desenvolvimento**: SAP standard não atende, precisa de objeto Z
- **Gap organizacional**: a mudança não é técnica, é de processo/cultura

Para cada gap, atribuir impacto: 🔴 Alto / 🟡 Médio / 🟢 Baixo

### PASSO 4 — DERIVAR REQUISITOS
A partir de cada gap de configuração ou desenvolvimento, gerar requisito formal no padrão URS Ayesa (REQ-ID, ator, gatilho, descrição, critério de aceite).

### PASSO 5 — RELATÓRIO FINAL
Apresentar:
1. Tabela AS-IS completa
2. Tabela TO-BE proposta
3. Análise de GAP com impacto
4. Requisitos derivados, prontos para validação com o cliente

## RESTRIÇÕES
❌ NUNCA propor TO-BE sem mapear o AS-IS primeiro
❌ NUNCA assumir que toda mudança requer desenvolvimento Z — verificar standard primeiro
✅ SEMPRE distinguir gap técnico de gap organizacional
✅ SEMPRE sinalizar quando a "solução" é apenas mudança de processo, sem necessidade de sistema

## FORMATO DE SAÍDA
Três tabelas sequenciais (AS-IS, TO-BE, GAP) seguidas da lista de requisitos derivados em formato URS padrão.
