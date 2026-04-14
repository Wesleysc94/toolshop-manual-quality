# Recomendacao de Release - 2026-04-14

## Decisao

- Status recomendado: No Go
- Data: 2026-04-14
- Responsavel: Wesley

## Base para decisao

- cobertura executada: smoke inicial do fluxo web principal
- bugs abertos: 2 bugs de alta severidade
- riscos residuais: elevados em checkout e cadastro de usuario

## Resumo executivo

Nao e recomendado liberar uma versao com foco em compra completa neste estado. A aplicacao navega bem, permite buscar produtos e teve login/logout validados em reteste posterior, mas o carrinho apresenta erro no valor total apos mudanca de quantidade e o cadastro de novo usuario ficou bloqueado por validacao incorreta de pais.

## Criticidades observadas

- BUG-001 compromete a confiabilidade do valor total no checkout
- BUG-002 bloqueia a criacao de novas contas no fluxo autenticado

## Validacoes complementares

- login validado com conta demo oficial do produto
- logout validado com encerramento de sessao e retorno para a tela de login

## Condicoes para seguir

- corrigir BUG-001 e validar recalculo correto do total
- corrigir BUG-002 e validar cadastro bem-sucedido
- reexecutar smoke dos itens bloqueados e do fluxo de checkout

## Condicoes para bloquear

- qualquer divergencia de valor total no checkout
- impossibilidade de criar conta ou autenticar novo usuario
