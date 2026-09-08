---
name: detector-conflitos-requisitos
description: "Ativar ao receber múltiplos requisitos ou um URS completo para verificação de consistência. Varre contradições, redundâncias e dependências circulares entre requisitos, sinalizando conflitos com recomendação de resolução."
---

# Skill: Detector de Conflitos de Requisitos — Ayesa Brasil
# Versão: 1.0 | Maintainer: Equipe de Qualidade Ayesa

## QUANDO ATIVAR
- "verifique conflitos"
- "esses requisitos são compatíveis?"
- "contradiction scan"
- Múltiplos requisitos ou múltiplas fontes (e-mails, atas) coladas juntas

## COMPORTAMENTO FIXO

### PASSO 1 — MAPEAMENTO
Liste todos os requisitos recebidos com REQ-ID (ou atribua um provisório se não houver).
Identifique a origem de cada um (documento, data, autor) quando disponível.

### PASSO 2 — VARREDURA DE CONFLITOS
Compare sistematicamente cada requisito com os demais buscando:
- **Contradição direta**: dois requisitos descrevem comportamentos opostos para a mesma situação
- **Contradição de responsável**: requisitos diferentes atribuem a mesma ação a atores diferentes
- **Redundância**: dois requisitos descrevem essencialmente a mesma coisa com IDs diferentes
- **Dependência circular**: REQ-A depende de REQ-B que depende de REQ-A
- **Contradição de critério**: critérios de aceite incompatíveis entre requisitos relacionados

### PASSO 3 — CLASSIFICAÇÃO DO CONFLITO
Para cada conflito encontrado, indicar:
- Severidade: 🔴 Bloqueante (impede sign-off) | 🟡 Atenção (precisa esclarecimento) | 🟢 Observação
- Requisitos envolvidos (REQ-IDs)
- Origem de cada versão conflitante
- Recomendação de resolução com justificativa

### PASSO 4 — RELATÓRIO FINAL
Gerar:
1. Tabela de conflitos identificados
2. Para cada conflito: o que diverge, por que importa, recomendação
3. Lista de perguntas que precisam ser respondidas pelo cliente para resolver
4. Indicação de quais requisitos podem seguir para aprovação sem bloqueio

## RESTRIÇÕES
❌ NUNCA decidir sozinho qual versão está "certa" sem dados suficientes
❌ NUNCA ignorar conflito por parecer pequeno — sempre reportar
✅ SEMPRE citar a origem exata de cada lado do conflito
✅ SEMPRE separar conflito real de mera diferença de detalhamento

## FORMATO DE SAÍDA
Tabela de conflitos com colunas: REQ-IDs envolvidos | Natureza do conflito | Severidade | Recomendação.
Seguida de detalhamento textual para os conflitos bloqueantes.
