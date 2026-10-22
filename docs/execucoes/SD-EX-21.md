# SD-EX-21 | Registro exploratório: ordenação dos produtos na vitrine

[Início](../../README.md) > [Execuções de teste](README.md) > SD-EX-21

## Identificação

- **Aplicação:** SauceDemo
- **Funcionalidade:** Vitrine / Catálogo
- **Caso relacionado:** [SD-CT-21](../casos-de-teste/SD-CT-21.md)
- **Natureza:** Registro retrospectivo de exploração manual anterior à formalização do caso.
- **Data da exploração:** 22/10/2026

**Objetivo:** documentar a verificação da sequência completa dos produtos nas quatro opções de ordenação da vitrine.

## Ambiente conhecido

- **Aplicação:** https://www.saucedemo.com/
- **Navegador, versão, sistema operacional e dimensões da janela:** não informados para esta exploração.

## Cobertura observada

Foram observados seis produtos. Em cada conjunto, foi conferida a sequência completa dos seis, sem limitar a verificação ao primeiro e ao último.

## Resultados por conjunto de dados

| ID | Opção de ordenação | Resultado observado |
|---|---|---|
| D01 | Price (low to high) | Sequência completa conferida por preço crescente, sem divergências relatadas. |
| D02 | Price (high to low) | Sequência completa conferida por preço decrescente, sem divergências relatadas. |
| D03 | Name (A to Z) | Sequência completa conferida por nome A–Z, sem divergências relatadas. |
| D04 | Name (Z to A) | Sequência completa conferida por nome Z–A, sem divergências relatadas. |

**Conclusão do registro:** não foram relatadas divergências de ordenação nos quatro conjuntos. Esse resultado não constitui aprovação de uma execução formal do SD-CT-21.

## Limitações

A associação ao SD-CT-21 é retrospectiva e não comprova a execução formal de todos os seus passos e critérios, incluindo a conferência específica de preservação dos produtos sem omissões ou duplicações.

Os nomes, preços e sequências individuais não foram fornecidos para este registro.

A ordenação observada considera os dados exibidos e não confirma a correção absoluta dos nomes ou preços, para a qual não há especificação oficial disponível.

## Rastreabilidade

- **Caso relacionado:** [SD-CT-21](../casos-de-teste/SD-CT-21.md) — caso formalizado relacionado à exploração aqui documentada.
- **VIT-06 — Ordenação por preço crescente e decrescente:** conjuntos D01 e D02.
- **VIT-07 — Ordenação por nome A–Z e Z–A:** conjuntos D03 e D04.

Os identificadores `VIT` pertencem ao planejamento. Sua associação a este registro indica correspondência com a exploração relatada, sem declarar execução formal do caso.

## Navegação

[← Voltar ao índice de execuções](README.md)

[⌂ Voltar ao README principal](../../README.md)
