# Song Popularity
Aprendizagem Computacional — Departamento de Matemática, Universidade de Aveiro (2023/2024)

## Enquadramento
Este projeto foi desenvolvido no âmbito da Unidade Curricular de Aprendizagem Computacional, com o objetivo de aplicar técnicas de aprendizagem supervisionada a um problema de regressão real.
O dataset escolhido foi o [Song Popularity Dataset](https://www.kaggle.com/datasets/yasserh/song-popularity-dataset), disponível em [Kaggle](https://www.kaggle.com/), cujo objetivo é prever a popularidade de uma música com base em variáveis descritivas como energia, acústica, dançabilidade, vivacidade e outras características fornecidas pela plataforma Spotify.

## Objetivo
Criar e comparar modelos de regressão que permitam prever o valor da variável popularity de uma canção, explorando e avaliando diferentes métodos de modelação e otimização de parâmetros.

## Estrutura e Métodos Utilizados
O trabalho foi desenvolvido em R e encontra-se documentado no ficheiro `TC_GrupoD.Rmd`.
Foram testados três modelos principais:
1. **Boosting**:
    - Implementação com xgboost / gbm.
    - Ajuste de hiperparâmetros através de cross-validation.
2. **SVM (Support Vector Machines)**
    - Implementação com e1071.
    - Teste de diferentes kernels e parâmetros de regularização.
3. **Redes Neuronais Artificiais (ANNs)**
    - Implementação com neuralnet / nnet.
    - Ajuste do número de camadas e neurónios.

## Metodologia
1. Exploração e Pré-processamento dos Dados:
    - Análise de distribuições, correlações e detecção de outliers.
    - Normalização e remoção de valores ausentes.
    - Separação dos dados em training e testing sets.
2. Treino e Validação:
    - Aplicação de validação cruzada (k-fold).
    - Ajuste sistemático de hiperparâmetros para cada modelo.
3. Avaliação:
    - Métricas de desempenho:
        - RMSE (Root Mean Squared Error)
        - MAE (Mean Absolute Error)
        - R² (Coeficiente de Determinação)
    - Comparação dos resultados obtidos entre os três modelos.

## Resultados
Cada modelo foi avaliado com base nas métricas de erro e na capacidade de generalização sobre o conjunto de teste.
O relatório (.Rmd) inclui tabelas comparativas e gráficos que ilustram o desempenho de cada abordagem.
A análise sugere que o modelo Boosting apresentou o melhor equilíbrio entre precisão e capacidade de generalização, seguido da SVM e das Redes Neuronais.

## Autores
Trabalho desenvolvido por: Ana Rita Silva, Vasco Margarido e Vitor Tavares.
Mestrado em Bioinformática Clínica - Universidade de Aveiro — Departamento de Ciências Biomédicas
Ano letivo 2023/2024