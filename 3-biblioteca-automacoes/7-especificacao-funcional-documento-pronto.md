### 2. Especificação Funcional — Da URS ao documento pronto para o cliente

**O que automatiza:** transforma um requisito estruturado numa FS completa, formatada no padrão Ayesa, pronta para envio.

**Pré-requisitos:** URS já aprovada na pasta (Excel ou Word). Template de FS da Ayesa disponível.

**Prompt:**
```
Com base no requisito [REQ-ID] já aprovado nesta pasta, gere a Especificação 
Funcional completa no padrão Ayesa (10 seções: Identificação, Objetivo, Módulo 
e Transações SAP, Escopo, Fluxo Principal, Fluxos Alternativos, Regras de 
Negócio, Integrações, Critérios de Aceite, Pontos em Aberto).

Antes de escrever, analise o requisito de origem e liste internamente:
1. Quais fluxos alternativos a URS não cobre
2. Quais critérios de aceite estão vagos ou não mensuráveis
3. Quais integrações estão implícitas mas não declaradas

Marque toda transação SAP incerta como [VERIFICAR COM CLIENTE]. Marque toda 
lacuna que já vinha do requisito original como [HERDADO DO URS]. A Seção 10 
(Pontos em Aberto) nunca pode ficar vazia.

Salve como FS-[MÓDULO]-[SEQ]_[nome-descritivo].docx no template Word da Ayesa, 
nesta mesma pasta.
```

**O que esperar de saída:** documento Word formatado, pronto para revisão interna antes de envio ao cliente — não um rascunho para reformatar depois.