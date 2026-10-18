# SD-CT-09 | Usuário incorreto

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-09

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste funcional manual

## Pré-condição

Estar na tela de login da aplicação.

## Dados de teste

| Campo | Valor |
|---|---|
| Usuário | `standard_use` |
| Senha | `secret_sauce` |

O usuário informado é intencionalmente inválido para verificar a rejeição da autenticação.

## Passos

1. Preencher o usuário.
2. Preencher a senha.
3. Clicar em Login.

## Resultado esperado

A autenticação deve ser recusada, com apresentação de uma mensagem de erro.

## Rastreabilidade

- **Execução relacionada:** [SD-EX-09](../execucoes/SD-EX-09.md)
- **Investigação derivada:** [SD-CT-16 | Legibilidade da mensagem de erro](SD-CT-16.md)

Durante a investigação deste cenário, foi identificado um comportamento visual que motivou a criação de um caso independente de responsividade.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
