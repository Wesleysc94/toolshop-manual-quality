# Escopo do Produto

## Visao geral

O produto sob teste e um e-commerce web voltado para pratica de qualidade. Para este repositorio, o interesse principal esta nos fluxos que mais representam risco funcional e valor de negocio.

## Objetivo do escopo

Definir de forma clara o recorte desta etapa, mantendo foco nos fluxos mais importantes do produto.

## Modulos em escopo

### 1. Autenticacao

- login com credenciais validas
- login com credenciais invalidas
- validacao de campos obrigatorios
- logout
- comportamento basico de sessao

### 2. Catalogo

- abertura da home e listagem de produtos
- navegacao para detalhes de produto
- consistencia basica de nome, preco e disponibilidade visual

### 3. Busca e filtros

- busca por palavra-chave
- combinacao de filtros aplicaveis
- retorno sem resultado
- reset ou alteracao de filtros

### 4. Carrinho

- adicao de item
- alteracao de quantidade
- remocao de item
- persistencia basica do estado enquanto a sessao estiver ativa
- consistencia de subtotal

### 5. Checkout

- acesso ao fluxo de checkout
- validacao de campos obrigatorios
- continuidade das etapas principais
- consistencia das informacoes carregadas do carrinho

### 6. Perfil e contato

- acesso a dados de conta quando autenticado
- validacoes basicas de formulario de contato

## Fora de escopo nesta fase

- automacao
- API testing
- compatibilidade mobile
- testes de performance
- acessibilidade profunda
- testes de seguranca
- painel administrativo

## Personas consideradas

### Visitante

Usuario que navega, busca produtos e tenta iniciar compra sem estar autenticado.

### Cliente autenticado

Usuario com conta valida que interage com carrinho, checkout e dados de conta.

## Dependencias

- ambiente publico do produto disponivel
- massa de dados funcional para login
- produtos ativos e visiveis no catalogo
- comportamento estavel do ambiente durante as execucoes

## Criterio de priorizacao

O foco inicial segue esta ordem:

1. fluxos que bloqueiam compra ou acesso
2. fluxos que afetam descoberta de produtos
3. fluxos de consistencia de dados e validacoes
4. fluxos secundarios de suporte e perfil

## Resultado esperado desta definicao

Com este recorte, a etapa fica concentrada nos fluxos que mais impactam navegacao, compra e acesso do usuario.
