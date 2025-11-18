# Análise de Dados de Viagens Globais

## Aluno: José Eduardo Fernandes Lolli


* Dataset: [Traveler-trip-data](https://www.kaggle.com/datasets/rkiattisak/traveler-trip-data)
* Motivação do Projeto:
O objetivo principal deste trabalho é aplicar os conhecimentos de análise e manipulação de dados com Python para explorar tendências e padrões a respeito de viagens globais. A motivação vem do interesse pessoal sobre viagens e como fatores geográficos e financeiros se relacionam com as escolhas e a duração de viagens.

## Conjunto de Dados

- Nome do Dataset: Traveler Trip Data

- Fonte: Kaggle

- Descrição: O arquivo Travel details dataset.csv contém informações detalhadas sobre viagens, incluindo destino, datas de início e fim, duração, características do viajante (idade, gênero, nacionalidade), tipo/custo de acomodação e tipo/custo de transporte.

## Insights a Serem Extraídos

* Quais são os 10 destinos mais visitados pelos viajantes segundo o dataset?

* Qual é o meio de transporte mais comum e qual é a relação entre seu custo médio e a duração média da viagem?

* Qual é o custo total médio da viagem e como ele se distribui?

* Qual é o custo médio por dia e quais destinos ou tipos de acomodação são mais "caros" ou "econômicos" por dia?

* Quais são as viagens com os maiores custos totais e o que as torna caras?

* Existe uma correlação entre a idade do viajante e a duração da viagem?

* Quais são os meses de pico para viagens e como a duração média e o custo médio variam ao longo do ano?

## Detalhamento dos Passos Realizados

1. Limpeza e Preparação de Dados
Conversão de Tipos: Conversão das colunas Accommodation cost, Transportation cost, Duration (days) e Traveler age para tipos numéricos (float/int).

Tratamento de Datas: Conversão das colunas Start date e End date para o tipo datetime.

Tratamento de Valores Ausentes: (A ser detalhado: Ex.: Remoção de linhas com dados faltantes (NaN) ou preenchimento com a média/moda, dependendo da coluna).

Criação de Novas Colunas:

Custo Total: Accommodation cost + Transportation cost.

Custo Diário Médio: Custo Total / Duration (days).

Mês de Início: Extraído da coluna Start date para análise de sazonalidade.

2. Análises e Visualizações
Análise de Frequência: Utilização de value_counts() e gráficos de barras para Destinos, Tipos de Acomodação e Tipos de Transporte.

Análise de Médias: Utilização de groupby() para calcular médias de custo e duração agrupadas por gênero, nacionalidade e tipo de acomodação.

Análise de Correlação: Cálculo do coeficiente de correlação entre idade e duração da viagem.

Visualizações: (A ser detalhado: Ex.: Gráficos de dispersão, Boxplots, Gráficos de Linha para sazonalidade, Mapas (se possível) para destinos).

