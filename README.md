# **Melody Metrics: Decoding Song Popularity**
Este projeto visa explorar e predizer a popularidade das músicas utilizando o conjunto de dados "Melody Metrics". Por meio da aplicação de técnicas de machine learning, analisaremos a interação entre diversos atributos de uma música e sua influência no sucesso comercial. Além disso, existirá uma etapa de Exploratory Data Analysis (EDA), que visa explorar as características dos dados e melhorar o compreensão sobre a base.

### **Relatório Final**
Este relatório detalha o processo e os resultados de uma análise de dados e modelagem preditiva realizada em um conjunto de dados de música. O objetivo era entender os fatores que influenciam a popularidade das músicas e desenvolver modelos preditivos para estimar essa popularidade.

##### **Metodologia**
O projeto seguiu um fluxo de trabalho estruturado em ciência de dados:
- Análise Exploratória de Dados (EDA): Compreensão das características fundamentais dos dados.
- Testes de Hipótese: Verificação de suposições estatísticas.
- Modelagem Preditiva: Construção e avaliação de modelos de machine learning.

##### **Ferramentas Utilizadas**
Seguiu-se a linguagem de programação Python, que normalmente é usada em problemas de Ciência de Dados. Algumas bibliotecas como Pandas, Seaborn, Matplot, scikit-learn foram utilizadas para ajudar no desenvolvimento do projeto. Os algoritmos utilizados foram XGBoost, RandomForestRegressor, LightGBM, e LinearRegression.

##### **Características do Dataset**
O dataset inclui Características de músicas, incluindo comprimento, número de instrumentos, gênero, tempo, conteúdo lírico, ano de lançamento e popularidade. As descobertas iniciais feitas foram a análise de distribuições, médias, desvios padrão e relações entre variáveis. Identificação de padrões e outliers.

##### **Insights Principai do Dataset**
- Distribuição de Popularidade: Variou amplamente, sugerindo uma relação não linear com outras características.
- Relações de Gênero e Ano de Lançamento: Investigação da evolução da popularidade ao longo do tempo e entre diferentes gêneros.

##### **Teste de Hipótese**
- Objetivo
    - Impacto do Gênero na Popularidade: Análise de variância (ANOVA) para comparar a popularidade entre diferentes gêneros musicais.
    - Influência do Conteúdo Lírico: Teste t para avaliar se o conteúdo lírico afeta significativamente a popularidade.
- Resultados
    - Diferenças Significativas: Encontradas entre gêneros, e um impacto substancial do conteúdo lírico na popularidade.

##### **Modelagem Preditiva**
A escolha dos modelos visou abranger diferentes técnicas de aprendizado (árvores, boosting, linear) para capturar uma gama mais ampla de padrões nos dados.

##### **Modelos Utilizados**
- RandomForestRegressor: Escolhido por sua capacidade de lidar com relações não lineares e robustez a overfitting.
- XGBoostRegressor: Devido à sua eficiência e alta performance em competições de dados.
- LightGBM: Por sua rapidez e eficiência em grandes conjuntos de dados.
- LinearRegression: Como modelo meta no ensemble para combinar as previsões dos modelos base.

##### **Ensemble de Stacking**
Utilização do stacking para combinar as previsões dos modelos individuais, buscando um equilíbrio entre viés e variância e melhorar a precisão geral.

##### **Avaliação dos Modelos**
- Métricas Utilizadas: R2, MAE, MedAE, RMSE para avaliar e comparar o desempenho dos modelos.
- Desempenho do Ensemble: Superior aos modelos individuais, indicando a eficácia da abordagem de stacking.

##### **Resultados**
- RandomForestRegressor
    - R2 Score (Validação): 0.9374
- XGBoost
    - R2 Score (Validação): 0.9367
- LightGBM
    - R2 Score (Validação): 0.9352
- Ensemble Stacking
    - R2 Score (Validação): 0.9393

##### **Conclusões**
- Importância da Análise Exploratória: Fundamental para orientar as etapas subsequentes de modelagem.
- Eficiência do Ensemble: Comprovada pela melhoria nas métricas de desempenho.
- Impacto do Conteúdo Lírico e Gênero: Fatores significativos na popularidade das músicas.
- Aplicações Práticas: Os modelos podem ser aplicados para prever tendências no mercado musical e orientar decisões de marketing.
- Futuras Pesquisas: Investigação de outras características musicais e sua relação com a popularidade.
