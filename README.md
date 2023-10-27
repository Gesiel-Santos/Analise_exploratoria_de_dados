# Análise exploratória de dados sobre o consumo de cerveja em São Paulo 🍻

Neste projeto, eu utilizei a técnica de **regressão linear** para analisar os impactos de algumas variáveis sobre o **consumo médio de cerveja** em uma área universitária de São Paulo.

## Dados 📊

Os dados foram obtidos do [Kaggle](^1^) e contêm as seguintes variáveis:

- **Data**: data da observação
- **Temperatura Media (C)**: temperatura média do dia
- **Temperatura Minima (C)**: temperatura mínima do dia
- **Temperatura Maxima (C)**: temperatura máxima do dia
- **Precipitacao (mm)**: precipitação do dia
- **Final de Semana**: indica se o dia é final de semana ou não
- **Consumo de cerveja (litros)**: consumo médio de cerveja na área universitária



## Bibliotecas 📚

As bibliotecas utilizadas neste projeto foram:

- **pandas**: para manipular os dados
- **matplotlib**: para gerar gráficos
- **numpy**: para operações numéricas
- **seaborn**: para gerar gráficos estatísticos
- **sklearn**: para estimar e avaliar o modelo de regressão linear
- **pickle**: para salvar e carregar o modelo estimado

## Análise 🔎

A análise foi dividida em quatro etapas:

1. Exploração dos dados: nesta etapa, eu verifiquei as características dos dados, como o número de observações, os tipos das variáveis, os valores ausentes, as estatísticas descritivas e a matriz de correlação.
2. Análise gráfica: nesta etapa, eu utilizei diferentes tipos de gráficos para visualizar a distribuição, a relação e a tendência das variáveis, como box plot, histograma, pair plot, joint plot e lm plot.
3. Estimação do modelo: nesta etapa, eu estimei um modelo de regressão linear simples usando a classe LinearRegression do sklearn, utilizando a temperatura máxima como variável explicativa e o consumo de cerveja como variável dependente. Eu também comparei o modelo com outro modelo que utilizou a temperatura média como variável explicativa e verifiquei qual teve melhor ajuste aos dados.
4. Avaliação do modelo: nesta etapa, eu avaliei o modelo através do coeficiente de determinação (R²) e outras métricas de regressão, como o erro quadrático médio (EQM) e a raiz do erro quadrático médio (REQM). Eu também criei um simulador simples para gerar previsões pontuais de consumo de cerveja a partir dos valores de entrada das variáveis explicativas. Eu salvei e carreguei o modelo estimado usando a biblioteca pickle.


## Resultados 🏆

Os principais resultados obtidos foram:

- O consumo médio de cerveja na área universitária foi de 25,4 litros por dia, com um desvio padrão de 4,4 litros.
- O consumo médio de cerveja foi maior nos finais de semana (28,9 litros) do que nos dias úteis (23,4 litros).
- O consumo médio de cerveja teve uma correlação positiva com a temperatura máxima (0,64) e uma correlação negativa com a precipitação (-0,19).
- O modelo que utilizou a temperatura máxima como variável explicativa teve um R² de 0,41, um EQM de 5,74 e um REQM de 2,40. O modelo que utilizou a temperatura média como variável explicativa teve um R² de 0,32, um EQM de 6,81 e um REQM de 2,61. Portanto, o modelo com a temperatura máxima teve um melhor ajuste aos dados.
- O simulador mostrou que, para uma temperatura máxima de 30°C, uma precipitação de 0 mm e um final de semana, o consumo médio previsto de cerveja seria de 31 litros por dia.

## Conclusão 🎓

A conclusão deste projeto foi que a técnica de regressão linear foi útil para analisar os impactos de algumas variáveis sobre o consumo médio de cerveja em São Paulo. O modelo estimado mostrou que a temperatura máxima foi a variável mais relevante para explicar o consumo de cerveja, seguida pelo final de semana. O modelo também permitiu gerar previsões pontuais de consumo de cerveja a partir dos valores de entrada das variáveis explicativas. No entanto, o modelo teve um R² relativamente baixo, o que indica que há outros fatores que podem influenciar o consumo de cerveja que não foram considerados neste projeto. Portanto, sugere-se que sejam realizadas novas análises com mais dados e mais variáveis para aprimorar o modelo e obter resultados mais precisos e confiáveis.

