# SD-CT-16 | Legibilidade da mensagem de erro no login

[Início](../../README.md) > [Casos de teste](README.md) > SD-CT-16

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste manual de interface e responsividade

## Origem

Caso criado a partir de um comportamento visual identificado durante a investigação do SD-CT-09.

**Caso de origem:** [SD-CT-09 | Usuário incorreto](SD-CT-09.md)

## Pré-condição

Estar na tela de login do SauceDemo.

## Dados de teste

| Campo | Valor |
|---|---|
| Usuário | `standard_use` |
| Senha | `secret_sauce` |
| Navegadores | Chrome, Edge, Safari e Vivaldi |

O usuário é intencionalmente inválido para provocar a apresentação da mensagem de erro.

## Passos

1. Abrir a aplicação em uma janela larga.
2. Preencher as credenciais inválidas.
3. Clicar em Login.
4. Verificar a legibilidade da mensagem de erro.
5. Reduzir gradualmente a largura da janela.
6. Comparar a apresentação da mensagem.
7. Repetir o procedimento nos quatro navegadores.

## Resultado esperado

A mensagem deve permanecer integralmente legível, sem cortes ou sobreposição de elementos, nas larguras de janela suportadas.

## Limitações

- A largura exata da viewport CSS não foi medida.
- O teste investiga o comportamento visual, não sua causa técnica.
- A faixa oficial de larguras suportadas não foi confirmada.

## Rastreabilidade

- **Caso de origem:** [SD-CT-09](SD-CT-09.md)
- **Execução relacionada:** SD-EX-16
- **Defeito relacionado:** [BUG-003](../bugs/BUG-003.md)

O resultado observado e as evidências estão documentados nos registros de execução e de defeito.

## Navegação

[← Voltar ao índice de casos de teste](README.md)

[⌂ Voltar ao README principal](../../README.md)
