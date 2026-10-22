# QA SauceDemo

Portfólio de Quality Assurance com testes manuais e investigação de comportamentos da aplicação SauceDemo.

## Aplicação testada
https://www.saucedemo.com/

## Objetivos
- Planejar e executar testes funcionais.
- Documentar casos de teste e resultados.
- Investigar possíveis defeitos.
- Organizar evidências e relatórios.
- Evoluir para automação com Cypress.

## Ferramentas
- Git e GitHub
- Jira
- JavaScript e Cypress (etapa futura)

## Situação
Projeto de QA em desenvolvimento, com foco em testes manuais, investigação de defeitos e documentação rastreável. A cobertura exploratória da vitrine contempla informações dos produtos, inclusão e remoção pela listagem e ordenação por preço e nome.

- **8 casos de teste** documentados.
- **5 execuções formais** registradas: 4 aprovadas, sendo 1 apenas no recorte funcional, e 1 reprovada.
- **3 registros exploratórios** da vitrine, sem divergências relatadas, que não representam aprovação de execuções formais.
- **1 defeito** documentado, com evidências visuais.
- Rastreabilidade entre casos, execuções e defeitos.

Próximas etapas: ampliar a cobertura de testes e explorar automação.

## Estrutura do projeto

```text
.
├── README.md
├── docs/
│   ├── estrategia-de-testes.md
│   ├── casos-de-teste/
│   │   └── SD-CT-*.md
│   ├── execucoes/
│   │   └── SD-EX-*.md
│   └── bugs/
│       └── BUG-*.md
└── evidencias/
```

## Documentação

| Seção | Conteúdo |
|---|---|
| [Estratégia de testes](docs/estrategia-de-testes.md) | Abordagens utilizadas e evolução da investigação |
| [Casos de teste](docs/casos-de-teste/README.md) | Cenários e resultados esperados |
| [Execuções](docs/execucoes/README.md) | Resultados observados e evidências |
| [Defeitos](docs/bugs/README.md) | Problemas identificados e investigados |

## Organização do projeto

Os documentos são organizados por funcionalidade, seguindo o fluxo de utilização da aplicação: login, catálogo, carrinho e checkout.

Os identificadores originais dos testes foram preservados para manter a rastreabilidade entre casos, execuções e defeitos.
