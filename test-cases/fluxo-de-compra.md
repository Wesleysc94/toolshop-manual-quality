# Shopping Flow Test Cases

## Cobertura

Fluxos principais de descoberta de produto, carrinho e checkout.

| ID | Titulo | Prioridade | Pre-condicoes | Passos principais | Resultado esperado |
| --- | --- | --- | --- | --- | --- |
| TC-SHOP-001 | Busca por termo valido retorna produtos relevantes | Alta | Aplicacao acessivel | Informar termo de busca valido no catalogo | Lista exibe resultados coerentes com o termo pesquisado |
| TC-SHOP-002 | Aplicacao de filtro refina os resultados | Alta | Catalogo carregado | Aplicar um filtro disponivel | Lista e reduzida ou reorganizada sem erro funcional |
| TC-SHOP-003 | Busca sem resultado nao quebra a experiencia | Media | Aplicacao acessivel | Informar termo sem correspondencia conhecida | Sistema mostra estado sem resultado de forma clara |
| TC-SHOP-004 | Abertura do detalhe de produto a partir da listagem | Media | Produto visivel no catalogo | Abrir um item da listagem | Detalhe corresponde ao item selecionado |
| TC-SHOP-005 | Adicao de produto ao carrinho | Alta | Produto disponivel | Abrir um produto e adicionar ao carrinho | Item aparece no carrinho com descricao e quantidade consistentes |
| TC-SHOP-006 | Atualizacao de quantidade no carrinho | Alta | Carrinho com item | Alterar quantidade do item | Subtotal e quantidade refletem a alteracao |
| TC-SHOP-007 | Remocao de item do carrinho | Alta | Carrinho com item | Remover item | Item deixa de aparecer e valores sao atualizados |
| TC-SHOP-008 | Inicio do checkout com carrinho valido | Alta | Carrinho com pelo menos um item | Avancar para checkout | Fluxo de checkout inicia sem perder os itens selecionados |
| TC-SHOP-009 | Validacao de campos obrigatorios no checkout | Alta | Checkout iniciado | Deixar campos obrigatorios vazios e tentar avancar | Sistema impede continuidade e destaca os campos necessarios |
| TC-SHOP-010 | Continuidade do checkout com dados validos | Alta | Dados validos disponiveis | Preencher informacoes obrigatorias e avancar | Sistema aceita os dados e segue para a proxima etapa prevista |

## Observacoes

- conferir se mensagens de erro sao compreensiveis
- observar se totalizadores e estado do carrinho permanecem consistentes entre paginas
