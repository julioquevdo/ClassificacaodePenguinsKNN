# Projeto de Classificação de Pinguins com KNN

Este projeto explora o comportamento do modelo K-Nearest Neighbors (KNN) com dataframes de diferentes tamanhos, usando dois datasets contendo características físicas e as respectivas espécies de pinguins.

## Objetivo do Projeto

O objetivo deste projeto é avaliar como o KNN performa ao ser aplicado a datasets de tamanhos distintos. Exploramos a precisão e robustez do modelo em diferentes situações, incluindo a utilização de um dataset com aproximadamente 10 vezes mais dados.

## Estrutura do Projeto

- `data/`: Contém os datasets utilizados (não incluídos neste repositório por questões de direitos).
- `notebooks/`: Notebooks com análise exploratória e execução do modelo.
- `src/`: Código-fonte do projeto, incluindo scripts para pré-processamento e treino do modelo.

## Dataset

Utilizamos dois datasets de pinguins, contendo características como:
- Comprimento do Bico
- Profundidade do Bico
- Peso Corporal
- Espécie (rótulo de classe)

## Etapas do Projeto

1. **Pré-processamento dos Dados**: Remoção de dados nulos e padronização das variáveis numéricas para aumentar a performance do modelo KNN.
2. **Configuração do Modelo KNN**: Ajuste dos hiperparâmetros do KNN visando alcançar a melhor acurácia possível.
3. **Validação**: Avaliação do modelo com diferentes estratégias, incluindo:
   - Cross-validation
   - Holdout em dataset original
   - Holdout em dataset padronizado
   - Holdout com um dataset 10 vezes maior

## Visualizações dos Resultados

Abaixo estão espaços reservados para as visualizações geradas ao longo do projeto:

- **Matriz de Confusão (Cross-validation)**
  
- **Matriz de Confusão (Holdout)**
  
- **Gráficos de Linha de Aprendizado**
  
- **Matriz de Confusão (Holdout - Dataset Padronizado)**
  
- **Matriz de Confusão (Holdout - Dataset 10x Maior)**

## Resultados

A configuração do modelo KNN foi feita levando em consideração a acurácia, obtendo resultados variados conforme as estratégias e tamanhos de datasets utilizados.

Claro! Aqui está a seção "Como Executar o Projeto Localmente" em código Markdown:

## Como Executar o Projeto Localmente

### Usando Conda
1. Clone este repositório:
   ```bash
   git clone https://github.com/usuario/projeto-classificacao-pinguins-knn.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd projeto-classificacao-pinguins-knn
   ```
3. Crie o ambiente Conda a partir do arquivo `environment.yml`:
   ```bash
   conda env create -f environment.yml
   ```
4. Ative o ambiente:
   ```bash
   conda activate classificacao_pinguins_knn
   ```
5. Execute o notebook principal na pasta `notebooks/` para ver o fluxo de análise completa.

### Usando Pip
1. Clone este repositório:
   ```bash
   git clone https://github.com/usuario/projeto-classificacao-pinguins-knn.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd projeto-classificacao-pinguins-knn
   ```
3. Instale as dependências a partir do arquivo `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```
4. Execute o notebook principal na pasta `notebooks/` para ver o fluxo de análise completa.

## Bibliotecas Utilizadas
O projeto foi desenvolvido em Python e fez uso das seguintes bibliotecas:

~~~from sklearn.neighbors import KNeighborsClassifier
from sklearn.model_selection import cross_val_predict, train_test_split, learning_curve
from sklearn.metrics import confusion_matrix, classification_report, accuracy_score
from sklearn.preprocessing import StandardScaler
import pandas as pd
import plotly.express as px
import seaborn as sns
import numpy as np
~~~
