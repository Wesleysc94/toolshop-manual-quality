# BUG-002 - Cadastro bloqueado por validacao incorreta de pais

## Identificacao

- Bug ID: BUG-002
- Titulo: Formulario de cadastro exige pais mesmo com `Brazil` selecionado
- Data: 2026-04-14
- Reportado por: Wesley

## Contexto

- Ambiente: Practice Software Testing - ambiente publico
- Navegador: Chrome via Playwright CLI
- Build ou referencia: Toolshop v5.0
- Severidade: Alta
- Prioridade: Alta

## Pre-condicoes

- usuario anonimo no fluxo de checkout
- acesso ao formulario `Register your account`

## Passos para reproduzir

1. Adicionar um item ao carrinho.
2. Abrir o checkout e avancar para a etapa de autenticacao.
3. Clicar em `Register your account`.
4. Preencher os campos obrigatorios do formulario.
5. Selecionar `Brazil` no campo `Country`.
6. Submeter o formulario.

## Resultado atual

O formulario permanece na tela e exibe a mensagem `Country is required`, mesmo com `Brazil` visivelmente selecionado no campo de pais.

## Resultado esperado

O campo `Country` deve ser aceito como preenchido quando um pais valido estiver selecionado, permitindo o prosseguimento do cadastro.

## Evidencias

- screenshot: `toolshop-manual-quality/output/playwright/.playwright-cli/page-2026-04-14T17-03-26-892Z.png`
- observacoes adicionais: o bloqueio persistiu apos novo submit com os demais campos obrigatorios preenchidos

## Impacto

Bloqueia a criacao de nova conta e prejudica a entrada de novos clientes no fluxo autenticado. Mesmo existindo opcao de checkout sem login, o defeito impacta onboarding e reduz a confianca no modulo de autenticacao.
