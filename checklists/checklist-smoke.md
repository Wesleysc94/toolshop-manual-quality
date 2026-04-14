# Smoke Checklist

## Objetivo

Validar rapidamente se o ambiente esta utilizavel para uma rodada funcional mais profunda.

## Pre-condicoes

- navegador desktop disponivel
- aplicacao acessivel
- usuario de teste disponivel caso o fluxo exija autenticacao

## Checklist

| ID | Fluxo | Verificacao | Resultado esperado |
| --- | --- | --- | --- |
| SMK-01 | Home | Abrir a aplicacao | Pagina inicial carrega sem erro visivel bloqueante |
| SMK-02 | Catalogo | Navegar para a listagem de produtos | Produtos ficam visiveis e navegaveis |
| SMK-03 | Busca | Buscar um termo valido | Lista retorna itens compativeis com a busca |
| SMK-04 | Filtro | Aplicar pelo menos um filtro funcional | Resultado e atualizado sem quebrar a pagina |
| SMK-05 | Detalhe | Abrir um produto | Nome, preco e CTA principal aparecem |
| SMK-06 | Carrinho | Adicionar um item ao carrinho | Item aparece no carrinho com quantidade inicial valida |
| SMK-07 | Carrinho | Alterar quantidade ou remover item | Carrinho atualiza corretamente |
| SMK-08 | Login | Entrar com usuario valido | Usuario e autenticado e a sessao segue ativa |
| SMK-09 | Logout | Sair da conta | Sessao encerra sem erro aparente |
| SMK-10 | Checkout | Iniciar o fluxo de checkout | Etapa inicial abre e mantem os dados do carrinho |

## Regras de decisao

- se qualquer item de autenticacao, carrinho ou checkout falhar, a rodada funcional deve ser reavaliada
- se a falha for cosmetica e nao bloquear fluxo, a execucao pode continuar com observacao registrada

## Evidencia minima esperada

- data e hora da execucao
- navegador utilizado
- status por item
- screenshot quando houver falha
