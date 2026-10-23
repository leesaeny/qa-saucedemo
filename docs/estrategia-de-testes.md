# Estratégia de Testes | SauceDemo

## 1. Objetivo

Avaliar o comportamento funcional e visual da aplicação SauceDemo por meio de testes manuais, investigando possíveis defeitos e documentando os resultados de maneira reproduzível e rastreável.

Este projeto tem finalidade prática e educacional, com foco na aplicação de processos de Quality Assurance (QA).

## 2. Escopo e cobertura

A investigação contempla as funcionalidades de autenticação, catálogo de produtos, carrinho e checkout.

**Cobertura formalmente documentada nesta etapa:**

- Login com usuário inválido.
- Login com senha inválida.
- Login com credenciais válidas.
- Legibilidade da mensagem de erro em diferentes larguras de janela.

As demais funcionalidades foram exploradas durante o desenvolvimento do projeto, mas ainda não possuem, neste repositório, registros individuais de casos e execuções equivalentes.

Essa distinção evita apresentar atividades exploratórias como testes formalmente documentados.

## 3. Abordagens utilizadas

- **Testes funcionais:** verificação do comportamento da aplicação diante das entradas fornecidas.
- **Testes negativos:** avaliação de credenciais inválidas e respostas de erro.
- **Testes exploratórios:** identificação de comportamentos não previstos nos cenários iniciais.
- **Testes de responsividade:** observação da interface em diferentes larguras de janela.
- **Testes entre navegadores:** comparação do comportamento no Chrome, Edge, Safari e Vivaldi durante a investigação visual.

A execução automatizada ainda não faz parte da cobertura realizada.

## 4. Ambiente e limitações técnicas

A aplicação testada está disponível em https://www.saucedemo.com/.

Os testes foram realizados manualmente em navegadores desktop.

Na investigação da mensagem de erro, o comportamento foi observado em quatro navegadores. As três evidências visuais disponíveis foram capturadas no Google Chrome.

Não foram registrados de forma sistemática:

- As versões dos navegadores utilizados.
- As dimensões exatas das viewports.
- Informações completas sobre o ambiente de execução.

Essas limitações são explicitadas para preservar a precisão dos registros e orientar futuras investigações.

## 5. Evolução da investigação

A estratégia foi construída progressivamente durante a exploração da aplicação. A sequência abaixo representa a evolução real do trabalho, não um planejamento integralmente definido antes da execução.

### Etapa 1 | Exploração inicial do checkout

A investigação começou pelas validações dos campos de identificação e pelo comportamento do checkout diante de entradas vazias ou incomuns.

Foi observado que a aplicação permite concluir um pedido com o carrinho vazio. Como os requisitos oficiais não foram disponibilizados, esse comportamento permanece como uma questão a investigar, não como um defeito confirmado.

### Etapa 2 | Ampliação da exploração funcional

A investigação foi ampliada para autenticação, catálogo e carrinho.

Foram explorados comportamentos como autenticação válida e inválida, inclusão e remoção de produtos e atualização do indicador do carrinho.

Parte dessa exploração originou os casos de teste formalizados no repositório.

### Etapa 3 | Identificação de comportamento visual

Durante a execução de um cenário de login inválido, foi percebida uma possível falha na apresentação da mensagem de erro.

A observação motivou a criação de um caso independente para investigar sua legibilidade em diferentes larguras de janela.

### Etapa 4 | Investigação e registro do defeito

O comportamento visual foi observado no Chrome, Edge, Safari e Vivaldi.

Em determinadas larguras de janela, a mensagem aparece parcialmente oculta. Ao reduzir a largura, o texto torna-se legível.

A investigação resultou em uma execução reprovada, evidências comparativas e um relatório de defeito.

## 6. Critérios de avaliação e conclusão

Cada caso de teste documentado apresenta pré-condições, dados de entrada, passos e resultado esperado.

Os resultados de execução são classificados de acordo com a comparação entre o comportamento esperado e o observado.

A etapa atual de documentação é considerada concluída quando os casos executados possuem seus respectivos registros, os defeitos identificados estão documentados e as evidências disponíveis podem ser consultadas.

Essa conclusão documental **não significa que toda a aplicação foi testada ou está livre de defeitos**.

## 7. Organização e rastreabilidade

- **Casos de teste:** identificados pelo prefixo `SD-CT`.
- **Execuções:** identificadas pelo prefixo `SD-EX`.
- **Defeitos:** identificados pelo prefixo `BUG`.
- **Evidências:** imagens associadas às investigações documentadas.

