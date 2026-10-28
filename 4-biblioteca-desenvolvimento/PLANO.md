# Plano: aba "Desenvolvimento com Agentes" (v4.0)

Contexto para o Claude Code. Origem: workshop WS03 (IA Generativa na Engenharia de Software SAP, Ayesa x ibp solutions), bloco "Desenvolvimento com Agentes". Esta aba espelha o fluxo principal dos slides: Explore, Plan, Code, Verificação, Commit, mais quatro variações.

## 1. Objetivo

Criar a quarta biblioteca do site (ao lado de Prompts, Skills e Automações) com 30 prompts para uso no Claude Code, organizados pelo fluxo principal de desenvolvimento e pelas variações. Público: pessoal técnico (desenvolvimento, verificação).

## 2. Decisões já tomadas

- Nome da aba: "💻 Desenvolvimento com Agentes". Pasta: `4-biblioteca-desenvolvimento`.
- Versão: trocar o selo do cabeçalho de `v3.0 · Workshop 1` para `v4.0` (linha ~180 do `index.html`, classe `header-badge`).
- 30 prompts (lista na seção 5).
- Os prompts de teste assumem repositório com fontes ABAP exportados e sem conexão ao SAP: verificação = revisão estática e escrita de testes ABAP Unit, não execução no SAP.
- Idioma: português do Brasil. Sem travessão (em dash) nos textos.

## 3. Como o site funciona (já levantado)

- Os dados ficam dentro do `index.html`, em listas JavaScript: `prompts`, `skills`, `automacoes`, `funcoes`. As pastas com `.md` são espelho para navegação no GitHub. Todo item novo entra nos dois lugares.
- O site é público (GitHub Pages). Tudo anonimizado: cenário fictício Indústria Alfa, placeholders como [cliente] e [módulo]. Regra: "descreva o contexto, não os dados". Nunca colocar caminhos de pasta reais, nomes de clientes reais ou dados pessoais.
- Para incluir uma aba nova, mexer em cinco pontos do `index.html`:
  1. `<nav class="lib-nav">`: botão novo com `data-lib="desenvolvimento"` e `onclick="setLibrary('desenvolvimento')"`.
  2. `setLibrary()`: nova entrada em `cfgs` (título, subtítulo, placeholder da busca, classe do hero, contadores) e a exibição/ocultação da nova sidebar.
  3. Sidebar nova `sidebarDesenvolvimento` com filtros (copiar o padrão de `sidebarAutomacoes`).
  4. `render()` + `renderDesenvolvimento()` + `devCardHtml()` (copiar o padrão de `renderAutomacoes` e `autoCardHtml`).
  5. `openDevModal(id)` (copiar o padrão de `openAutoModal`), com blocos extras "O que esperar" e "O que conferir".
- CSS: criar `--dev` e `--dev-light` em `:root` e `.hero.hero-desenvolvimento`, seguindo `--auto` e `.hero-automacoes`. Escolher uma cor distinta das três existentes (navy/azul, verde e marrom já usados). Sugestão: tom de roxo ou petróleo.
- Não alterar nada das abas existentes, além do selo de versão e do que for estritamente necessário para o botão novo.

## 4. Molde de cada item

Objeto JavaScript (lista `desenvolvimento`, nova):

```js
{
  id: 1,
  nome: 'Mapear o repositório',
  ferramenta: 'Claude Code',
  etapa: 'explore',            // explore | plan | code | verificacao | commit | var-pequena | var-entender | var-revisao | var-bug
  etapaLabel: '1 · Explore',
  quando: 'Ao abrir um repositório novo ou desconhecido, antes de pedir qualquer mudança.',
  prompt: `...`,               // texto pronto para colar no Claude Code
  esperar: '...',              // o que esperar de saída
  conferir: '...',             // o que checar antes de seguir
  proximo: 'Plan: plano de implementação'   // opcional
}
```

Arquivo `.md` espelho (mesmo padrão das automações), por exemplo `01-explore-mapear-repositorio.md`:

```
### 1. Mapear o repositório
**Etapa:** 1 · Explore
**Quando usar:** ...
**Pré-requisitos:** ...
**Prompt:**
(bloco de código)
**O que esperar de saída:** ...
**O que conferir:** ...
**Próximo passo:** ...
```

Filtros da sidebar, em dois grupos:
- Fluxo principal: Explore (1), Plan (2), Code (3), Verificação (3 na numeração dos slides, ver nota), Commit (4).
- Variações: Tarefa pequena, Entender o código, Revisão de código, Corrigir bug.

Nota de numeração: nos slides, o fluxo é 1 Explore, 2 Plan, 3 Code, 4 Commit, e a Verificação faz parte do Code (ciclo código, verifica, refaz). Na sidebar, mostrar Verificação como subitem do Code ou como grupo próprio com a etiqueta "3 · Code / Verificação". Decisão de interface: usar um grupo próprio chamado "Verificação (dentro do Code)".

## 5. Lista dos 30 prompts

Cenário comum: Indústria Alfa S.A. (cliente fictício), SAP ECC 6.0, módulos MM e FI, fase atual "Especificação Técnica aprovada, desenvolvimento ABAP". Repositório de exemplo:

