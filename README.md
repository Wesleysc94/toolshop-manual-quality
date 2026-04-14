# toolshop-manual-quality

Projeto de QA manual construido sobre a aplicacao publica **Practice Software Testing**.

Este repositorio registra a etapa manual do portfolio: definicao de escopo, organizacao da rodada, execucao do smoke, abertura de bugs e recomendacao final.

## Visao Geral

Aqui, a proposta foi documentar de forma simples e confiavel:

- o que entrou na primeira rodada
- como a execucao foi conduzida
- quais falhas foram encontradas
- qual foi a conclusao da etapa

## Produto Sob Teste

- Aplicacao web: https://practicesoftwaretesting.com/
- Referencia de API: https://practiceautomatedtesting.com/api
- Swagger: https://practiceautomatedtesting.com/swagger

## Escopo Da Etapa

Os fluxos priorizados nesta primeira fase foram:

- autenticacao
- catalogo
- busca e filtros
- carrinho
- checkout
- contato e perfil

Ficaram fora desta etapa:

- automacao web
- automacao de API
- testes mobile
- performance
- area administrativa

## Resultado Da Rodada

Em `2026-04-14`, o projeto registrou:

- uma rodada inicial de smoke
- um reteste de autenticacao com conta demo oficial
- `2` defeitos relevantes documentados
- confirmacao de login e logout no reteste
- recomendacao final `No Go`

## Estrutura Do Repositorio

- [RESUMO-DO-PROJETO.txt](./RESUMO-DO-PROJETO.txt): leitura curta da etapa
- [docs/](./docs/): escopo, plano de testes, analise de risco e guia de revisao
- [checklists/](./checklists/): checklist smoke da rodada
- [test-cases/](./test-cases/): casos de teste por area funcional
- [bug-reports/](./bug-reports/): falhas encontradas com impacto e reproducao
- [execution-reports/](./execution-reports/): relatorios das execucoes realizadas
- [release/](./release/): recomendacao final da rodada
- [evidence/](./evidence/): screenshots e registros de apoio

## Como Revisar

1. Comece por [RESUMO-DO-PROJETO.txt](./RESUMO-DO-PROJETO.txt).
2. Leia [docs/guia-de-revisao.md](./docs/guia-de-revisao.md).
3. Consulte os relatorios em [execution-reports/](./execution-reports/).
4. Veja os registros em [bug-reports/](./bug-reports/).
5. Feche a leitura com [release/2026-04-14-recomendacao-de-release.md](./release/2026-04-14-recomendacao-de-release.md).

## Como Validar

Como esta etapa e manual, a validacao e feita por leitura e reproducao:

1. Acesse o produto publico.
2. Siga os relatorios e os casos de teste.
3. Compare os resultados com os bugs e as evidencias registradas.
