# 🎬 IMDb Movie Rating Prediction
## 1. Descrição do Projeto

Este projeto utiliza dados da base de filmes do IMDb para realizar a predição da nota de filmes. A ideia é desenvolver um modelo de machine learning capaz de estimar a avaliação (rating) de um filme com base em variáveis como ano de lançamento, duração, gênero, número de votos, arrecadação, entre outras.

O projeto envolve etapas de Exploração de Dados (EDA), pré-processamento, modelagem e avaliação do modelo, fornecendo insights sobre quais fatores influenciam a nota de um filme.

## 2. Base de Dados

A base de dados utilizada contém informações de filmes do IMDb, incluindo:

* Released_Year: Ano de lançamento do filme

* Runtime_min: Duração do filme em minutos

* Meta_score: Avaliação da crítica especializada

* No_of_Votes: Número de votos recebidos

* Gross_clean: Arrecadação em valor numérico

* Certificate: Classificação indicativa

* Genre: Gênero do filme

* IMDB_Rating: Nota do filme (variável alvo)

A base permite explorar distribuições de notas, frequência de gêneros e certificações, além de identificar outliers e ruídos nos dados.

## 3. Objetivo

O objetivo principal é prever a nota de um filme (IMDB_Rating) com base em variáveis relevantes, utilizando técnicas de machine learning.

Tipo de problema: Regressão

Algoritmo utilizado: Random Forest Regression

Métrica de avaliação: Root Mean Squared Error (RMSE)

## 4. Pré-processamento

Antes de treinar o modelo, foram realizadas etapas importantes de limpeza e transformação de dados:

Conversão de colunas para tipos numéricos (Released_Year, Runtime_min, Gross_clean)

Tratamento de valores nulos (Certificate, Gross)

Identificação e remoção de ruídos em notas, anos e duração

Exploração de variáveis categóricas (Genre, Certificate) e análise de correlação com a nota

## 5. Modelagem

O modelo Random Forest Regression foi treinado utilizando as variáveis selecionadas.

Divisão entre treino e teste para avaliação do desempenho.

Métrica principal utilizada: RMSE, que mede o erro médio entre a nota prevista e a nota real.

## 6. Resultados

O modelo apresenta boa capacidade de aproximação das notas reais, considerando fatores como gênero, número de votos e arrecadação.

Análises exploratórias indicaram tendências importantes, como:

Filmes com mais votos tendem a ter avaliações mais estáveis.

Gênero e classificação indicativa influenciam a nota.

Duração e arrecadação apresentam correlação moderada com a nota

## 7. Como Executar

* 1. Clone o repositório:

* git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git

* 2. Entre na pasta do projeto:

* cd NOME_DO_REPOSITORIO

* 3. Instale as dependências:

* pip install -r requirements.txt

* 4. Abra o notebook no Jupyter ou Colab e execute as células para reproduzir os resultados.

O modelo treinado está disponível como modelo_filmes.pkl e pode ser carregado para fazer predições futuras.
