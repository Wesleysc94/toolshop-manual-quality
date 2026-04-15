# Guia de Revisao

## Objetivo

Este repositorio apresenta uma rodada de QA manual realizada sobre a aplicacao publica **Practice Software Testing**.

O foco aqui e registrar:

- o que foi testado
- o que foi encontrado
- quais evidencias foram registradas
- qual foi a conclusao da rodada

## Ordem de leitura recomendada

1. Ler `RESUMO-DO-PROJETO.txt`.
2. Ler o `README.md` para entender o projeto de forma geral.
3. Ler `execution-reports/2026-04-14-rodada-smoke-01.md`.
4. Ler `execution-reports/2026-04-14-reteste-autenticacao.md`.
5. Abrir os registros em `bug-reports/`.
6. Conferir as evidencias em `evidence/`.
7. Ler `release/2026-04-14-recomendacao-de-release.md`.

## Produto sob teste

- aplicacao web: https://practicesoftwaretesting.com/
- API: https://api.practicesoftwaretesting.com/
- Swagger: https://api.practicesoftwaretesting.com/swagger
- repositorio oficial: https://github.com/testsmith-io/practice-software-testing

## Como validar os resultados

### Execucao smoke

O relatorio inicial concentra os fluxos cobertos na primeira rodada. Quem quiser validar o projeto pode acessar a aplicacao publica e repetir os seguintes fluxos:

- home
- catalogo
- busca
- filtro
- detalhe do produto
- carrinho
- checkout

### Login e logout

O projeto oficial publica credenciais demo em seu README. No reteste de autenticacao foi utilizada a seguinte conta:

- email: `customer@practicesoftwaretesting.com`
- senha: `welcome01`

Fonte oficial:

- https://github.com/testsmith-io/practice-software-testing

### Defeitos

Cada bug report traz:

- pre-condicoes
- passos para reproduzir
- resultado atual
- resultado esperado
- impacto
- evidencias

## Escopo validado

- navegacao principal do produto
- descoberta de produto por busca e filtro
- adicao ao carrinho
- entrada no checkout
- login com conta demo oficial
- logout com encerramento de sessao

## Pontos abertos

- inconsistencia no total do carrinho apos alteracao de quantidade
- bloqueio no cadastro de novo usuario por validacao incorreta de pais

## Posicionamento do repositorio

Este repositorio nao foi criado como framework de automacao. A proposta desta etapa e apresentar uma base de QA manual bem documentada, com execucao real, evidencias e conclusao clara.

## Navegacao do portfolio

- portfolio principal: https://github.com/Wesleysc94/Wesleysc94
- hub do Case Study 1: https://github.com/Wesleysc94/toolshop-quality-portfolio
- Case Study 2: https://github.com/Wesleysc94/swaglab-quality-suite
