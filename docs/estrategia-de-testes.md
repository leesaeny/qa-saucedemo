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
