# Prestação de Contas Eleitorais — TSE 2026

Projeto de análise de dados desenvolvido em **Power BI** a partir de dados públicos de prestação de contas eleitorais disponibilizados pelo Tribunal Superior Eleitoral (TSE).

## Objetivo

Explorar e analisar informações de receitas e despesas de candidatos, permitindo visualizar os dados de forma estruturada e facilitar a análise financeira das campanhas.

## Páginas do dashboard

- **Visão Geral**
- **Análise de Candidatos**
- **Despesas Detalhadas**
- **Comparação entre Partidos**

## Principais análises

- Total de receitas
- Total de despesas contratadas
- Total de despesas pagas
- Receitas por fonte
- Despesas por origem
- Valores por candidato
- Categorias de despesas
- Fornecedores
- Comparação entre despesas contratadas e pagas
- Comparação entre partidos

## Modelagem

O projeto utiliza um modelo de dados estruturado no Power BI, com tabelas auxiliares para apoiar os relacionamentos e as análises.

Entre as estruturas utilizadas estão:

- DimCandidato
- DimDespesa
- DimPartidoA
- DimPartidoB
- ComparativoPartido

As tabelas de fatos foram mantidas separadas para organizar os dados de receitas e despesas.

## Ferramentas

- Power BI
- DAX
- Modelagem de Dados
- Business Intelligence (BI)

## Dados

Os dados utilizados são públicos e foram obtidos no **Portal de Dados Abertos do TSE**, no conjunto **Prestação de Contas Eleitorais - 2026**.

Fonte oficial:  
https://dadosabertos.tse.jus.br/pt_BR/dataset/prestacao-de-contas-eleitorais-2026

Os arquivos CSV utilizados na análise não estão armazenados neste repositório devido ao grande volume dos dados. Eles podem ser obtidos diretamente na fonte oficial do TSE.

## Arquivo do projeto

O arquivo .pbix disponibilizado neste repositório contém o dashboard e o modelo desenvolvido para a análise.