### Registros relacionados à investigação do login

- [SD-CT-09 | Caso de teste](casos-de-teste/SD-CT-09.md)
- [SD-CT-16 | Caso de teste](casos-de-teste/SD-CT-16.md)
- [SD-EX-16 | Registro de execução](execucoes/SD-EX-16.md)
- [BUG-003 | Relatório de defeito](bugs/BUG-003.md)

O GitHub concentra a documentação pública e versionada dos testes. O acompanhamento operacional dos defeitos é realizado separadamente no Jira, em ambiente privado.

## 8. Requisitos e incertezas

Os requisitos oficiais e os critérios de aceitação da aplicação não foram disponibilizados para esta investigação.

Por isso, comportamentos dependentes de regras de negócio não confirmadas são tratados como inconclusivos até que existam informações suficientes para classificá-los.

As hipóteses sobre possíveis causas técnicas também não são apresentadas como diagnósticos comprovados.

## 9. Próximas etapas

- Ampliar a documentação funcional do catálogo, carrinho e checkout.
- Registrar informações mais precisas sobre os ambientes de execução.
- Investigar cenários adicionais e comportamentos ainda inconclusivos.
- Introduzir testes automatizados progressivamente, mantendo a separação entre resultados manuais e automatizados.

## 10. Cobertura e priorização da vitrine

Esta matriz propõe a ampliação da cobertura da vitrine de produtos. Ela representa o planejamento de verificações e não comprova execução ou cobertura formalmente documentada.

Os identificadores `VIT` pertencem exclusivamente ao planejamento. Não são casos de teste `SD-CT`. A formalização dos cenários deverá gerar casos com identificadores `SD-CT`, vinculados aos respectivos itens desta matriz.

| Identificador | Cenário | Prioridade inicial | Impacto de uma falha | Dependência de execução | Situação |
|---|---|---|---|---|---|
| VIT-01 | Exibição da identidade e do preço dos produtos | Alta | Pode impedir a identificação do produto ou apresentar informação de preço inadequada à decisão de compra. | Autenticação válida e acesso à listagem. | Explorado e documentado |
| VIT-02 | Adição e remoção de produtos pela vitrine | Alta | Pode impedir a seleção dos itens desejados ou manter itens indesejados no carrinho. | Acesso à listagem e estado inicial conhecido do carrinho. A remoção exige um produto previamente adicionado. | Explorado e documentado |
| VIT-03 | Consistência de identidade e preço entre listagem e detalhes | Alta | Divergências podem levar à seleção equivocada de produtos e comprometer a confiança nas informações exibidas. | Acesso à listagem e aos detalhes do mesmo produto. | Explorado e documentado |
| VIT-04 | Navegação da listagem para os detalhes | Média | Pode impedir o acesso às informações detalhadas do produto. | Autenticação válida e acesso à listagem. | Explorado e documentado |
| VIT-05 | Exibição de imagens e descrições | Média | Pode dificultar a compreensão das características e a identificação visual dos produtos. | Acesso à listagem e aos detalhes, conforme os elementos avaliados. | Explorado e documentado |
| VIT-06 | Ordenação por preço crescente e decrescente | Média | Pode dificultar a comparação e a busca de produtos por faixa de preço. | Listagem com produtos de preços distintos e controle de ordenação disponível. | Explorado e documentado |
| VIT-07 | Ordenação por nome A–Z e Z–A | Baixa | Pode dificultar a localização de produtos pelo nome. | Listagem com nomes distintos e controle de ordenação disponível. | Explorado e documentado |

A exploração está registrada em [SD-EX-19](execucoes/SD-EX-19.md), [SD-EX-20](execucoes/SD-EX-20.md) e [SD-EX-21](execucoes/SD-EX-21.md). A situação “Explorado e documentado” não representa aprovação de execuções formais.

### Critérios de priorização e sequência de execução

As prioridades são **provisórias e baseadas principalmente no impacto** de uma possível falha. A probabilidade de ocorrência das falhas ainda não foi estimada; portanto, esta matriz não constitui uma avaliação completa de risco.

- **Prioridade** indica a importância relativa de investigar cada cenário.
- **Risco** considera o impacto e a probabilidade de uma falha. Sua avaliação deverá ser refinada quando houver informações suficientes.
- **Dependência de execução** indica as condições necessárias para realizar uma verificação e pode influenciar a sequência dos testes, sem alterar automaticamente sua prioridade.

Por exemplo, o acesso aos detalhes é uma condição necessária para VIT-03, mas não exige a execução independente de VIT-04 como pré-requisito.

