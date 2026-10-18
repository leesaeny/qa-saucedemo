# SD-EX-16 | Legibilidade da mensagem de erro no login

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-16

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Login
- **Tipo:** Teste manual de interface e compatibilidade entre navegadores
- **Caso relacionado:** [SD-CT-16](../casos-de-teste/SD-CT-16.md)
- **Data:** 17/10/2026
- **Resultado:** Reprovado

## Resultado esperado

A mensagem de erro deve permanecer integralmente legível, sem cortes ou sobreposição de elementos, nas larguras de janela suportadas.

## Resultado observado

Em janelas desktop mais largas, parte da mensagem de erro fica oculta.

Ao reduzir a largura da janela, o texto passa a ser exibido integralmente.

O comportamento foi reproduzido nos navegadores Chrome, Edge, Safari e Vivaldi.

## Cobertura por navegador

| Navegador | Executado | Evidência visual |
|---|---|---|
| Google Chrome | Sim | 3 capturas |
| Microsoft Edge | Sim | Não registrada |
| Safari | Sim | Não registrada |
| Vivaldi | Sim | Não registrada |

As capturas foram realizadas exclusivamente no Google Chrome. Nos demais navegadores, o comportamento foi reproduzido por observação manual.

## Evidências visuais

### Janela larga: mensagem parcialmente oculta

![Mensagem de erro parcialmente oculta em janela larga](../../evidencias/login/erro-janela-larga.png)

### Janela intermediária: mensagem legível

![Mensagem de erro legível em janela intermediária](../../evidencias/login/erro-janela-intermediaria.png)

### Janela estreita: mensagem legível

![Mensagem de erro legível em janela estreita](../../evidencias/login/erro-janela-estreita.png)

## Limitações

- As larguras exatas da viewport CSS não foram medidas.
- As versões dos navegadores não foram registradas.
- A faixa oficial de larguras suportadas não foi confirmada.
- A causa técnica do problema não foi identificada.

## Rastreabilidade

- **Caso relacionado:** [SD-CT-16](../casos-de-teste/SD-CT-16.md)
- **Caso de origem da investigação:** [SD-CT-09](../casos-de-teste/SD-CT-09.md)
- **Execução funcional relacionada:** [SD-EX-09](SD-EX-09.md)
- **Defeito identificado:** [BUG-003](../bugs/BUG-003.md)

O teste funcional de rejeição das credenciais inválidas permanece aprovado no SD-EX-09. Esta execução avalia especificamente a legibilidade da mensagem.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
