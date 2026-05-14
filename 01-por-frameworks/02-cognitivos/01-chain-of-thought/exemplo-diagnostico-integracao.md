# Exemplo Chain-of-Thought — Diagnóstico de Falha em Integração SAP
> Grupo 4 · Arquitetura e Desenvolvimento · Perfil: Arquiteto de Soluções / Consultor Técnico

---

A integração entre SAP S/4HANA e o sistema de e-commerce do cliente parou de funcionar após uma atualização no fim de semana. Pedidos feitos no e-commerce não estão chegando ao SAP como ordens de venda.

**Pense passo a passo antes de recomendar qualquer ação:**
1. Mapeie o fluxo completo da integração (e-commerce → middleware → SAP)
2. Liste os pontos onde a falha pode estar ocorrendo em cada camada
3. Para cada ponto, indique como verificar se é ali o problema (log, transação SAP, endpoint)
4. Ordene as hipóteses da mais à menos provável com base no contexto da atualização
5. Proponha o plano de diagnóstico — o que testar primeiro e por quê

Não sugira soluções antes de completar o diagnóstico passo a passo.
