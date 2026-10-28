### 8. Implementar um passo do plano, um de cada vez
**Etapa:** 3 · Code
**Ferramenta:** Claude Code

**Quando usar:** Durante a implementação, depois do plano aprovado, para manter cada mudança revisável.

**Prompt:**

```
Implemente apenas o passo 1 do plano aprovado. Não avance para o passo 2 antes de eu confirmar.

Ao terminar o passo 1, mostre o que foi alterado e explique como isso atende ao critério de aceite correspondente. Espere minha confirmação antes de seguir para o próximo passo.
```

**O que esperar de saída:** A implementação de um único passo do plano, com explicação de como ele atende ao critério de aceite, e a sessão parada esperando confirmação.

**O que conferir:** Se o Claude realmente implementou só o passo pedido (confira com /diff) e se a explicação cita o critério de aceite correto.

**Próximo passo:** Rodar as checagens e trazer evidência
