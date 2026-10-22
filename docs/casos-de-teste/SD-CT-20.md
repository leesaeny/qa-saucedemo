# SD-CT-20 | Inclusão e remoção de produtos pela vitrine

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-20

## 1. Identificação e objetivo

- **Aplicação:** SauceDemo
- **Funcionalidade:** Vitrine / Catálogo
- **Tipo:** Teste funcional manual
- **Base do critério:** Critérios funcionais adotados para a investigação, sem especificação oficial disponível.

**Objetivo:** verificar a atualização do contador do carrinho e dos botões dos produtos ao adicionar e remover dois produtos diferentes pela vitrine.

## 2. Pré-condições

- Estar autenticado com uma conta válida e na vitrine.
- Ter pelo menos dois produtos diferentes disponíveis.
- Iniciar com o carrinho vazio, sem contador numérico e com os botões dos produtos A e B exibindo **Add to cart**.

## 3. Dados de teste

Selecionar dois produtos diferentes disponíveis na vitrine:

- **Produto A:** primeiro produto a adicionar e remover.
- **Produto B:** segundo produto a adicionar e remover.

Registrar os nomes exibidos para identificar A e B na execução, sem definir antecipadamente nomes ou preços.

## 4. Passos e resultados esperados

Executar a sequência na mesma sessão, verificando o resultado após cada ação.

| Etapa | Ação | Resultado esperado |
|---|---|---|
| 1 | Verificar o estado inicial na vitrine. | Contador numérico ausente; A e B exibem **Add to cart**. |
| 2 | Clicar em **Add to cart** no produto A. | Contador exibe **1**; A exibe **Remove** e B permanece com **Add to cart**. |
| 3 | Clicar em **Add to cart** no produto B. | Contador exibe **2**; A e B exibem **Remove**. |
| 4 | Clicar em **Remove** no produto A. | Contador exibe **1**; A retorna a **Add to cart** e B permanece com **Remove**, indicando que continua selecionado. |
| 5 | Clicar em **Remove** no produto B. | Contador numérico desaparece; A e B exibem **Add to cart**. |

## 5. Critérios de aprovação

Todos os resultados esperados devem ser atendidos na sequência indicada.

Registrar o resultado de cada etapa em um único registro de execução. Em caso de divergência, identificar a etapa, o produto envolvido e o estado observado do contador ou botão.

Se o estado inicial não puder ser estabelecido ou a sequência não puder ser concluída, registrar a limitação, sem apresentar a verificação incompleta como aprovada.

## 6. Escopo e limitações

O caso avalia as ações realizadas pela vitrine e seus efeitos visíveis no contador e nos botões de A e B.

A conferência dos produtos dentro do carrinho será coberta separadamente. Os estados visuais avaliados neste caso não comprovam, por si só, o conteúdo interno do carrinho.

A sequência já foi observada exploratoriamente e correspondeu ao comportamento esperado. Essa observação anterior não constitui execução formal deste caso, elaborado posteriormente.

Capturas de tela não são obrigatórias. Podem ser utilizadas quando contribuírem para demonstrar uma divergência que o registro textual não descreva suficientemente.

## 7. Rastreabilidade

- **Execução relacionada:** [SD-EX-20](../execucoes/SD-EX-20.md) — registro exploratório anterior à formalização deste caso.
- **VIT-02 — Adição e remoção de produtos pela vitrine:** inclusão e remoção de dois produtos diferentes, com verificação do contador e dos botões correspondentes.

`VIT-02` pertence ao planejamento. `SD-CT-20` identifica este caso de teste; os resultados de sua futura execução deverão ser registrados separadamente.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
