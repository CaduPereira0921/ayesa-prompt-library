---
name: gerador-perguntas-blueprint
description: "Ativar ao se preparar para uma reunião de levantamento de requisitos ou Blueprint. Recebe o escopo do projeto e gera roteiro de perguntas estruturado por dimensão e por stakeholder, cobrindo processo, regras de negócio, exceções, volumes e conformidade."
---

# Skill: Gerador de Perguntas de Blueprint — Ayesa Brasil
# Versão: 1.0 | Maintainer: Equipe de Qualidade Ayesa

## QUANDO ATIVAR
- "vou para uma reunião de blueprint"
- "me ajude a preparar perguntas"
- "levantamento de requisitos [módulo]"
- "o que devo perguntar ao cliente sobre [processo]"

## COMPORTAMENTO FIXO

### PASSO 1 — IDENTIFICAR O ESCOPO
A partir do input, identifique: módulo(s) SAP envolvido(s), setor do cliente, fase do projeto (Blueprint inicial / refinamento / follow-up) e se há informação prévia disponível.

### PASSO 2 — GERAR PERGUNTAS POR DIMENSÃO
Estruturar perguntas obrigatórias nas seguintes dimensões:

**Processo atual (AS-IS)**
- Como o processo funciona hoje, passo a passo?
- Quais sistemas estão envolvidos atualmente?
- Quais são as principais reclamações sobre o processo atual?

**Regras de negócio**
- Existem regras de aprovação ou alçada?
- Há diferenças de processo por filial, planta ou tipo de cliente?

**Exceções**
- O que acontece quando o processo não segue o caminho padrão?
- Existem casos especiais ou clientes/fornecedores com tratamento diferenciado?

**Volumes e performance**
- Qual o volume médio diário/mensal de transações?
- Existem picos sazonais (fechamento, datas comerciais)?

**Integrações**
- Há sistemas legados ou terceiros envolvidos?
- Existe troca de dados com outras empresas do grupo?

**Perfis de acesso**
- Quem pode executar cada etapa do processo?
- Há necessidade de segregação de funções (SoD)?

**Conformidade**
- Existem requisitos fiscais, regulatórios ou de auditoria aplicáveis?
- Há políticas de retenção de dados a considerar?

**Critério de aceite**
- Como o cliente vai validar que o requisito foi atendido?

### PASSO 3 — ORGANIZAR POR STAKEHOLDER
Agrupar as perguntas indicando para qual perfil cada uma deve ser direcionada: Key User, Gestor de área, TI/Basis, Financeiro/Auditoria, Diretoria.

### PASSO 4 — PRIORIZAR
Marcar com 🔴 as perguntas críticas que, se não respondidas, impedem o avanço do Blueprint.

## RESTRIÇÕES
❌ NUNCA gerar perguntas genéricas que sirvam para qualquer módulo
❌ NUNCA omitir perguntas de conformidade/auditoria
✅ SEMPRE adaptar as perguntas ao módulo e setor informados
✅ SEMPRE incluir ao menos uma pergunta sobre critério de aceite mensurável

## FORMATO DE SAÍDA
Roteiro organizado por dimensão, com sub-agrupamento por stakeholder e marcação de prioridade.
