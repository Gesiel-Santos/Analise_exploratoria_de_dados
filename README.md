# Neste projeto, eu utilizei a técnica de regressão linear para analisar os impactos de algumas variáveis sobre o consumo de cerveja em São Paulo.
A regressão linear é um método estatístico que permite estimar o valor esperado de uma variável dependente a partir de uma ou mais variáveis independentes.

O objetivo do projeto foi criar um modelo de previsão para o consumo médio de cerveja segundo os inputs de temperatura, chuva e final de semana.

Para isso, eu segui os seguintes passos:

=> Conheci o dataset, que contém dados de consumo de cerveja, temperatura, chuva e final de semana em uma área universitária de São Paulo.

=> Importei as bibliotecas necessárias para manipular os dados e gerar gráficos, como pandas, matplotlib, numpy, seaborn e sklearn.

=> Explorei os dados através de estatísticas descritivas, matriz de correlação e análises gráficas, como box plot, distribuição de frequências, pair plot, joint plot e lm plot.

=> Estimei um modelo de regressão linear simples usando a classe LinearRegression do sklearn, utilizando a temperatura máxima como variável explicativa e o consumo de cerveja como variável dependente.

=> Avaliei o modelo através do coeficiente de determinação (R²) e outras métricas de regressão, como o erro quadrático médio (EQM) e a raiz do erro quadrático médio (REQM).

=>Comparei o modelo com outro modelo que utilizou a temperatura média como variável explicativa e verifiquei qual teve melhor ajuste aos dados.

=>Criei um simulador simples para gerar previsões pontuais de consumo de cerveja a partir dos valores de entrada das variáveis explicativas.
Salvei e carreguei o modelo estimado usando a biblioteca pickle.
