# SD-CT-22 | Integridade dos produtos e preços no carrinho

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-22

## 1. Identificação e objetivo

- **Aplicação:** SauceDemo
- **Funcionalidade:** Carrinho
- **Tipo:** Teste funcional manual
- **Prioridade:** Alta
- **Base do critério:** Critérios funcionais adotados para a investigação, sem especificação oficial disponível.

**Objetivo:** verificar se o carrinho contém exatamente os três produtos selecionados na vitrine, sem itens adicionais ou duplicados, mantendo a identidade e o preço apresentados na listagem.

## 2. Pré-condições

- Estar autenticado com uma conta válida.
- Iniciar com o carrinho vazio.
- Ter pelo menos três produtos distintos disponíveis na vitrine.
- Aguardar o carregamento das informações antes de avaliá-las.

## 3. Dados de teste

Selecionar três produtos distintos disponíveis na vitrine, denominados A, B e C.

Registrar durante a execução o nome e o preço exibidos na vitrine para cada produto, associando-os à respectiva referência A, B ou C. Não há nomes ou preços definidos antecipadamente.

Essas informações serão a referência para comparação com o carrinho, sem constituir uma fonte independente de correção absoluta dos dados.

## 4. Passos

1. Na vitrine, identificar os produtos A, B e C e registrar seus nomes e preços antes da inclusão.
2. Adicionar uma vez cada um dos três produtos selecionados, sem adicionar outros produtos.
3. Acessar o carrinho e aguardar o carregamento dos itens.
4. Conferir todos os itens apresentados, verificando se correspondem exatamente a A, B e C, sem produtos adicionais ou duplicados.
5. Comparar o nome e o preço de cada item com os registrados na vitrine e documentar os resultados em um único registro de execução. Em caso de divergência, identificar o produto, o atributo afetado e os valores apresentados em cada tela.

## 5. Resultados esperados

- O carrinho deve apresentar exatamente os três produtos selecionados: A, B e C.
- Cada produto selecionado deve aparecer uma única vez, sem itens adicionais ou duplicados.
- O nome de cada produto no carrinho deve corresponder ao nome registrado na vitrine, permitindo identificar o mesmo produto.
- O preço de cada produto deve manter o mesmo valor e a mesma indicação de moeda, quando apresentada, entre vitrine e carrinho.

## 6. Critérios de aprovação

Todos os resultados esperados devem ser atendidos para os três produtos.

A ausência de um produto selecionado, a presença de um item adicional ou duplicado, ou uma divergência de identidade ou preço representa não atendimento ao critério correspondente.

Se algum produto não puder ser avaliado ou o procedimento não puder ser concluído, registrar a causa e a cobertura efetiva, sem apresentar a verificação incompleta como aprovada.

## 7. Escopo e limitações

O caso avalia o conteúdo do carrinho e a consistência da identidade e do preço dos três produtos em relação à vitrine. Não contempla contador, remoção, ordenação ou checkout.

A comparação confirma consistência entre telas, mas não comprova a correção absoluta dos preços: ambas podem apresentar o mesmo valor incorreto. Sem especificação oficial ou referência independente confiável, a correção absoluta dos dados permanece não determinada.

Este documento define o procedimento e os critérios de teste; não registra resultados de execução.

Capturas de tela não são obrigatórias. Podem ser utilizadas quando ajudarem a demonstrar uma divergência que o registro textual não descreva suficientemente.

## 8. Rastreabilidade

- **Planejamento relacionado:** CAR-01 — Integridade dos produtos e preços no carrinho, prioridade alta.
- **Execução relacionada:** SD-EX-22 (pendente; a documentar).

`CAR-01` pertence ao planejamento. `SD-CT-22` identifica este caso de teste; os resultados de sua futura execução deverão ser registrados separadamente.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
