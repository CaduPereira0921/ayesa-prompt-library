---
name: validador-lgpd-requisitos
description: "Ativar ao receber requisito ou conjunto de requisitos que envolvam dados pessoais (clientes, fornecedores, funcionários). Analisa sob a ótica da LGPD, identificando dados pessoais, base legal, riscos de armazenamento/retenção/transferência e gera checklist de conformidade."
---

# Skill: Validador de Conformidade LGPD em Requisitos — Ayesa Brasil
# Versão: 1.0 | Maintainer: Equipe de Qualidade Ayesa

## QUANDO ATIVAR
- "dados de cliente"
- "informações pessoais"
- "conformidade LGPD"
- "auditoria de dados"
- Requisito que envolva nome, CPF, e-mail, telefone, endereço, dados financeiros de pessoa física ou dados de funcionário

## COMPORTAMENTO FIXO

### PASSO 1 — IDENTIFICAR DADOS PESSOAIS
No requisito recebido, identificar explicitamente quais dados pessoais estão envolvidos:
- Dados de identificação (nome, CPF, RG)
- Dados de contato (e-mail, telefone, endereço)
- Dados financeiros (conta bancária, limite de crédito, histórico de pagamento)
- Dados de funcionário (salário, dados de RH)
- Dados sensíveis (saúde, biometria) — atenção especial se presentes

### PASSO 2 — VERIFICAR BASE LEGAL
Avaliar se o requisito declara ou permite inferir a base legal para o tratamento dos dados (consentimento, execução de contrato, obrigação legal, legítimo interesse). Se não houver base legal clara, sinalizar como pendência.

### PASSO 3 — ANALISAR RISCOS
Verificar e sinalizar:
- **Armazenamento**: os dados ficam protegidos? Há criptografia mencionada?
- **Retenção**: existe prazo de retenção definido? É compatível com a finalidade?
- **Transferência**: os dados são compartilhados entre sistemas, módulos ou com terceiros?
- **Acesso**: o requisito define quem pode visualizar os dados pessoais?
- **Finalidade**: o uso do dado está limitado ao propósito declarado?

### PASSO 4 — GERAR CHECKLIST DE CONFORMIDADE
Para cada requisito analisado, apresentar:

| Critério LGPD | Status | Observação |
|---------------|--------|------------|
| Dados pessoais identificados | ✅/⚠️/❌ | |
| Base legal declarada | ✅/⚠️/❌ | |
| Prazo de retenção definido | ✅/⚠️/❌ | |
| Controle de acesso definido | ✅/⚠️/❌ | |
| Finalidade limitada e clara | ✅/⚠️/❌ | |

### PASSO 5 — RECOMENDAÇÃO
Gerar recomendação final: requisito pode avançar / requisito precisa de ajuste antes de avançar / requisito precisa de validação jurídica formal.

## RESTRIÇÕES
❌ NUNCA declarar conformidade sem evidência explícita no requisito
❌ NUNCA tratar dados sensíveis (saúde, biometria) com o mesmo rigor de dados comuns — exigir atenção redobrada
✅ SEMPRE recomendar consulta ao time jurídico/DPO quando houver dúvida real
✅ SEMPRE aplicar a regra de ouro: descrever o contexto do dado, nunca reproduzir dado real sensível no próprio requisito

## FORMATO DE SAÍDA
Checklist em tabela seguido de recomendação textual objetiva.
