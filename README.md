# Portfólio de Dados, BI e Power BI

Projetos de análise de dados, Business Intelligence e Power BI.

## Projetos

### Prestação de Contas Eleitorais — TSE 2026

Dashboard desenvolvido em Power BI para análise das prestações de contas eleitorais de 2026, utilizando dados públicos do Tribunal Superior Eleitoral (TSE).

O projeto contém 4 páginas:

1. **Visão Geral** — receitas e despesas dos candidatos.
2. **Análise por Candidato** — análise de receitas, despesas contratadas e cargos.
3. **Análise Detalhada das Despesas** — despesas contratadas e pagas, fornecedores e origens.
4. **Comparativo entre Partidos** — comparação de receitas e despesas contratadas entre dois partidos selecionados.

### Bases utilizadas

Foram utilizadas exclusivamente estas três bases:

- `receitas_candidatos_2026_BRASIL`
- `despesas_contratadas_candidatos_2026_BRASIL`
- `despesas_pagas_candidatos_2026_BRASIL`

O modelo utiliza dimensões auxiliares para relacionar candidatos, despesas e permitir o comparativo independente entre dois partidos.

### Fonte

Tribunal Superior Eleitoral — Dados Abertos  
https://dadosabertos.tse.jus.br/pt_BR/dataset/prestacao-de-contas-eleitorais-2026

> Os arquivos de dados brutos não são armazenados neste repositório. O projeto utiliza a fonte oficial do TSE.

## Ferramentas

- Power BI
- DAX
- Modelagem dimensional
- Análise de dados
