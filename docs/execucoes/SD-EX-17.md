# SD-EX-17 | Login: Validação de campos obrigatórios

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-17

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste funcional manual parametrizado
- **Caso de teste:** [SD-CT-17](../casos-de-teste/SD-CT-17.md)
- **Data da execução:** 19/10/2026
- **Ambiente:** Aplicação web, Chrome em macOS
- **Versão da aplicação e navegador:** Não identificadas
- **Resultado:** Aprovado no recorte funcional adotado

## Resultado esperado

A autenticação deve ser impedida quando o nome de usuário ou a senha estiverem vazios.

Esse é um critério funcional assumido para o teste, sem confirmação por especificação formal de requisitos.

## Resultados por conjunto de dados

| ID | Condição | Resultado observado | Avaliação funcional |
|---|---|---|---|
| D01 | Usuário e senha vazios | Login não realizado; `Epic sadface: Username is required` | Aprovado |
| D02 | Usuário preenchido e senha vazia | Login não realizado; `Epic sadface: Password is required` | Aprovado |
| D03 | Usuário vazio e senha preenchida | Login não realizado; `Epic sadface: Username is required` | Aprovado |

## Status

**Aprovado exclusivamente no recorte funcional definido.**

Nos três conjuntos de dados, a aplicação permaneceu na tela de login, sem autenticação bem-sucedida.

A aprovação não representa conformidade integral com os requisitos do produto, pois a especificação formal não foi disponibilizada.

## Observações de interface e usabilidade

Nos três cenários, ambos os campos apresentaram bordas vermelhas e ícones X, inclusive quando apenas um estava vazio.

As mensagens apresentadas variaram conforme os dados informados.

Esses comportamentos foram registrados como observações de interface e usabilidade, sem julgamento de conformidade ou classificação como defeito confirmado.

## Evidências

- **D01:** [Usuário e senha vazios](../../evidencias/login/login-campos-vazios-chrome-macos-2026-10-19.png)
- **D02:** [Senha vazia](../../evidencias/login/login-senha-vazia-chrome-macos-2026-10-19.png)
- **D03:** [Usuário vazio](../../evidencias/login/login-usuario-vazio-chrome-macos-2026-10-19.png)

## Limitações

- Não foi disponibilizada especificação formal dos requisitos de login.
- O critério de aprovação é funcional e foi explicitamente assumido.
- Não foram avaliadas a conformidade das mensagens de erro, a acessibilidade, a segurança ou o desempenho.
- As versões exatas do navegador e da aplicação não foram registradas.
- Não foram realizadas verificações de implementação ou chamadas internas de autenticação.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
