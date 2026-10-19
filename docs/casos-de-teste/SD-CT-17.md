# SD-CT-17 | Login: Validação de campos obrigatórios

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-17

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste funcional manual
- **Abordagem:** Teste parametrizado
- **Técnica:** Particionamento de equivalência
- **Base do critério:** Hipótese funcional adotada para o teste, sem acesso à especificação formal de requisitos.

## Objetivo

Verificar se a aplicação impede a autenticação quando o nome de usuário, a senha ou ambos não são informados.

## Pré-condição

Estar na tela de login da aplicação, sem autenticação ativa.

## Dados de teste

| ID | Usuário | Senha |
|---|---|---|
| D01 | Vazio | Vazia |
| D02 | `standard_user` | Vazia |
| D03 | Vazio | `secret_sauce` |

## Passos

Executar os passos para cada conjunto de dados:

1. Acessar a tela de login.
2. Garantir que os campos estejam no estado inicial, sem dados de uma tentativa anterior.
3. Preencher usuário e senha conforme o conjunto selecionado.
4. Clicar em Login.
5. Verificar o comportamento da aplicação.

## Resultado esperado

**Critério funcional adotado:** a aplicação deve impedir a autenticação quando o usuário ou a senha estiverem vazios.

Esse critério foi estabelecido a partir da finalidade da funcionalidade de login e não representa um requisito formal confirmado.

## Escopo e limitações

A aprovação deste caso considera exclusivamente o comportamento funcional de impedir a autenticação.

O conteúdo e a ordem das mensagens de erro, os destaques visuais e os ícones dos campos não fazem parte dos critérios de aprovação deste caso.

Esses comportamentos poderão ser registrados na execução como observações de interface ou usabilidade, sem classificação automática como defeitos.

## Rastreabilidade

- **Execução relacionada:** SD-EX-17 (a formalizar).

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
