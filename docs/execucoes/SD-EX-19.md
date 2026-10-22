# SD-EX-19 | Registro exploratório: informações dos produtos

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-19

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Vitrine / Catálogo
- **Caso relacionado:** [SD-CT-19](../casos-de-teste/SD-CT-19.md)
- **Natureza:** Registro retrospectivo de exploração manual anterior à formalização do caso.
- **Data da exploração:** 22/10/2026

**Objetivo:** documentar as observações sobre a exibição das informações dos produtos e sua consistência entre listagem e detalhes.

## Ambiente conhecido

- **Aplicação:** https://www.saucedemo.com/
- **Navegador, versão, sistema operacional e dimensões da janela:** não informados para esta exploração.

## Cobertura observada

Foram identificados seis produtos na vitrine e acessados individualmente os detalhes dos seis.

A verificação contemplou nome, descrição, imagem e preço, considerando sua exibição e a consistência entre listagem e detalhes.

## Resultados

- Os seis produtos apresentaram nome, descrição, imagem e preço visível na vitrine.
- Nome, descrição, imagem e preço permaneceram consistentes entre a listagem e os detalhes dos seis produtos.
- Foram observados textos com aparência de código na descrição de uma mochila e no título de uma camiseta vermelha. Essas observações não foram classificadas como defeitos, pois não há confirmação de que os textos estejam incorretos.

**Conclusão do registro:** não foram relatadas ausências dos quatro atributos na vitrine nem divergências entre as telas. Este resultado descreve a exploração realizada e não constitui aprovação de uma execução formal do SD-CT-19.

## Limitações

A exploração ocorreu antes da formalização do SD-CT-19. A associação ao caso é retrospectiva e não comprova que seu procedimento e todos os seus critérios tenham sido executados formalmente.

As informações fornecidas não incluem identificação individual dos seis produtos, valores completos dos atributos ou resultados detalhados de legibilidade por produto. Este registro mantém os resultados consolidados disponíveis, sem reconstruir dados não registrados.

Não há especificação oficial ou referência independente confiável para confirmar a correção absoluta das informações. A consistência entre telas não garante correção: ambas podem apresentar o mesmo dado incorreto.

Os textos com aparência de código permanecem como observações a investigar.

## Rastreabilidade

- **Caso relacionado:** [SD-CT-19](../casos-de-teste/SD-CT-19.md) — caso formalizado relacionado às verificações exploratórias aqui documentadas.
- **VIT-01:** observação da presença de nome e preço na vitrine.
- **VIT-03:** observação da consistência de nome e preço entre listagem e detalhes.
- **VIT-05:** observação da presença de imagens e descrições; sem registro detalhado de legibilidade por produto.

Os identificadores `VIT` representam itens de planejamento. Sua associação a este registro indica correspondência com a exploração relatada, sem declarar cobertura formal integral.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
