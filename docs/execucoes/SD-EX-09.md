# SD-EX-09 | Usuário incorreto

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-09

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste funcional manual
- **Caso de teste:** [SD-CT-09](../casos-de-teste/SD-CT-09.md)
- **Data da execução:** Não registrada
- **Resultado:** Aprovado

## Resultado esperado

A autenticação deve ser recusada, com apresentação de uma mensagem de erro.

## Resultado observado

A autenticação foi recusada. A aplicação exibiu uma mensagem de credenciais inválidas e destacou os campos em vermelho.

## Status

**Aprovado.**

O comportamento de rejeição das credenciais inválidas correspondeu ao resultado esperado para este caso.

## Investigação complementar

Durante a investigação, foi identificado um comportamento visual na apresentação da mensagem de erro.

Esse comportamento motivou um teste independente de responsividade, sem alterar o resultado funcional desta execução.

- **Caso derivado:** [SD-CT-16](../casos-de-teste/SD-CT-16.md)
- **Execução complementar:** [SD-EX-16](SD-EX-16.md)
- **Defeito identificado:** [BUG-003](../bugs/BUG-003.md)

## Evidências e limitações

- Não há captura individual atribuída a esta execução no registro original.
- A data original da execução não foi documentada.
- A apresentação visual da mensagem foi avaliada separadamente no SD-EX-16.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
