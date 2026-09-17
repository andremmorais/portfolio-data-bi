# portfolio-data-bi
Portfólio de projetos em Dados, Business Intelligence e Power BI.

# Emendas Parlamentares — Power BI

Projeto de análise de dados de Emendas Parlamentares desenvolvido com Power BI, utilizando dados públicos do Portal da Transparência.

## Objetivo

Desenvolver um painel analítico para explorar informações relacionadas às emendas parlamentares, seus autores, destinos, classificações e execução financeira.

O projeto foi estruturado em seis páginas de análise:

1. **Visão Geral**
2. **Autores das Emendas**
3. **Destino dos Recursos**
4. **Perfil das Emendas**
5. **Execução Orçamentária**
6. **Análise Detalhada**

## Dados

A base utilizada contém informações de Emendas Parlamentares e foi obtida a partir de dados públicos do Portal da Transparência referentes ao período de 2014 a 2026.

Principais informações utilizadas:

- Ano da Emenda
- Código da Emenda
- Número da emenda
- Nome do Autor da Emenda
- Tipo de Emenda
- UF
- Município
- Região
- Localidade de aplicação do recurso
- Nome Função
- Nome Subfunção
- Nome Programa
- Nome Ação
- Nome Plano Orçamentário
- Valor Empenhado
- Valor Liquidado
- Valor Pago
- Valores relacionados a Restos a Pagar

## Ferramentas

- Power BI
- Power Query
- DAX

## Principais medidas DAX

```DAX
Total Empenhado =
SUM(EmendasParlamentares[Valor Empenhado])
Total Liquidado =
SUM(EmendasParlamentares[Valor Liquidado])
Total Pago =
SUM(EmendasParlamentares[Valor Pago])
% Pago sobre Empenhado =
DIVIDE(
    [Total Pago],
    [Total Empenhado],
    0
)
Quantidade de Emendas =
DISTINCTCOUNT(EmendasParlamentares[Código da Emenda])

Estrutura do Dashboard
01 — Visão Geral

Apresenta uma visão consolidada dos valores empenhados, liquidados e pagos, além da distribuição dos recursos pagos por função.

02 — Autores das Emendas

Analisa os recursos pagos e a quantidade de emendas por autor, permitindo explorar os principais registros da base.

03 — Destino dos Recursos

Apresenta a distribuição dos recursos pagos por UF e permite analisar o destino geográfico dos recursos.

04 — Perfil das Emendas

Explora as emendas segundo tipo, região, apoiador/solicitante, função, programa e ação.

05 — Execução Orçamentária

Apresenta a execução financeira por ano e informações relacionadas a empenho, liquidação, pagamento e Restos a Pagar.

06 — Análise Detalhada

Permite consultar uma emenda específica por meio do Código da Emenda e visualizar sua identificação, destino, classificação orçamentária e execução financeira.

Visualizações

Visão Geral

Autores das Emendas

Destino dos Recursos

Perfil das Emendas

Execução Orçamentária

Análise Detalhada

Arquivos

Arquivo .pbix com o desenvolvimento do dashboard.

Base de dados utilizada no projeto, disponibilizada em arquivo compactado.

Imagens das páginas do dashboard.

Fonte dos dados

Portal da Transparência — dados públicos de Emendas Parlamentares.

Observação

Este projeto tem finalidade analítica e de portfólio, utilizando dados públicos para exploração e visualização de informações.
