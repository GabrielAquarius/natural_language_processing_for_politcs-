# Análise de Dados e Predição do Posicionamento Político

Este é um projeto de análise de dados que utiliza dados coletados de duas figuras políticas proeminentes no Brasil, Lula e Bolsonaro, a partir de suas respectivas contas no Twitter. O objetivo principal é realizar uma análise exploratória desses dados, realizar um pré-processamento para prepará-los para modelagem, e então, treinar modelos de machine learning para prever o posicionamento político dessas figuras com base em métricas como contagem de retweets, contagem de favoritos e data dos tweets.

## Bibliotecas Principais Utilizadas

- Pandas (pd)
- NumPy (np)
- Matplotlib (plt)
- Seaborn (sns)
- Plotly (go)
- Scikit-learn (confusion_matrix, LabelEncoder, StandardScaler, OneHotEncoder, train_test_split, cross_val_score, GridSearchCV, LinearRegression, LogisticRegression, DecisionTreeRegressor, RandomForestRegressor)
- Spacy (spacy, Doc)
- String
- Emoji

## Etapas do Projeto

1. **Carregamento dos Dados**: Os dados foram carregados a partir de arquivos JSON contendo os tweets de Lula e Bolsonaro.

2. **Pré-Processamento dos Dados**:
   - Tratamento de dados temporais, incluindo a mudança de formato de data e ordenação cronológica dos tweets.
   - Tratamento de dados numéricos, incluindo a extração de valores e exclusão de colunas irrelevantes.
   - Tratamento de outliers através da função `remover_outliers`.
   
3. **Análise de Marcos Temporais**: Realizada para entender padrões de atividade temporal nos tweets.

4. **Predição do Posicionamento Político**:
   - Proporcionalização dos dados e criação dos rótulos para treinamento.
   - Utilização de palavras-chave para atribuir um posicionamento político (esquerda, direita ou neutro) aos tweets.
   - Separação dos dados em conjuntos de treino e teste.
   - Treinamento de modelos de Regressão Linear, Regressão Logística, Árvore de Decisão e Random Forest Regressor.
   
5. **Avaliação dos Modelos**:
   - Utilização de métricas como Mean Squared Error (MSE) e R² para avaliação da performance dos modelos.

## Execução do Código

O código foi executado em um ambiente Python, utilizando as bibliotecas mencionadas. Recomenda-se instalar as bibliotecas listadas no ambiente de execução antes de rodar o código.

## Arquivos de Dados

Os arquivos de dados utilizados foram:
- `LulaOficial.json`
- `jairbolsonaro.json`

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou uma issue para propor melhorias, correções ou novas funcionalidades.

## Licença

Este projeto é licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).
