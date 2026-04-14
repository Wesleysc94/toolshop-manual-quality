# Analise de Risco

## Criterio

Classificacao simples baseada em:

- impacto no usuario ou negocio
- probabilidade de falha
- prioridade de teste

Escala usada:

- Alto
- Medio
- Baixo

## Matriz inicial de risco

| ID | Area | Risco | Impacto | Probabilidade | Prioridade de teste |
| --- | --- | --- | --- | --- | --- |
| R-01 | Autenticacao | Usuario nao consegue entrar com credenciais validas | Alto | Medio | Alta |
| R-02 | Busca e filtros | Usuario nao encontra produtos relevantes ou recebe resultado inconsistente | Alto | Medio | Alta |
| R-03 | Carrinho | Itens nao sao adicionados, removidos ou recalculados corretamente | Alto | Medio | Alta |
| R-04 | Checkout | Usuario nao consegue concluir etapas principais da compra | Alto | Medio | Alta |
| R-05 | Validacoes | Campos obrigatorios permitem dados invalidos ou bloqueiam dados corretos | Medio | Alto | Alta |
| R-06 | Sessao | Estado do usuario fica inconsistente apos login, logout ou navegacao | Medio | Medio | Media |
| R-07 | Catalogo | Informacoes de produto aparecem incorretas ou navegam para detalhe errado | Medio | Medio | Media |
| R-08 | Perfil e contato | Fluxos secundarios falham sem bloquear compra, mas afetam confianca do produto | Medio | Baixo | Media |

## Leitura pratica da matriz

### Testar primeiro

- login
- busca e filtros
- carrinho
- checkout

### Testar em seguida

- detalhe de produto
- consistencia de sessao
- formularios e mensagens de validacao

### Testar depois

- fluxos secundarios de perfil e contato

## Estrategia derivada do risco

1. Usar smoke curto para confirmar navegacao basica e pontos de entrada criticos.
2. Concentrar os primeiros casos detalhados em autenticacao e compra.
3. Registrar com prioridade qualquer falha que afete compra, acesso ou confiabilidade das informacoes.

## Hipoteses iniciais

- por ser um ambiente de pratica, podem existir mudancas ocasionais no catalogo ou em dados de exemplo
- o foco desta etapa esta na cobertura dos fluxos de maior impacto
