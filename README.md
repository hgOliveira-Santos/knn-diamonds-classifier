# Classificador de Qualidade de Diamantes com KNN

## Visão Geral

Este projeto aplica o algoritmo de K-Nearest Neighbors (KNN) para prever a categoria de corte de diamantes, utilizando um conjunto de dados popular extraído do pacote `ggplot2`. O objetivo principal é construir um pipeline simples, mas eficaz, de classificação supervisionada com foco em boas práticas de Machine Learning.

Além de servir como um estudo aplicado de KNN, o projeto demonstra etapas fundamentais como aquisição e pré-processamento de dados, escolha de hiperparâmetros com validação, e análise de desempenho com visualizações interpretáveis.

## Objetivos Técnicos

- Treinar um modelo de classificação com KNN para prever a variável `cut` com base em atributos numéricos dos diamantes.
- Determinar o valor ótimo de `k` com base em um conjunto de validação.
- Avaliar o desempenho do modelo com métricas adequadas.
- Interpretar os resultados com visualizações.

## Etapas do Projeto

1. Download do Dataset: O notebook automatiza a importação e o salvamento do dataset de diamantes.
2. Pré-processamento:
  - Filtragem de colunas relevantes (carat, depth, table, x, y, z).
  - Normalização das features numéricas.
  - Divisão em treino (60%), validação (20%) e teste (20%).
3. Treinamento e Validação:
  - Loop sobre k de 1 a 20 para encontrar o valor ótimo com base na acurácia do conjunto de validação.
  - Visualização da curva de desempenho por valor de k.
4. Teste Final:
  - Aplicação do modelo com melhor k no conjunto de teste.
  - Impressão da acurácia final e exibição da matriz de confusão.

## Resultados

- Melhor valor de k: 10
- Acurácia no conjunto de teste: 72.27%
- Matriz de confusão: Gerada para análise detalhada do desempenho por classe.

## Tecnologias e Ferramentas

- **Linguagem**: Python 3.x  
- **Bibliotecas**:
  - `pandas` e `numpy` (manipulação de dados)
  - `scikit-learn` (modelo KNN, validação, métricas, pré-processamento)
  - `matplotlib` (gráficos e visualizações)

## Estrutura do Projeto

├── dataset/
    └── diamonds.csv # Conjunto de dados original (baixado automaticamente)
├── knn_diamond_classifier.ipynb # Notebook principal com todo o pipeline
├── README.md # Este arquivo

