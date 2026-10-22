# SD-CT-19 | Exibição e consistência das informações dos produtos

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-19

## 1. Identificação e objetivo

- **Aplicação:** SauceDemo
- **Funcionalidade:** Vitrine / Catálogo
- **Tipo:** Teste funcional manual
- **Abordagem:** Procedimento reutilizável para cada produto.
- **Base do critério:** Critérios adotados para a investigação, sem especificação oficial disponível.

**Objetivo:** verificar a presença de nome, descrição, imagem e preço nos produtos da vitrine e a consistência desses atributos entre a listagem e os detalhes do mesmo produto.

## 2. Pré-condições

- Estar autenticado com uma conta válida.
- Ter acesso à listagem e aos detalhes dos produtos.
- Aguardar o carregamento das informações e imagens antes de avaliá-las.

## 3. Dados de teste

Utilizar os produtos disponíveis na vitrine durante a execução. Os seis produtos observados na exploração de 22/10/2026 são uma referência da investigação atual, não uma quantidade estabelecida por requisito oficial.

Identificar cada produto no registro de execução pelo nome exibido ou por outra referência inequívoca, caso o nome esteja ausente ou duplicado.

Não é necessário transcrever integralmente os atributos de todos os produtos. Registrar a identificação do produto e os resultados por atributo. Quando houver divergência, registrar os valores ou conteúdos completos envolvidos e a tela em que cada um foi apresentado.

A listagem será a referência para comparação com os detalhes, sem ser considerada fonte independente de correção absoluta.

## 4. Passos

1. Acessar a vitrine, aguardar o carregamento e identificar os produtos disponíveis. Registrar a quantidade encontrada e eventual diferença em relação aos seis produtos da exploração anterior.
2. Para cada produto, verificar na listagem a presença e a legibilidade do nome, da descrição e do preço, além do carregamento e da visibilidade da imagem.
3. Acessar os detalhes do mesmo produto, verificar os quatro atributos e comparar seu conteúdo com o apresentado na listagem. Retornar à listagem quando necessário para confirmar a comparação.
4. Registrar, em um único registro de execução, a identificação do produto e o resultado por atributo. Documentar ausências, falhas de carregamento ou divergências com informações suficientes para localizar e reproduzir o comportamento. Retornar à listagem e repetir o procedimento para os demais produtos.
5. Conferir que todos os produtos disponíveis foram considerados, sem omissões ou repetições, e registrar a cobertura efetiva, incluindo itens não avaliados e suas justificativas.

## 5. Resultados esperados e critérios de aprovação

Para cada produto:

- Nome e descrição devem estar preenchidos e legíveis nas duas telas.
- A imagem deve estar carregada e visível nas duas telas, sem indicação de falha de carregamento.
- O preço deve estar visível e legível nas duas telas.
- Nome e descrição devem manter o mesmo conteúdo entre listagem e detalhes.
- A imagem deve representar o mesmo conteúdo visual nas duas telas; diferenças de tamanho decorrentes da apresentação não caracterizam inconsistência.
- O preço deve manter o mesmo valor e a mesma indicação de moeda, quando apresentada, entre listagem e detalhes.

**Aprovação:** todos os critérios devem ser atendidos para todos os produtos disponíveis na execução.

A diferença em relação à referência de seis produtos não implica reprovação automática. Deve ser registrada junto à quantidade e à cobertura efetivamente avaliadas.

Uma ausência ou divergência confirmada representa não atendimento ao critério correspondente e deve ser registrada com a identificação do produto e do atributo afetado. Se algum produto não puder ser avaliado, a verificação incompleta não deve ser apresentada como aprovada; a causa e a cobertura efetiva devem constar na execução.

Textos com aparência de código não constituem, isoladamente, motivo de reprovação.

## 6. Escopo e limitações

O caso avalia a exibição dos quatro atributos e sua consistência entre listagem e detalhes. Não avalia ordenação, carrinho, checkout ou responsividade.

A exploração de **22/10/2026** foi utilizada como contexto para elaborar este caso. Suas observações não constituem resultados de uma execução formal deste procedimento.

A comparação entre telas pode identificar divergências, mas não comprova a correção absoluta dos dados: ambas podem apresentar a mesma informação incorreta. Sem especificação oficial ou referência independente confiável, a correção absoluta de nomes, descrições, imagens e preços permanece não determinada.

Os textos com aparência de código identificados durante a exploração devem permanecer como observações a investigar, sem classificação automática como defeitos.

Os resultados de todos os produtos devem compor um único registro de execução, permitindo identificar o produto, o atributo e a verificação que eventualmente falhou. Não é necessário criar um documento por produto.

Capturas de tela não são obrigatórias. Podem ser utilizadas quando ajudarem a demonstrar uma divergência ou um problema visual que o registro textual não descreva suficientemente.

## 7. Rastreabilidade

- **Execução relacionada:** [SD-EX-19](../execucoes/SD-EX-19.md) — registro exploratório anterior à formalização deste caso.

| Item de planejamento | Cobertura neste caso |
|---|---|
| VIT-01 — Exibição da identidade e do preço dos produtos | Verificação da presença e legibilidade do nome e do preço na vitrine. |
| VIT-03 — Consistência de identidade e preço entre listagem e detalhes | Comparação do nome e do preço entre as duas telas para cada produto. |
| VIT-05 — Exibição de imagens e descrições | Limitada à presença e legibilidade das descrições e à presença, carregamento e visibilidade das imagens na listagem e nos detalhes. |

Os identificadores `VIT` pertencem ao planejamento. `SD-CT-19` identifica este único caso de teste; os resultados de sua futura execução deverão ser registrados separadamente.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