```
requirements/   REQ-MM-001.md            (somente leitura)
design/         FS-MM-001.md, TS-MM-001.md, ARQ-MM-001.md
src/            ZMM_NOTIF_GR_FI.abap, ZFM_VALIDA_FORNECEDOR_MM001.abap
CLAUDE.md       regra: ler requirements/ e design/ antes de agir
```

### Fluxo principal (20)

Explore (3)
1. Mapear o repositório: estrutura, convenções e dependências, sem editar nada.
2. Entender um objeto ABAP existente: o que faz, tabelas, quem o chama.
3. Levantar o impacto de uma mudança: o que mais seria afetado.

Plan (4), para usar no Plan mode
4. Entrevista antes do plano: o Claude pergunta o que falta antes de planejar.
5. Plano de implementação a partir da ET aprovada: arquivos, ordem, riscos e critério de sucesso.
6. Revisar o plano antes de aprovar: lacunas, riscos e perguntas.
7. Transformar o plano em critérios de aceite verificáveis.

Code (4)
8. Implementar um passo do plano, um de cada vez.
9. Corrigir um desvio: redirecionar o Claude no meio do caminho.
10. Escrever os testes ABAP Unit primeiro, a partir dos critérios de aceite.
11. Registrar o aprendizado no CLAUDE.md.

Verificação (5), dentro do Code
12. Rodar as checagens e trazer evidência (comando e saída; no cenário sem SAP, revisão estática e testes escritos).
13. Revisor independente: subagente só de leitura (tools Read, Grep, Glob) contra a ET.
14. Conferir contra o requisito: rastreabilidade REQ, FS, TS e código.
15. Checar padrões Ayesa: SELECT dentro de loop, AUTHORITY-CHECK, valores fixos no código.
16. Registro de evidências de verificação: o que foi checado, resultado e pendências.

Commit (4)
17. Revisar o diff antes do commit.
18. Mensagem de commit e descrição do PR ligando REQ e ET.
19. Retomar a sessão de um PR (`claude --from-pr`) e, sem PR, `/resume`.
20. Nota de handoff para o time e para o próximo desenvolvedor.

### Variações (10), reaproveitam os prompts acima por referência

Tarefa pequena (1)
21. Pedir direto um ajuste pontual (conferir o diff e commitar usam os prompts 17 e 18).

Entender o código (3)
22. Subagente explorador: criar e usar um para ler sem mudar nada.
23. Perguntar em camadas: do geral ao detalhe.
24. Registrar notas do que foi descoberto.

Revisão de código (3)
25. Explorar o PR de outra pessoa.
26. Revisar contra a ET, segurança e performance.
27. Resumo para a sua decisão (aprovar, pedir ajustes ou recusar).

Corrigir bug (3)
28. Dar o erro: dump (ex.: ST22) anonimizado e o contexto.
29. Reproduzir e corrigir com mudança mínima.
30. Verificar a correção e registrar (reaproveita 12 e 16).

## 6. Regras de qualidade dos prompts

- Escritos para o Claude Code (terminal e Desktop), em português, prontos para colar.
- Cada prompt cita o que o Claude deve ler primeiro (CLAUDE.md, requirements/, design/).
- Pedir evidência nas verificações (comando e saída), não só "passou".
- Plan mode: os prompts da etapa 2 funcionam com o Plan mode ativo (Shift+Tab no terminal, seletor de modo no Desktop).
- Comandos citados devem existir na versão atual do Claude Code. Evitar `/agents` para criar subagente: pedir ao Claude para criar o arquivo em `.claude/agents/`. Usar `/code-review`, `/diff`, `/rewind`, `/clear`, `/resume` e `claude --from-pr` com a descrição correta.
- Nada de dados reais. Exemplos com [cliente], [módulo], REQ-MM-001 etc.
- Testar cada prompt no Claude Code antes de publicar e registrar o resultado.

## 7. Etapas de execução

1. Ler o `index.html` e confirmar os cinco pontos de alteração (seção 3).
2. Escrever os 30 `.md` na pasta `4-biblioteca-desenvolvimento` e o README da aba.
3. Gerar a lista `desenvolvimento` no `index.html` a partir dos `.md` (ou escrever os dois juntos e conferir que o conteúdo é idêntico).
4. Implementar a aba (botão, hero, sidebar, cards, modal, busca) e atualizar o selo para `v4.0`.
5. Rodar o site local (`.claude/launch.json`: `npx serve -p 3000 .`) e conferir as quatro abas, a busca, os filtros e o botão Copiar.
6. Atualizar o `library-README.md` da raiz de `1-biblioteca-prompts` apenas se citar as bibliotecas (conferir antes).
7. Mostrar o diff ao Cadu. Só fazer commit e push com a aprovação dele.

## 8. Critérios de aceite

- Quatro abas funcionando; as três antigas sem mudança de comportamento.
- 30 itens na nova aba, com filtros por etapa e por variação, busca e Copiar.
- Selo `v4.0` no cabeçalho.
- Nenhum dado real; nenhum caminho de máquina; nenhum travessão.
- Contadores do topo e da sidebar batendo com a lista.
