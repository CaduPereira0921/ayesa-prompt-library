# Exemplo Iterative — Geração de Código Incremental
> Grupo 4 · Desenvolvimento · Perfil: Desenvolvedor ABAP / .Net / Java

---

## 🔄 Rodada 1 — Estrutura base

Crie a estrutura base de um programa ABAP para leitura de pedidos de venda em aberto (tabela VBAK/VBAP), sem lógica de negócio ainda — apenas o esqueleto com seleção de dados e ALV básico.

---

## 🔄 Rodada 2 — Adição de lógica de negócio (usar após receber a estrutura)

Agora adicione a seguinte lógica ao programa:
- Filtrar apenas pedidos com status de entrega pendente
- Calcular o valor total em aberto por cliente
- Destacar em vermelho pedidos com atraso superior a 30 dias

---

## 🔄 Rodada 3 — Otimização de performance (usar após validar a lógica)

O programa está correto mas lento em volumes acima de 50 mil registros. Otimize:
- Substitua SELECTs aninhados por JOIN ou FOR ALL ENTRIES onde aplicável
- Adicione índices recomendados nos comentários do código

---

## 🔄 Rodada 4 — Documentação (usar antes de entregar)

Adicione comentários técnicos no código no padrão de documentação da Ayesa: cabeçalho com autor, data, descrição e histórico de alterações; comentários inline nas regras de negócio críticas.
