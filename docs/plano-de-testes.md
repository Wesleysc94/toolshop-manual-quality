# Plano de Testes

## 1. Objetivo

Organizar a primeira rodada de QA manual para o produto Practice Software Testing, priorizando os fluxos mais importantes de navegacao, autenticacao e compra.

## 2. Itens de teste

- pagina inicial
- catalogo de produtos
- busca e filtros
- detalhe do produto
- carrinho
- checkout
- login e logout
- contato e perfil

## 3. Tipos de teste previstos

- smoke
- funcional positivo
- funcional negativo
- validacao de campos obrigatorios
- consistencia basica de estado
- exploratorio orientado a risco

## 4. Abordagem

### Smoke

Usado para verificar rapidamente se o ambiente esta pronto para uma rodada mais ampla.

### Testes funcionais

Usados para validar os fluxos principais e os comportamentos esperados em cada area.

### Exploratorio guiado por risco

Usado para ampliar a cobertura nos pontos de maior impacto, principalmente em navegacao, validacoes e persistencia do carrinho.

## 5. Ambiente

- tipo: ambiente publico de demonstracao
- interface principal: web browser desktop
- evidencias esperadas: screenshots, anotacoes de execucao e links quando aplicavel

## 6. Dados de teste

- usuario valido para autenticacao
- usuario invalido ou senha incorreta
- produtos disponiveis no catalogo
- dados de checkout para validacao positiva e negativa

## 7. Criterios de entrada

- ambiente acessivel
- massa de dados minima disponivel
- escopo e checklist revisados
- casos prioritarios definidos

## 8. Criterios de saida

- smoke executado
- casos prioritarios executados ou justificados
- defeitos relevantes registrados
- execution report consolidado
- recomendacao de release emitida

## 9. Entregaveis

- product scope
- risk analysis
- smoke checklist
- test cases
- execution report
- bug reports
- release recommendation

## 10. Priorizacao

Prioridade alta:

- login
- busca e filtros
- carrinho
- checkout

Prioridade media:

- catalogo
- detalhe do produto
- perfil e contato

## 11. Riscos operacionais

- indisponibilidade intermitente do ambiente
- mudanca de dados do catalogo entre execucoes
- dependencia de usuario valido

## 12. Metricas simples que serao acompanhadas

- total de casos planejados
- total executado
- taxa de aprovacao
- quantidade de bugs por severidade
- cobertura dos fluxos criticos
