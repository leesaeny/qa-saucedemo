# Execuções de teste | Responsividade

**Aplicação:** SauceDemo
**Data:** 17/10/2026
**Tipo:** Teste manual de interface e compatibilidade entre navegadores

## SD-EX-16 | Mensagem de erro no login

**Caso relacionado:** SD-CT-16

**Resultado:** Reprovado

### Resultado esperado

A mensagem de erro deve permanecer integralmente legível, sem cortes ou sobreposição de elementos, nas larguras de janela suportadas.

### Resultado observado

Em janelas desktop mais largas, parte da mensagem de erro fica oculta. Ao reduzir a largura da janela, o texto passa a ser exibido corretamente.

O comportamento foi reproduzido nos seguintes navegadores:

- Google Chrome
- Microsoft Edge
- Safari
- Vivaldi

### Evidências

Foram realizadas capturas comparativas em diferentes larguras de janela.

As três capturas estão disponíveis na seção Evidências visuais, com imagens armazenadas em `evidencias/login/`.

### Cobertura por navegador

| Navegador | Executado | Evidência visual |
|---|---|---|
| Chrome | Sim | 3 capturas |
| Edge | Sim | Não registrada |
| Safari | Sim | Não registrada |
| Vivaldi | Sim | Não registrada |

**Observação:** As três capturas foram realizadas exclusivamente no Google Chrome, em diferentes larguras de janela. O comportamento também foi reproduzido manualmente nos demais navegadores.

### Limitações

- As larguras exatas da viewport CSS não foram medidas.
- As versões de todos os navegadores não foram registradas.
- A causa técnica do problema não foi identificada.

### Defeito relacionado

BUG-003 | Mensagem de erro parcialmente oculta em determinadas larguras de janela.

O teste funcional de rejeição das credenciais inválidas (SD-CT-09) permanece aprovado.

## Evidências visuais

### Janela larga: mensagem parcialmente oculta

![Mensagem de erro parcialmente oculta em janela larga](../../evidencias/login/erro-janela-larga.png)

### Janela intermediária: mensagem legível

![Mensagem de erro legível em janela intermediária](../../evidencias/login/erro-janela-intermediaria.png)

### Janela estreita: mensagem legível

![Mensagem de erro legível em janela estreita](../../evidencias/login/erro-janela-estreita.png)
