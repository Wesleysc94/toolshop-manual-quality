# 📋 toolshop-manual-quality

> Projeto de QA manual com planejamento, execução smoke, bug reports e recomendação de release.

[![Bugs encontrados](https://img.shields.io/badge/Bugs-2%20defeitos-red)](bug-reports/)
[![Recomendação](https://img.shields.io/badge/Release-No%20Go-red)]()
[![Produto](https://img.shields.io/badge/Produto-Practice%20Software%20Testing-blue)](https://practicesoftwaretesting.com/)

🔎 **Portfolio principal:** [Wesleysc94](https://github.com/Wesleysc94/Wesleysc94)
📦 **Case Study 1:** [toolshop-quality-portfolio](https://github.com/Wesleysc94/toolshop-quality-portfolio)

---

## Objetivo

Esta etapa cobre uma rodada completa de QA manual sobre um produto real, da preparação inicial até a recomendação final de release.

Este projeto responde a uma pergunta simples de contexto profissional: se eu receber um produto novo hoje, como organizo o começo da validação, documento os achados e comunico risco com clareza?

---

## Produto sob teste

| Recurso | URL |
|---|---|
| Aplicação web | https://practicesoftwaretesting.com/ |
| Referência de API | https://practiceautomatedtesting.com/api |
| Swagger | https://practiceautomatedtesting.com/swagger |

---

## Escopo da rodada

Fluxos priorizados na primeira rodada:

- autenticação
- catálogo de produtos
- busca e filtros
- carrinho
- checkout
- contato e perfil

Fora do escopo desta etapa:

- automação web e API
- testes mobile
- performance
- área administrativa

---

## O que foi validado

### Planejamento

- definição de escopo funcional
- análise de risco
- plano de testes com critérios de entrada e saída

### Execução

- rodada smoke registrada em 2026-04-14
- reteste de autenticação com conta demo oficial
- evidências consolidadas em relatórios e screenshots

### Resultado

| Métrica | Valor |
|---|---|
| Defeitos encontrados | **2** |
| Retestes realizados | 1 |
| Login/Logout no reteste | ✅ Confirmado |
| Recomendação final | **❌ No Go** |

---

## Stack e artefatos

| Camada | Uso |
|---|---|
| **QA Manual** | checklist smoke, casos de teste e bug reports |
| **Documentação** | Markdown para escopo, plano, risco e relatórios |
| **Evidências** | screenshots e registros da execução |

---

## Como revisar

1. Leia o [RESUMO-DO-PROJETO.txt](RESUMO-DO-PROJETO.txt)
2. Consulte o [docs/guia-de-revisao.md](docs/guia-de-revisao.md)
3. Abra os relatórios em [execution-reports/](execution-reports/)
4. Leia os bugs em [bug-reports/](bug-reports/)
5. Feche com a recomendação em [release/2026-04-14-recomendacao-de-release.md](release/2026-04-14-recomendacao-de-release.md)

---

## Como validar

Este projeto é manual, então a validação é por reprodução:

1. Acesse [practicesoftwaretesting.com](https://practicesoftwaretesting.com/)
2. Siga os casos de teste em `test-cases/`
3. Compare os resultados com os bugs documentados
4. Confira as evidências em `evidence/`

---

## O que este projeto entrega

- **Planejamento antes de execução** — escopo e risco definidos antes da rodada
- **Bug reports com rastreabilidade** — passos de reprodução, impacto e evidência
- **Comunicação de risco** — recomendação de release baseada em resultado concreto
- **Execução verificável** — outra pessoa consegue seguir o mesmo caminho de validação
