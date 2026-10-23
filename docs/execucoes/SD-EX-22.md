# SD-EX-22 | Integridade dos produtos e preços no carrinho

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-22

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Carrinho
- **Tipo:** Teste funcional manual
- **Caso relacionado:** [SD-CT-22](../casos-de-teste/SD-CT-22.md)
- **Planejamento relacionado:** CAR-01
- **Data da execução:** 22/10/2026
- **Navegador:** Google Chrome
- **Resultado:** Aprovado no escopo funcional definido pelo SD-CT-22.

## Dados de teste

| Referência | Produto selecionado na vitrine | Preço registrado na vitrine |
|---|---|---|
| A | Sauce Labs Bike Light | US$ 9.99 |
| B | Sauce Labs Fleece Jacket | US$ 49.99 |
| C | Test.allTheThings() T-shirt (Red) | US$ 15.99 |

## Resultados esperados

- O carrinho deve conter exatamente A, B e C, cada um uma única vez, sem produtos adicionais ou duplicados.
- Os nomes devem corresponder aos apresentados na vitrine.
- Os preços devem manter o mesmo valor e a mesma indicação de moeda, quando apresentada, entre vitrine e carrinho.

## Resultados observados

Os três produtos foram adicionados pela vitrine e estavam presentes ao acessar o carrinho.

| Referência | Identidade no carrinho | Preço no carrinho |
|---|---|---|
| A | Nome correspondente ao apresentado na vitrine | US$ 9.99, igual ao registrado na vitrine |
| B | Nome correspondente ao apresentado na vitrine | US$ 49.99, igual ao registrado na vitrine |
| C | Nome correspondente ao apresentado na vitrine | US$ 15.99, igual ao registrado na vitrine |

Não havia produtos adicionais ou duplicados. Não foram relatadas divergências durante a execução.

## Status

**Aprovado no escopo funcional definido pelo SD-CT-22.**

O carrinho apresentou exatamente os três produtos selecionados, com identidade e preços consistentes com a vitrine. A conclusão se limita à combinação de produtos e às verificações documentadas nesta execução.

## Limitações

- A comparação demonstra consistência entre telas, sem comprovar a correção absoluta dos preços. Sem especificação oficial ou referência independente confiável, ambas as telas podem apresentar o mesmo valor incorreto.
- A versão do Chrome, o sistema operacional, as dimensões da janela e a versão da aplicação não foram informados.
- Não foram fornecidas capturas de tela ou outras evidências para associação a este registro.
- A aprovação não se estende a outras combinações de produtos nem às funcionalidades de contador, remoção, ordenação ou checkout.

## Rastreabilidade

- **Caso relacionado:** [SD-CT-22](../casos-de-teste/SD-CT-22.md) — Integridade dos produtos e preços no carrinho.
- **Planejamento relacionado:** CAR-01 — Integridade dos produtos e preços no carrinho.

`CAR-01` pertence ao planejamento; este registro documenta os resultados da execução do caso SD-CT-22.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
