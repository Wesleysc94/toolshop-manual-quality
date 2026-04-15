# 📋 toolshop-manual-quality

> Projeto de QA manual com planejamento, execução smoke, bug reports e recomendação de release.

[![Bugs encontrados](https://img.shields.io/badge/Bugs-2%20defeitos-red)](bug-reports/)
[![Recomendação](https://img.shields.io/badge/Release-No%20Go-red)]()
[![Produto](https://img.shields.io/badge/Produto-Practice%20Software%20Testing-blue)](https://practicesoftwaretesting.com/)

📦 **Parte do portfolio:** [toolshop-quality-portfolio](https://github.com/Wesleysc94/toolshop-quality-portfolio)

---

## Objetivo

Demonstrar a capacidade de conduzir uma rodada completa de QA manual — do planejamento à recomendação final — sobre um produto real, documentando cada etapa de forma reproduzível.

Este projeto responde à pergunta que um tech lead faria: **"Se eu te der um produto novo hoje, como você começa a testar?"**

---

## Produto sob teste

| Recurso | URL |
|---|---|
| Aplicação web | https://practicesoftwaretesting.com/ |
| Referência de API | https://practiceautomatedtesting.com/api |
| Swagger | https://practiceautomatedtesting.com/swagger |

---

## O que foi feito

### 1. Planejamento

- Mapeamento do escopo funcional (o que entra e o que fica de fora)
- Análise de risco para priorizar os fluxos mais críticos
- Criação do plano de testes com critérios de entrada e saída

### 2. Escopo priorizado

Fluxos que entraram na primeira rodada:

- ✅ Autenticação (login e logout)
- ✅ Catálogo de produtos
- ✅ Busca e filtros
- ✅ Carrinho de compras
- ✅ Checkout
- ✅ Contato e perfil

Fluxos que ficaram de fora (decisão documentada):

- ⏳ Automação web e API (cobertos em repositórios separados)
- ⏳ Testes mobile
- ⏳ Performance
- ⏳ Área administrativa

### 3. Execução

- Rodada smoke executada em 2026-04-14
- Reteste de autenticação com conta demo oficial
- Todas as execuções registradas com evidências

### 4. Resultado

| Métrica | Valor |
|---|---|
| Defeitos encontrados | **2** |
| Retestes realizados | 1 (autenticação) |
| Login/Logout no reteste | ✅ Confirmado |
| Recomendação final | **❌ No Go** |

> A recomendação **No Go** foi emitida porque os defeitos encontrados impactam fluxos críticos do produto. Isso demonstra independência de julgamento — o papel do QA é informar riscos, não aprovar entregas por pressão.

---

## Estrutura do repositório

```
toolshop-manual-quality/
├── README.md                    ← Você está aqui
├── RESUMO-DO-PROJETO.txt        ← Leitura rápida (2 min)
├── 00-LEIA-PRIMEIRO.txt         ← Orientação inicial
├── docs/
│   ├── escopo.md                ← O que entra e o que fica de fora
│   ├── plano-de-testes.md       ← Critérios, abordagem, riscos
│   ├── analise-de-risco.md      ← Priorização por impacto
│   └── guia-de-revisao.md       ← Trilha de leitura pra avaliadores
├── checklists/                  ← Checklist smoke da rodada
├── test-cases/                  ← Casos de teste por área funcional
├── bug-reports/                 ← Defeitos com reprodução e evidência
├── execution-reports/           ← Relatórios das execuções
├── release/                     ← Recomendação final (No Go)
└── evidence/                    ← Screenshots e registros de apoio
```

---

## Como revisar

Se você está avaliando este trabalho, siga esta ordem:

1. **[RESUMO-DO-PROJETO.txt](RESUMO-DO-PROJETO.txt)** — Visão geral em 2 minutos
2. **[docs/guia-de-revisao.md](docs/guia-de-revisao.md)** — Trilha completa de leitura
3. **[execution-reports/](execution-reports/)** — O que aconteceu na rodada
4. **[bug-reports/](bug-reports/)** — Os defeitos encontrados
5. **[release/2026-04-14-recomendacao-de-release.md](release/2026-04-14-recomendacao-de-release.md)** — Parecer final

## Como validar

Este projeto é manual, então a validação é por reprodução:

1. Acesse [practicesoftwaretesting.com](https://practicesoftwaretesting.com/)
2. Siga os casos de teste em `test-cases/`
3. Compare com os bugs registrados em `bug-reports/`
4. Confira as evidências em `evidence/`

---

## O que este projeto demonstra

- **Planejamento antes de execução** — escopo e risco definidos antes de abrir o navegador
- **Bug reports profissionais** — passos de reprodução, severidade, impacto e evidência
- **Parecer técnico independente** — recomendação No Go baseada em dados, não em opinião
- **Documentação reproduzível** — qualquer pessoa pode seguir os mesmos passos e validar os resultados
