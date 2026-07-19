Business Intelligence Aplicado a Vendas de Produtos Educacionais
Este projeto é uma solução de BI ponta a ponta, desenvolvida individualmente como parte da minha formação em análise de dados. Abrange desde a auditoria e limpeza de dados brutos, passando pela modelagem dimensional em estrela, até à construção de 3 dashboards interativos no Power BI, segmentados por área de negócio (Comercial, Financeiro, Marketing).
Problema de Negócio
Os dados brutos de vendas continham problemas reais de qualidade que, se ignorados, teriam gerado relatórios enganosos:

33,5% das transações (40.197 de 120.000) referenciavam produtos sem cadastro correspondente na tabela de produtos — um problema clássico de governança de dados que, sem tratamento, faria esses valores desaparecerem silenciosamente de qualquer análise por categoria.
Inconsistências de formatação em campos-chave (região e estado de clientes com múltiplas variações de maiúsculas/minúsculas e erros de digitação), que distorceriam qualquer segmentação geográfica.
Margem negativa presente em cerca de 1/3 das transações, sem causa aparente nos dados brutos.

Meu papel
Conduzi o projeto integralmente, do zero ao dashboard publicado: auditoria e limpeza dos dados em Power Query, modelagem do star schema (fato + 3 dimensões + tabela calendário), construção de mais de 15 medidas DAX (incluindo time intelligence, ranking e dimensões de papéis múltiplos com USERELATIONSHIP), e desenho dos 3 dashboards com foco em perguntas reais de stakeholder.
Dados & Stack
Dataset relacional (Vendas, Clientes, Produtos) — 120.000 transações, 3.000 clientes, 300 produtos.
Ferramentas: Power Query (ETL), modelagem dimensional (star schema), DAX (CALCULATE, RANKX, SAMEPERIODLASTYEAR, DATEADD, USERELATIONSHIP), Power BI Desktop.
Resultados / Achados

Identifiquei que 33% da receita total provinha de produtos sem cadastro válido — um achado que, numa empresa real, geraria ação imediata de governança de dados antes de qualquer decisão estratégica baseada nesses números.
Confirmei, via análise cruzada entre desconto médio e margem por canal, que a variação de rentabilidade entre canais não é explicada por política de desconto — a causa está na estrutura de custo, não no comportamento comercial.
Construí um modelo de dados resiliente a análises temporais duplas (data de venda vs. data de cadastro de cliente) usando relações inativas geridas por DAX.
