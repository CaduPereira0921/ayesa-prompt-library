## GRUPO 4 — Arquitetura, Desenvolvimento e Revisão de Código

### 6. Arquitetura — Consolidação em ADR formal

**O que automatiza:** transforma decisões de arquitetura discutidas informalmente num Architecture Decision Record rastreável.

**Pré-requisitos:** e-mails, atas ou transcrições onde a decisão foi discutida, na pasta do projeto.

**Prompt:**
```
Leia os e-mails e atas de reunião nesta pasta relacionados à decisão de 
arquitetura sobre [tema da decisão, ex.: "migração do módulo MM para 
S/4HANA"]. Gere um ADR (Architecture Decision Record) formal, contendo:

1. Contexto — por que essa decisão precisou ser tomada
2. Opções consideradas — cada uma com prós e contras, citados das fontes reais
3. Decisão tomada — e por quem, se identificável nas fontes
4. Consequências esperadas — técnicas e de negócio
5. Status — decidido / em aberto / revisão pendente

Se as fontes não deixarem claro algum desses pontos, marque como [VERIFICAR 
COM O RESPONSÁVEL] em vez de presumir.

Salve como ADR-[número sequencial]_[tema-curto].md nesta pasta.
```

**O que esperar de saída:** documento único, versionável em Git junto com o código, que qualquer pessoa nova no projeto consegue ler para entender por que uma decisão técnica foi tomada.

---