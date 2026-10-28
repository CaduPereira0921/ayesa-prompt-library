### 25. Explorar o PR de outra pessoa
**Etapa:** Variação · Revisão de código
**Ferramenta:** Claude Code

**Quando usar:** Ao receber um PR de outra pessoa para revisar, antes de dar qualquer parecer.

**Prompt:**

```
Use /code-review [número do PR] para revisar o PR. Antes de me dar o parecer, me explique em linguagem simples o que esse PR faz e quais arquivos ele toca, como se eu não tivesse lido o código ainda.
```

**O que esperar de saída:** Uma explicação em linguagem simples do que o PR faz e quais arquivos ele altera, antes de qualquer parecer técnico detalhado.

**O que conferir:** Se a explicação realmente ajuda a entender a intenção do PR antes de entrar nos detalhes, e se os arquivos citados batem com o PR real.

**Próximo passo:** Revisar contra a ET, segurança e performance
