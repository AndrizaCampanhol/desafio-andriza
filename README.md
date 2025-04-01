# Desafio Técnico Zeit 2025

O desafio consiste em predizer o preço da habitação a partir de informações do senso de California de 1990.

As colunas do dataset são as seguintes:
- **longitude**: Longitude geográfica.
- **latitude**: Latitude geográfica.
- **housing_median_age**: Idade média das habitações na região, medida em anos.
- **total_rooms**: Número total de cômodos em todas as unidades habitacionais da área analisada.
- **total_bedrooms**: Número total de quartos em todas as unidades habitacionais da área analisada.
- **population**: População total residente na área geográfica correspondente ao imóvel.
- **households**: Número total de domicílios na região, representando unidades familiares ou habitacionais.
- **median_income**: Renda mediana dos moradores da região, expressa em múltiplos de 1.000 dólares.
- **median_house_value**: Valor mediano das residências na área, representado em dólares.
- **ocean_proximity**: Proximidade da localização em relação ao oceano, categorizada por rótulos como "Perto da Baía" (Near Bay), "Perto do Oceano" (Near Ocean), "Interior" (Inland), entre outros.

O candidato deve apresentar um modelo que faça a predição do preço da habitação (o candidato é livre para entregar mais de um modelo).

Disponibilizamos um [template](desafio.ipynb) no formato [Notebook Jupyter](https://jupyter.org/) para o desafio e os dados estão disponíveis neste [arquivo](housing.csv)

# Desafio Bônus (não obrigatório)

O desafio consiste em predizer **propriedades do solo** a partir de near-infrared spectroscopy (NIRS). O infravermelho-próximo (NIR) é uma região do espectro eletromagnético situada entre a luz visível e o infravermelho médio, um espectro na região do NIR refere-se à distribuição da intensidade da radiação em função do comprimento de onda ou frequência. A espectroscopia de infravermelho-próximo (NIRS) é uma técnica não destrutiva que busca identificar e quantificar componentes químicos a partir da interação da radiação, emitida por uma lâmpada, com a matéria e possui diversos usos nas áreas alimentícias, farmacêuticas, entre outras. No dataset temos as seguintes propriedades do solo:

- Porcentagem de Carbono Orgânico   
- Porcentagem de Carbono Total
- Porcentagem de Nitrogênio Total
- Porcentagem de Argila
- Porcentagem de Areia
- Porcentagem de Lodo
- Densidade Aparente
- pH da Água
- Carbonato
- Potássio

Todas essas são características importantes para avaliar a qualidade do solo. Seu trabalho é usar um algoritmo de Machine Learning para predizer esses dados a partir dos dados do espectro de cada amostra, cada um com uma distância de 2nm e alcance de 1350-2550nm e apresentar métricas como [RMSE](https://en.wikipedia.org/wiki/Root_mean_square_deviation) e [R²](https://pt.wikipedia.org/wiki/Coeficiente_de_determina%C3%A7%C3%A3o). Como desafio o candidato deve decidir:

- Como lidar com os dados ausentes na tabela
- Quais métodos de preprocessamento utilizar
- Quais algoritmos de Machine Learning utilizar
- Quais outras métricas usar para avaliar o modelo
- Como apresentar os resultados

O candidato é livre para entregar mais de um algoritmo e discutir pontos fortes e fracos de cada abordagem (recomendado). Também recomenda-se fortemente o uso do PyTorch, visto que essa é a biblioteca utilizada na empresa.

Os dados para o desafio bônus estão neste [arquivo](dados_nir.csv)