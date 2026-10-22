# SD-EX-20 | Registro exploratório: inclusão e remoção de produtos pela vitrine

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-20

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Vitrine / Catálogo
- **Caso relacionado:** [SD-CT-20](../casos-de-teste/SD-CT-20.md)
- **Natureza:** Registro retrospectivo de exploração manual anterior à formalização do caso.
- **Data da exploração:** 22/10/2026

**Objetivo:** documentar as alterações observadas no contador do carrinho e nos botões ao adicionar e remover dois produtos diferentes pela vitrine.

## Ambiente conhecido

- **Aplicação:** https://www.saucedemo.com/
- **Navegador, versão, sistema operacional e dimensões da janela:** não informados para esta exploração.

## Cobertura observada

Foi utilizada uma sequência de inclusão e remoção de dois produtos diferentes, denominados A e B. Seus nomes não foram informados.

A verificação contemplou os estados visíveis do contador numérico e dos botões na vitrine.

## Resultados por etapa

| Etapa | Ação / estado | Resultado observado |
|---|---|---|
| 1 | Estado inicial | Carrinho relatado como vazio, sem contador numérico e com os botões de A e B exibindo **Add to cart**. |
| 2 | Adição de A | Contador exibiu **1** e o botão de A mudou para **Remove**. |
| 3 | Adição de B | Contador exibiu **2** e ambos os botões exibiram **Remove**. |
| 4 | Remoção de A | Contador exibiu **1**, o botão de A retornou a **Add to cart** e B permaneceu selecionado, com **Remove**. |
| 5 | Remoção de B | Contador numérico desapareceu e ambos os botões retornaram a **Add to cart**. |

**Conclusão do registro:** todos os estados relatados corresponderam ao esperado para a sequência explorada. Essa correspondência não constitui aprovação de uma execução formal do SD-CT-20.

## Limitações

A exploração ocorreu antes da formalização do SD-CT-20. A associação ao caso é retrospectiva e não representa uma execução formal previamente planejada.

Os nomes dos produtos não foram informados, limitando sua identificação às referências A e B.

O conteúdo interno do carrinho não foi verificado. O estado inicial vazio foi relatado como contexto; os resultados documentados se limitam ao contador e aos botões da vitrine e não comprovam, por si só, o conteúdo do carrinho.

## Rastreabilidade

- **Caso relacionado:** [SD-CT-20](../casos-de-teste/SD-CT-20.md) — caso formalizado relacionado à sequência exploratória aqui documentada.
- **VIT-02 — Adição e remoção de produtos pela vitrine:** observação das alterações do contador e dos botões durante a inclusão e remoção de dois produtos diferentes.

`VIT-02` pertence ao planejamento. Sua associação a este registro indica correspondência com a exploração relatada, sem declarar execução formal do caso.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
