# SD-CT-21 | Ordenação dos produtos na vitrine

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-21

## 1. Identificação e objetivo

- **Aplicação:** SauceDemo
- **Funcionalidade:** Vitrine / Catálogo
- **Tipo:** Teste funcional manual
- **Abordagem:** Teste parametrizado
- **Base do critério:** Significado das opções de ordenação apresentadas na interface, sem especificação oficial disponível.

**Objetivo:** verificar se a sequência completa dos produtos corresponde à ordenação selecionada por preço ou nome, nos dois sentidos.

## 2. Pré-condições

- Estar autenticado com uma conta válida e na vitrine.
- Aguardar o carregamento dos produtos.
- Ter o controle de ordenação disponível e pelo menos dois produtos com nomes e preços distintos.

## 3. Dados de teste

| ID | Opção de ordenação |
|---|---|
| D01 | Price (low to high) |
| D02 | Price (high to low) |
| D03 | Name (A to Z) |
| D04 | Name (Z to A) |

Utilizar os produtos disponíveis durante a execução, sem definir antecipadamente nomes ou preços. Os seis produtos observados na exploração de 22/10/2026 são uma referência, não uma quantidade estabelecida por requisito oficial.

## 4. Passos

1. Identificar os produtos disponíveis e registrar a quantidade inicial e referências suficientes para conferir que os mesmos produtos permanecem após cada ordenação.
2. Selecionar a opção do conjunto de dados e aguardar a atualização da listagem.
3. Percorrer toda a sequência exibida, na ordem de leitura da vitrine, comparando cada produto com o seguinte pelo atributo e sentido selecionados. Não limitar a conferência ao primeiro e ao último.
4. Conferir se os mesmos produtos permanecem na listagem, sem omissões ou duplicações introduzidas pela ordenação.
5. Registrar o resultado do conjunto e repetir os passos 2 a 4 para as demais opções. Em caso de divergência, registrar a opção, as posições e os produtos envolvidos, com os nomes ou preços necessários para demonstrá-la.

## 5. Resultados esperados e critérios de aprovação

| ID | Resultado esperado para a sequência completa |
|---|---|
| D01 | Cada preço deve ser menor ou igual ao preço seguinte, considerando os valores numericamente. |
| D02 | Cada preço deve ser maior ou igual ao preço seguinte, considerando os valores numericamente. |
| D03 | Cada nome deve preceder ou ser equivalente ao seguinte em ordem alfabética A–Z. |
| D04 | Cada nome deve suceder ou ser equivalente ao seguinte em ordem alfabética Z–A. |

Em todos os conjuntos, a opção selecionada deve corresponder à opção aplicada, e os produtos da listagem inicial devem ser preservados.

**Aprovação:** os quatro conjuntos devem atender aos resultados esperados em toda a sequência e preservar os produtos inicialmente disponíveis.

Preços iguais ou nomes equivalentes não exigem uma ordem específica entre si, pois não há regra de desempate confirmada.

Registrar os resultados por conjunto em um único registro de execução. Se algum conjunto não puder ser concluído, registrar a causa e a cobertura efetiva, sem apresentar a verificação incompleta como aprovada.

## 6. Escopo e limitações

O caso avalia a ordenação dos produtos na vitrine. Não confirma a correção absoluta de nomes ou preços, nem avalia detalhes dos produtos, carrinho ou checkout.

A quantidade diferente da referência de seis produtos não implica reprovação automática. A quantidade encontrada e a cobertura efetiva devem ser registradas.

Regras específicas para capitalização, acentos e caracteres especiais não foram disponibilizadas. Eventuais ambiguidades de ordenação envolvendo esses elementos devem ser registradas para investigação, sem classificação automática como defeito.

A exploração de **22/10/2026** contemplou os seis produtos nas quatro ordenações, sem divergências relatadas. Essa observação anterior não constitui execução formal deste caso, elaborado posteriormente.

Capturas de tela não são obrigatórias. Podem ser utilizadas quando ajudarem a demonstrar uma divergência que o registro textual não descreva suficientemente.

## 7. Rastreabilidade

- **Execução relacionada:** [SD-EX-21](../execucoes/SD-EX-21.md) — registro exploratório anterior à formalização deste caso.
- **VIT-06 — Ordenação por preço crescente e decrescente:** conjuntos D01 e D02.
- **VIT-07 — Ordenação por nome A–Z e Z–A:** conjuntos D03 e D04.

Os identificadores `VIT` pertencem ao planejamento. `SD-CT-21` identifica este caso de teste; os resultados de sua futura execução deverão ser registrados separadamente.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
