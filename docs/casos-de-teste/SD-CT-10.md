# SD-CT-10 | Senha incorreta

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-10

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste funcional manual

## Pré-condição

Estar na tela de login da aplicação.

## Dados de teste

| Campo | Valor |
|---|---|
| Usuário | `standard_user` |
| Senha | `secret_sauc` |

A senha informada é intencionalmente inválida para verificar a rejeição da autenticação.

## Passos

1. Preencher o usuário.
2. Preencher a senha.
3. Clicar em Login.

## Resultado esperado

A autenticação deve ser recusada, com apresentação de uma mensagem de erro.

## Rastreabilidade

- **Execução relacionada:** SD-EX-10

O resultado observado está documentado no registro de execução correspondente.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
