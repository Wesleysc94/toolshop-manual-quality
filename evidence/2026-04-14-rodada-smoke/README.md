# Evidencias - 2026-04-14 Rodada Smoke

## Contexto

Rodada inicial de smoke executada no ambiente publico do Practice Software Testing usando Chrome via Playwright CLI.

## Artefatos principais

- home carregada: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T16-55-38-081Z.png`
- inconsistencia no carrinho: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T16-59-34-451Z.png`
- bloqueio no cadastro: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T17-03-26-892Z.png`
- log de console: `toolshop-manual-quality/output/playwright/.playwright-cli/console-2026-04-14T16-54-59-982Z.log`

## Leitura rapida da rodada

- home, catalogo, busca, filtro, detalhe de produto e adicao ao carrinho funcionaram
- ao alterar a quantidade do item no checkout, o total da linha foi atualizado, mas o total geral nao
- ao tentar criar uma conta de teste, o formulario manteve a mensagem `Country is required` mesmo com `Brazil` selecionado

## Observacoes tecnicas

- houve erros de console relacionados a `cart_items` durante o checkout
- tambem houve respostas `401 Unauthorized` para `/users/me` quando a sessao nao estava autenticada; isso parece coerente com usuario anonimo e nao foi tratado como bug por si so
