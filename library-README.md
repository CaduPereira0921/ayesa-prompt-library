# 📚 Ayesa Prompt Library

Biblioteca de prompts da trilha **Workshops de IA Generativa — Ayesa × ibp solutions**.

Repositório vivo — novos prompts adicionados a cada workshop.

---

## 🗂️ Como está organizado

### 1. Por Framework
Prompts organizados pela técnica de engenharia de prompt utilizada.

```
frameworks/
├── estruturais/      → definem a estrutura do prompt
│   ├── 01-4Is/
│   ├── 02-RAIN/
│   ├── 03-RTF/
│   ├── 04-RISE/
│   ├── 05-FLOW/
│   ├── 06-ROSE/
│   ├── 07-PIVO/
│   └── 08-PLAN/
├── cognitivos/       → definem como o modelo raciocina
│   ├── 01-chain-of-thought/
│   ├── 02-socratic/
│   ├── 03-meta-cognition/
│   ├── 04-iterative/
│   └── 05-team-prompting/
└── verificacao/      → auditam a própria resposta da IA
    ├── 01-fact-checklist/
    ├── 02-reference-injection/
    ├── 03-contradiction-scan/
    └── 04-counter-example-hunt/
```

### 2. Por Função ou Atividade
Índices organizados pelo processo de negócio da Ayesa. Cada pasta contém um README com os prompts recomendados e o fluxo de uso.

```
por-funcao/
├── 01-analise-editais/
├── 02-proposta-tecnica-comercial/
├── 03-busca-candidatos/
├── 04-selecao-candidatos/
├── 05-auditoria/
├── 06-gestao-projetos/
├── 07-analise-requisitos/
├── 08-especificacao-funcional/
├── 09-especificacao-tecnica/
├── 10-arquitetura-software/
├── 11-engenharia-reversa/
├── 12-codificacao/
├── 13-revisao-codigo/
├── 14-planejamento-testes/
├── 15-testes-automatizados/
├── 16-documentacao-testes/
└── 17-rastreabilidade/
```

---

## 🧭 Por onde começar?

**Não sei qual framework usar →** acesse `por-funcao/` e encontre sua atividade. O README indica os prompts recomendados e o fluxo de uso.

**Sei qual framework quero usar →** acesse `frameworks/` e vá direto à pasta do framework.

**Primeira vez usando a biblioteca →** leia o guia abaixo.

---

## 📖 Guia rápido de frameworks

### Estruturais — definem a estrutura do prompt

| Framework | Ideal para | Diferencial |
|---|---|---|
| **4Is** | Tarefas com objetivo claro e próximo passo definido | Controla o que fazer depois da resposta |
| **RAIN** | Análises com papel especialista e output delimitado | Exige número concreto de itens ou limite mensurável |
| **RTF** | Outputs com formato padronizado | O formato é tão importante quanto o conteúdo |
| **RISE** | Análises e revisões com metodologia definida | Explicita o processo e o padrão de qualidade |
| **FLOW** | Decisões e avaliações com critério de sucesso | Define o que significa "tarefa bem-feita" |
| **ROSE** | Criação de documentos com objetivo claro | Ponto de partida é a meta, não o material |
| **PIVO** | Comunicações sensíveis ou de crise | Único que define o tipo de raciocínio e o tom |
| **PLAN** | Resolução de problemas com soluções priorizadas | Limita alternativas e mede impacto |

### Cognitivos — definem como o modelo raciocina

| Framework | Ideal para | Diferencial |
|---|---|---|
| **Chain-of-Thought** | Debug, diagnóstico, análises complexas | Mostra o raciocínio passo a passo |
| **Socratic** | Levantamento de requisitos, validação de escopo | Inverte o fluxo — o modelo pergunta antes de responder |
| **Meta-Cognition** | Revisão crítica de qualquer documento gerado | O modelo audita a própria resposta |
| **Iterative** | Documentos complexos que precisam de refinamento | Constrói o resultado em camadas progressivas |
| **Team Prompting** | Decisões que impactam múltiplas áreas | Simula perspectivas diferentes em uma única interação |

### Verificação — auditam a resposta antes de agir

| Framework | Ideal para | Diferencial |
|---|---|---|
| **Fact-Checklist** | Propostas e análises com afirmações factuais | Separa fatos verificáveis de suposições |
| **Reference Injection** | Especificações e análises técnicas | Força citação de normas e padrões |
| **Contradiction Scan** | Documentos extensos com múltiplas seções | Encontra inconsistências internas |
| **Counter Example Hunt** | Decisões e estimativas antes de fechar | Testa a robustez lógica buscando exceções |

---

## 🔄 Versionamento

| Versão | Conteúdo |
|---|---|
| `v1.0` | Frameworks estruturais (4Is, RAIN, RTF, RISE, FLOW, ROSE, PIVO, PLAN) |
| `v1.1` | Frameworks cognitivos (Chain-of-Thought, Socratic, Meta-Cognition, Iterative, Team Prompting) |
| `v1.2` | Frameworks de verificação (Fact-Checklist, Reference Injection, Contradiction Scan, Counter Example Hunt) |
| `v1.3` | Índices por função/atividade (17 processos Ayesa) |

---

## 🏢 Contexto

Desenvolvido durante a trilha de 10 workshops de IA Generativa da Ayesa em parceria com a ibp solutions.

Dúvidas ou sugestões de novos prompts: abra uma _issue_ neste repositório.
