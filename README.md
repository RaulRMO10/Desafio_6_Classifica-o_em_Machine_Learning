# Desafio 6 Escola DNC : Preveja os usuários com alta chance de deixar seu Streaming

Quero compartilhar um projeto que concluí recentemente, onde desenvolvi um modelo preditivo para identificar usuários com alta chance de deixar um serviço de streaming. Abaixo, descrevo brevemente as etapas que segui para alcançar os resultados.

## Etapa 01: Análise exploratória dos dados (Data Understanding)

- **Carregamento da base de dados:** Importei a base de dados relevante para o projeto.
- **Descrição estatística dos dados:** Realizei uma análise estatística detalhada, examinando medidas como média, mediana, desvio padrão e outras estatísticas descritivas.
- **Verificação dos tipos de dados:** Identifiquei e verifiquei os tipos de dados presentes no dataset, como numéricos, categóricos e texto, para garantir a consistência e a integridade das informações.

## Etapa 02: Tratamento dos Dados (Data Preparation)

- **Substituição de valores “NaN” por 0:** Substituí valores nulos nas colunas Time_on_platform, Num_streaming_services, Churned, Avg_rating e Devices_connected.
- **Remoção de linhas nulas:** Removi linhas com valores nulos nas colunas Gender, Subscription_type e Age.
- **Transformação de valores churned:** Converti os valores da coluna Churned de 0 e 1 para No e Yes.
- **Conversão de valores floats:** Transformei valores do tipo float em valores inteiros para facilitar a análise.

## Etapa 03: Modelagem dos Dados - Regressão Logística

- **Definição de variáveis X e y:** Defini as variáveis independentes (X) e a variável dependente (y) para o modelo de regressão logística.
- **Treinamento do modelo:** Utilizei o método `.fit` para ajustar o modelo aos dados.
- **Separação dos dados em train e test:** Dividi os dados em conjuntos de treino e teste para validação do modelo.
- **Realização da modelagem:** Executei o processo de modelagem com os dados de treino.
- **Plotagem da matriz de confusão:** Gereia matriz de confusão para avaliar o desempenho do modelo.
- **Impressão das métricas:** Calculei e imprimi métricas de desempenho como acurácia, precisão, recall e F1-score.

## Etapa 04: Modelagem dos Dados - Tuning

- **Definição de variáveis X e y:** Defini as variáveis independentes (X) e a variável dependente (y) para o modelo de previsão de churn.
- **Treinamento do modelo:** Utilizei o método `.fit` para ajustar o modelo aos dados, focando na previsão de usuários com alta chance de deixar o serviço de streaming.
- **Separação dos dados em train e test:** Dividi os dados em conjuntos de treino e teste para validação do modelo.
- **Realização da modelagem:** Executei o processo de modelagem com os dados de treino, aplicando técnicas de tuning para melhorar a performance do modelo.
- **Plotagem da matriz de confusão:** Gereia matriz de confusão para avaliar o desempenho do modelo ajustado.
- **Impressão das métricas:** Calculei e imprimi métricas de desempenho como acurácia, precisão, recall e F1-score.

## Etapa 05: Modelagem dos Dados - Random Forest

- **Montagem do grid search:** Configurei o grid search para encontrar os melhores hiperparâmetros do modelo Random Forest.
- **Treinamento do modelo:** Utilizei o método `.fit` para ajustar o modelo aos dados.
- **Tuning:** Realizei o tuning do modelo para otimizar sua performance com os melhores hiperparâmetros encontrados.
- **Realização da modelagem:** Executei o processo de modelagem com os dados ajustados.
- **Plotagem da matriz de confusão:** Gereia matriz de confusão para avaliar o desempenho do modelo.
- **Impressão das métricas:** Calculei e imprimi métricas de desempenho como acurácia, precisão, recall e F1-score.

Foi um desafio enriquecedor! Estou muito feliz com os resultados obtidos e animado para aplicar esses conhecimentos em futuros projetos. 🚀📊

