# Breast-Cancer-Prediction
Este projeto utiliza aprendizado de máquina para construir modelos preditivos que detectam o câncer de mama a partir de dados de RNA sequencial fornecidos pelo **The Cancer Genome Atlas Program (TCGA)**. A análise inclui pipelines de pré-processamento e avaliação de modelos com diferentes abordagens de classificação.

## 📂 Estrutura do Projeto

- **Data**: O dataset utilizado é o `brca_mirnaseq.csv`, contendo informações sobre o RNA sequencial e a classe (benigno ou maligno).
- **Objetivo**: Desenvolver modelos preditivos robustos e avaliar seu desempenho na tarefa de classificação binária.

## 🚀 Técnicas e Ferramentas Utilizadas

O projeto explora as seguintes ferramentas do Python para a criação e avaliação de modelos:

- **Bibliotecas principais**:
  - `pandas` e `numpy`: Manipulação e análise de dados.
  - `matplotlib` e `seaborn`: Visualização de dados.
  - `scikit-learn`: Criação de modelos, pré-processamento e avaliação.
- **Técnicas aplicadas**:
  - Pré-processamento com `StandardScaler` e `MinMaxScaler`.
  - Seleção de features com `SelectKBest` e o teste qui-quadrado (`chi2`).
  - Redução de dimensionalidade com **Análise de Componentes Principais (PCA)**.
  - Algoritmos testados:
    - Regressão Logística (`LogisticRegression`).
    - K-Nearest Neighbors (`KNeighborsClassifier`).

## 📊 Avaliação dos Modelos

Os modelos foram avaliados utilizando validação cruzada com métricas de precisão balanceada (`balanced_accuracy_score`). O desempenho dos diferentes pipelines foi comparado utilizando boxplots, gráficos de swarm e violinos.

Resultados destacados:
- **Pipeline com PCA e Regressão Logística**: Obteve um desempenho balanceado de **0.972** no conjunto de teste.

## 🧩 Visualizações Adicionais

- Matrizes de confusão foram geradas para os modelos finais, com e sem normalização, para identificar erros de classificação, como falsos positivos e falsos negativos.

## 🛠️ Como Executar

1. **Pré-requisitos**:
   Certifique-se de ter instalado o Python e as dependências listadas abaixo:
   - `pandas`
   - `numpy`
   - `seaborn`
   - `matplotlib`
   - `scikit-learn`

2. **Executar o script**:
   - Baixe o arquivo `brca_mirnaseq.csv` na mesma pasta do script.
   - Execute o código em um ambiente Python ou Jupyter Notebook.

3. **Resultados**:
   Os resultados incluem métricas de desempenho, visualizações de métricas e o pipeline final ajustado.

## 📁 Código

O código completo deste projeto está disponível no [repositório GitHub](https://github.com/suzanalop/Breast-Cancer-Prediction).