### Limite da comparação entre telas

A comparação de identidade e preço entre listagem e detalhes demonstra **consistência entre as telas**, mas não necessariamente a correção absoluta dessas informações. As duas telas podem apresentar o mesmo valor incorreto.

Para confirmar a correção absoluta dos preços, é necessária uma referência independente e confiável, como requisitos aprovados ou um catálogo de preços validado. Na ausência dessa referência, o resultado deve se limitar à consistência observada, registrando a correção absoluta como não determinada.

## 11. Cobertura e priorização do carrinho

Esta matriz registra o planejamento inicial da cobertura do carrinho. O identificador `CAR` pertence ao planejamento e não substitui o identificador do caso de teste `SD-CT`.

| Identificador | Cenário | Prioridade inicial | Impacto de uma falha | Dependência de execução | Situação |
|---|---|---|---|---|---|
| CAR-01 | Integridade dos produtos e preços no carrinho | Alta | Pode apresentar produtos diferentes dos selecionados, itens ausentes, adicionais ou duplicados, ou preços inconsistentes com a vitrine, comprometendo a conferência da seleção de compra. | Autenticação válida, carrinho inicialmente vazio e pelo menos três produtos distintos disponíveis. Inclusão dos três produtos pela vitrine, com identificação dos nomes e preços, e acesso ao carrinho. | Caso documentado; execução pendente |
| CAR-02 | Remoção individual e preservação dos demais produtos | Alta | A remoção incorreta pode manter produtos indesejados, excluir outros produtos ou alterar indevidamente a composição da compra. | Carrinho com pelo menos dois produtos diferentes previamente adicionados. | Explorado; caso formal pendente |
| CAR-03 | Preservação da seleção durante a navegação | Alta | A perda ou alteração da seleção pode comprometer a composição da compra. | Produtos previamente selecionados; acesso ao carrinho e retorno à vitrine. | Explorado; caso formal pendente |
| CAR-04 | Consistência do contador do carrinho | Média | Um contador incorreto pode transmitir uma quantidade equivocada de itens selecionados. | Estado inicial conhecido do carrinho e produtos disponíveis para inclusão e remoção. | Explorado; caso formal pendente |
| CAR-05 | Navegação entre carrinho, vitrine e checkout | Média | Falhas de navegação podem dificultar ou impedir a continuidade da jornada de compra. | Acesso ao carrinho e controles de navegação disponíveis. | Explorado; caso formal pendente |
| CAR-06 | Ordem de apresentação dos produtos no carrinho | Baixa | Uma ordem inesperada pode prejudicar a previsibilidade da apresentação, mas não foi identificado requisito oficial determinando a ordenação. | Pelo menos três produtos distintos adicionados, permitindo remover um item intermediário e adicioná-lo novamente. | Explorado; formalização a avaliar |

O CAR-01 está detalhado em [SD-CT-22](casos-de-teste/SD-CT-22.md). Os demais cenários ainda não possuem casos formais documentados. O registro SD-EX-22 permanece pendente; a documentação do caso não comprova execução ou aprovação.

As prioridades são provisórias, baseadas principalmente no impacto, pois a probabilidade das falhas ainda não foi estimada. Prioridade indica a importância relativa da investigação; risco considera impacto e probabilidade. As dependências indicam condições necessárias para executar o teste e podem orientar sua sequência, sem definir prioridade ou risco nem exigir a execução independente do SD-CT-20. Se uma falha impedir completamente o acesso ao checkout, a prioridade de CAR-05 deverá ser reavaliada.

Na exploração, a remoção individual preservou os demais produtos; ao retornar à vitrine, a seleção permaneceu e os botões exibiram **Remove**. O contador diminuiu corretamente após remoção diretamente no carrinho. O [SD-CT-20](casos-de-teste/SD-CT-20.md) cobre alterações do contador pela vitrine, com execução formal pendente. Também foi possível retornar à vitrine e avançar para o checkout.

Os produtos apareceram na ordem de inclusão, e um item removido e adicionado novamente apareceu no final. Essas observações são exploratórias e não representam execuções formais aprovadas. Sem requisitos oficiais, outra ordem de apresentação, ausência de subtotal ou checkout com carrinho vazio não constituem, por si só, defeitos confirmados.

A comparação de identidade e preço entre vitrine e carrinho demonstra consistência entre telas, sem confirmar a correção absoluta dos dados. Contador, remoção, ordenação e checkout não fazem parte de CAR-01.
