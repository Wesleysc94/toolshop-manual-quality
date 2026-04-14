# Evidencias - 2026-04-14 Reteste de Autenticacao

## Contexto

Rodada curta de reteste executada para fechar os itens bloqueados de autenticacao do smoke inicial.

## Base usada

Conta demo oficial publicada no repositorio do produto:

- email: `customer@practicesoftwaretesting.com`
- senha: `welcome01`

Fonte:

- https://github.com/testsmith-io/practice-software-testing

## Artefatos principais

- login bem-sucedido: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T17-35-18-085Z.png`
- logout e retorno para tela de login: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T17-36-53-329Z.png`
- log tecnico da sessao: `toolshop-manual-quality/output/playwright/.playwright-cli/console-2026-04-14T17-34-20-854Z.log`

## Resultado

- login validado com sucesso
- menu autenticado exibido com o nome `Jane Doe`
- logout validado com retorno para `/auth/login`
