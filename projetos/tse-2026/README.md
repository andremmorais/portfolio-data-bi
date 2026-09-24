# Prestação de Contas Eleitorais — TSE 2026

Projeto de Power BI desenvolvido para análise dos dados públicos de prestação de contas eleitorais de 2026.

## Estrutura do dashboard

### 01 — Visão Geral
- Total de receitas
- Total de despesas contratadas
- Total de despesas pagas
- Receitas por fonte
- Despesas contratadas por origem
- Despesas pagas por origem

### 02 — Análise por Candidato
- Total de candidatos
- Total de receitas
- Total de despesas contratadas
- Receitas por candidato
- Despesas contratadas por candidato
- Candidatos por cargo

### 03 — Análise Detalhada das Despesas
- Despesas contratadas
- Despesas pagas
- Percentual pago
- Despesas por categoria/origem
- Despesas por fornecedor
- Comparativo entre despesas contratadas e pagas

### 04 — Comparativo entre Partidos
- Seleção independente do Partido A
- Seleção independente do Partido B
- Receitas por partido
- Despesas contratadas por partido

A comparação apresenta os valores registrados nas bases, sem classificação ou indicação de preferência entre partidos.

## Dados utilizados

- `receitas_candidatos_2026_BRASIL`
- `despesas_contratadas_candidatos_2026_BRASIL`
- `despesas_pagas_candidatos_2026_BRASIL`

Fonte oficial: Tribunal Superior Eleitoral (TSE), Prestação de Contas Eleitorais 2026.

https://dadosabertos.tse.jus.br/pt_BR/dataset/prestacao-de-contas-eleitorais-2026

## Modelagem

O projeto utiliza dimensões auxiliares para evitar relacionamentos diretos inadequados entre tabelas de fatos:

- `DimCandidato`
- `DimDespesa`
- `DimPartidoA`
- `DimPartidoB`
- `ComparativoPartido`

As tabelas de fatos permanecem separadas, com dimensões intermediárias para os relacionamentos necessários.

## Ferramentas

Power BI · DAX · Modelagem de Dados · Business Intelligence
