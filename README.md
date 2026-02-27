Dashboard de Gestão de Vendas – Power BI
📌 Objetivo

Este projeto consiste em um dashboard interativo desenvolvido no Power BI com o objetivo de apoiar a análise e o acompanhamento do desempenho de vendas ao longo do ano de 2023.

O painel foi construído para simular um cenário real de gestão comercial, permitindo:

Monitorar faturamento por loja

Avaliar desempenho por forma de pagamento

Analisar evolução mensal das vendas

Calcular crescimento percentual mês a mês

Comparar faturamento realizado versus meta mensal

Identificar participação percentual por produto

🏗 Estrutura do Modelo de Dados

O modelo foi construído seguindo boas práticas de BI, utilizando estrutura em formato estrela (Star Schema).

🔹 Tabelas

registroVendas (Fato)

ID Pedido

Data Pedido

Código Loja

Produto

Quantidade

Preço Unitário

Valor Vendido

Pagamento

lojas (Dimensão)

codigo_loja

nome_loja

Cidade

UF

DimData (Dimensão de Calendário)

Date

Ano

MesNumero

MesNome

AnoMes

AnoMes_Ordem

_Medidas
Tabela dedicada exclusivamente para organização das medidas do modelo.

🔗 Relacionamentos

DimData[Date] → registroVendas[Data Pedido]

lojas[codigo_loja] → registroVendas[Código Loja]

Direção de filtro: dimensão → fato.

📊 Principais Indicadores do Dashboard

Faturamento Total

Comissão

Ticket Médio

Crescimento Mensal (%)

Meta Mensal

Percentual de Atingimento da Meta

📈 Visuais Desenvolvidos

Gráfico de colunas: Faturamento por Loja

Gráfico de rosca: Distribuição por forma de pagamento

Gráfico combinado (coluna + linha): Faturamento vs Meta Mensal

Sparkline: Tendência de crescimento mensal

Tabela com formatação condicional: Participação por produto

Cards de KPI: Indicadores estratégicos

🎯 Problema de Negócio Simulado

O dashboard foi desenvolvido para responder às seguintes perguntas:

Qual loja apresenta melhor desempenho?

O faturamento está crescendo ou desacelerando?

A meta mensal está sendo atingida?

Qual produto possui maior participação no faturamento?

Como as vendas estão distribuídas por meio de pagamento?

🛠 Ferramentas Utilizadas

Power BI Desktop

DAX (Data Analysis Expressions)

Modelagem Dimensional

Inteligência temporal (Time Intelligence)

Formatação condicional

📌 Diferenciais Técnicos

Separação de medidas em tabela dedicada (_Medidas)

Uso de tabela calendário para cálculos temporais

Aplicação de crescimento mensal (MoM)

Implementação de meta e comparação visual (Realizado vs Meta)

Estrutura de modelo seguindo padrão estrela

📷 Preview



👤 Autor

Desenvolvido por Otávio Tavares
Projeto para portfólio de Business Intelligence
