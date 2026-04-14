# Relatorio de Execucao Smoke - Rodada 01

## Resumo

- Data da execucao: 2026-04-14
- Ambiente: Practice Software Testing - ambiente publico
- Navegador: Chrome via Playwright CLI
- Executor: Wesley

## Escopo executado

- checklist smoke: executado
- casos de teste: nao aplicavel nesta rodada
- exploratorio: pontual, durante carrinho e cadastro

## Resultado consolidado

| Categoria | Quantidade |
| --- | --- |
| Casos planejados | 10 |
| Casos executados | 10 |
| Aprovados | 7 |
| Reprovados | 1 |
| Bloqueados | 2 |
| Nao executados | 0 |

## Resultado por item do smoke

| ID | Status | Evidencia resumida |
| --- | --- | --- |
| SMK-01 | Pass | Home carregou com titulo e listagem inicial visiveis |
| SMK-02 | Pass | Catalogo exibiu produtos navegaveis |
| SMK-03 | Pass | Busca por `hammer` retornou itens coerentes com o termo |
| SMK-04 | Pass | Filtro de produtos eco-friendly reduziu os resultados corretamente |
| SMK-05 | Pass | Detalhe do produto `Hammer` exibiu nome, preco e CTA `Add to cart` |
| SMK-06 | Pass | Item foi adicionado ao carrinho e contador do carrinho foi atualizado |
| SMK-07 | Fail | Alteracao de quantidade gerou divergencia entre total da linha e total geral |
| SMK-08 | Blocked | Nao havia credencial valida pre-provisionada; tentativa de criar conta foi bloqueada por defeito no cadastro |
| SMK-09 | Blocked | Dependente de autenticacao bem-sucedida, nao executado por bloqueio anterior |
| SMK-10 | Pass | Fluxo avancou para a etapa de `Sign in` no checkout mantendo o item no carrinho |

## Bugs encontrados

| Bug ID | Titulo | Severidade | Status |
| --- | --- | --- | --- |
| BUG-001 | Total geral do carrinho nao acompanha mudanca de quantidade | Alta | Aberto |
| BUG-002 | Formulario de cadastro exige pais mesmo com `Brazil` selecionado | Alta | Aberto |

## Principais observacoes

- o fluxo principal de navegacao e descoberta de produto esta operacional
- o modulo de checkout apresentou comportamento inconsistente em valor total, afetando confianca e corretude do fluxo
- o fluxo de cadastro impediu a criacao de conta de teste, impactando a validacao de login/logout nesta rodada
- o console registrou erros relacionados a `cart_items` durante o checkout, o que merece correlacao tecnica com o BUG-001

## Riscos residuais

- risco alto no fluxo de compra por calculo inconsistente
- risco alto no onboarding autenticado por bloqueio no cadastro
- risco medio em autenticacao por ausencia de validacao completa de login/logout nesta rodada

## Recomendacao preliminar

- No Go

## Proximas acoes recomendadas

1. Corrigir e retestar BUG-001 com foco em recalculo de carrinho.
2. Corrigir e retestar BUG-002 com foco em validacao do formulario.
3. Reexecutar SMK-08 e SMK-09 apos disponibilizar credencial valida ou concluir cadastro com sucesso.
