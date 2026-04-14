# BUG-001 - Total geral do carrinho nao acompanha mudanca de quantidade

## Identificacao

- Bug ID: BUG-001
- Titulo: Total geral permanece desatualizado apos alterar quantidade no checkout
- Data: 2026-04-14
- Reportado por: Wesley

## Contexto

- Ambiente: Practice Software Testing - ambiente publico
- Navegador: Chrome via Playwright CLI
- Build ou referencia: Toolshop v5.0
- Severidade: Alta
- Prioridade: Alta

## Pre-condicoes

- item em estoque adicionado ao carrinho
- checkout acessivel na etapa de carrinho

## Passos para reproduzir

1. Abrir a aplicacao.
2. Acessar um produto em estoque, como `Hammer`.
3. Adicionar o item ao carrinho.
4. Abrir o checkout.
5. Alterar a quantidade do item de `1` para `2`.

## Resultado atual

O total da linha do item e recalculado para `25.16`, mas o total geral do carrinho permanece em `12.58`.

## Resultado esperado

O total geral do carrinho deve refletir a mesma quantidade atualizada do item, passando para `25.16`.

## Evidencias

- screenshot: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T16-59-34-451Z.png`
- log tecnico: `toolshop-manual-quality/output/playwright/.playwright-cli/console-2026-04-14T16-54-59-982Z.log`
- observacoes adicionais: o problema persistiu apos aguardar nova renderizacao da tela

## Impacto

Afeta diretamente um fluxo critico de compra. O usuario pode visualizar valores inconsistentes antes de prosseguir, gerando perda de confianca, risco de cobranca incorreta percebida e bloqueio de release orientada a checkout.
