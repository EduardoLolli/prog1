# Análise de Dados de Viagens Globais

## Alunos: 
* José Eduardo Fernandes Lolli
* Arthur Anício Carvalho Morais Silva


#### Dataset: [Traveler-trip-data](https://www.kaggle.com/datasets/rkiattisak/traveler-trip-data)
#### Motivação do Projeto:
O objetivo principal deste trabalho é aplicar os conhecimentos de análise e manipulação de dados com Python para explorar tendências e padrões a respeito de viagens globais. A motivação vem do interesse pessoal sobre viagens e como fatores geográficos e financeiros se relacionam com as escolhas e a duração de viagens.

## Conjunto de Dados

- Nome do Dataset: Traveler Trip Data

- Fonte: Kaggle

- Descrição: O arquivo Travel details dataset.csv contém informações detalhadas sobre viagens, incluindo destino, datas de início e fim, duração, características do viajante (idade, gênero, nacionalidade), tipo/custo de acomodação e tipo/custo de transporte.

## Insights a Serem Extraídos

* Quais são os 10 destinos mais visitados pelos viajantes segundo o dataset?

* Qual é o meio de transporte mais comum e qual é a relação entre seu custo médio e a duração média da viagem?

* Qual é o custo médio e quais destinos ou tipos de acomodação são mais "caros" ou "econômicos" por dia?

* Quais são as viagens com os maiores custos totais e o que as torna caras?

* Existe uma correlação entre a idade do viajante e a duração da viagem?

## Detalhamento dos Passos Realizados

### Primeiro Insight: Quais são os 10 destinos mais visitados pelos viajantes segundo o dataset?

* 1º - Inicializado um gráfico com matplotlib.

* 2º - Inicializada a variável "top_destinos" com os top 10 destinos, por meio da lib do pandas.

* 3º - Definido no gráfico de barras, no eixo X, com os valores referentes a quantidade de visitas e o eixo Y com o indice referente ao nome de cada destino de viagens.


### Segundo Insight: Qual é o meio de transporte mais comum e qual é a relação entre seu custo médio e a duração média da viagem?

* 1º - Realizada a limpeza dos valores de custos de transporte, eliminando os caracteres que não são referentes aos valores numéricos e formatando os valores para numeros decimais (float)

* 2º - Inicializado um dicionário com as traduções dos meios de transporte

* 3º - Agrupamento, remoção de valores nulos e reordenação dos valores de médias
 
* 4º - Inicialização dos gráficos, criando o ax1 e ax2 que compartilham o mesmo eixo da figura

* 5º - Inseridos detalhes visuais no gráfico, colocaração de cada linha do gráfico, legenda, posicionamento , etc.


### Terceiro Insight: Qual é o custo médio e quais destinos ou tipos de acomodação são mais "caros" ou "econômicos" por dia?

* 1º - Limpeza do valores de custo de acomodação, eliminando caracteres que não são referentes aos valores numéricos e formatando os valores para decimal

* 2º - Inicializado um dicionário salvando os valores de cuso de cada tipo de acomodação a chave equivalente ao tipo de acomodação. 

* 3º - Feita a separação dos valores a serem utilizados no cabeçalho e legenda dos gráfico 

* 4º - Iniciado gráfico de barras em sentido decrescente de acordo com o custo

### Quarto Insight: Quais são as viagens com os maiores custos totais e o que as torna caras?

* 1º - Criada uma nova coluna somando-se o custo total da viagem.

* 2º - Inicializada uma tabela com os 5 maiores custos.

### Quinto Insight: Existe uma correlação entre a idade e gênero do viajante e a duração da viagem?

* 1º - Criado um array com o range das faixas etárias que serão utilizadas como legenda.

* 2º - Separação dos dados de idades de acordo com o gênero

* 3º - Agrupados dadaos relacionados a cada genero

* 4º - Criados dois gráficos em sentidos opostos, à esquerda masculino e à direita feminino
