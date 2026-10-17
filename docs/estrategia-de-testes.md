# Estratégia de Testes | SauceDemo

## 1. Objetivo

Avaliar o comportamento funcional da aplicação SauceDemo, identificar possíveis defeitos e documentar os resultados de maneira reproduzível e rastreável.

## 2. Abordagens utilizadas

- **Testes funcionais:** validação de login, catálogo, carrinho e checkout.
- **Testes negativos:** investigação de entradas inválidas e comportamentos inesperados.
- **Testes exploratórios:** observação de comportamentos não previstos inicialmente.
- **Testes de responsividade:** avaliação da interface em diferentes larguras de janela.
- **Testes cross-browser:** comparação de comportamentos entre navegadores.

## 3. Evolução da estratégia

A estratégia foi construída progressivamente durante a exploração da aplicação. As etapas abaixo representam a evolução real da investigação, e não um planejamento integralmente definido antes da execução.

### Etapa 1 | Exploração inicial do checkout

A investigação começou pelas validações dos campos de identificação e pelo comportamento do checkout diante de entradas vazias ou incomuns.

Também foi observado que a aplicação permite concluir um pedido com o carrinho vazio, comportamento que depende de confirmação das regras de negócio para ser classificado definitivamente como defeito.

### Etapa 2 | Ampliação da cobertura funcional

A cobertura foi ampliada para autenticação, catálogo e carrinho.

Foram documentados cenários positivos e negativos, incluindo credenciais válidas, credenciais incorretas, inclusão e remoção de produtos e atualização do indicador do carrinho.

### Etapa 3 | Investigação exploratória de interface

Durante a validação de um login inválido, foi identificada uma possível falha visual na apresentação da mensagem de erro.

A observação originou um novo caso independente: SD-CT-16.

### Etapa 4 | Verificação entre navegadores

O comportamento visual foi reproduzido no Chrome, Edge, Safari e Vivaldi.

Em determinadas larguras de janela, parte da mensagem fica oculta. Ao reduzir a largura, o texto passa a ser exibido corretamente.

O resultado foi registrado como execução reprovada e defeito BUG-003.

## 4. Organização e rastreabilidade

- Casos de teste identificados por SD-CT.
- Execuções identificadas por SD-EX.
- Defeitos identificados por BUG.
- Evidências associadas às execuções.
- GitHub utilizado para documentação versionada.
- Notion utilizado para organização e acompanhamento.
- Jira destinado ao acompanhamento dos defeitos.

## 5. Limitações

Os requisitos oficiais e critérios de aceitação da aplicação não foram disponibilizados para esta investigação.

Por isso, os comportamentos que dependem de regras de negócio não confirmadas são classificados como inconclusivos, em vez de automaticamente considerados defeitos.

As documentações retrospectivas preservam a sequência real das descobertas.
