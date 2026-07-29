# 🚢 Titanic - Projeto de Ciência de Dados

[![Kaggle](https://img.shields.io/badge/Kaggle-Titanic-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/c/titanic](https://www.kaggle.com/caiosantal))

> **Classificação de sobreviventes do naufrágio do Titanic** – um projeto completo de *machine learning* com análise exploratória, pré-processamento e comparação de modelos.


## 📖 Sobre o Projeto

O naufrágio do Titanic é um dos desastres marítimos mais famosos da história. Este projeto utiliza dados reais dos passageiros para construir um modelo preditivo capaz de classificar se um determinado passageiro sobreviveria ou não ao desastre.

O objetivo é aplicar todo o *pipeline* de Ciência de Dados: desde a formulação do problema, limpeza e análise dos dados, até a construção e avaliação de modelos de classificação, culminando em uma submissão para o *Kaggle*.

### 🎯 Objetivo

- Construir um classificador que preveja a sobrevivência de passageiros do Titanic.
- Comparar diferentes algoritmos (*Naive Bayes*, *Regressão Logística* e *k‑NN*).
- Gerar um *submission file* para o Kaggle e avaliar o desempenho.


## 📁 Estrutura do Projeto

O projeto está organizado nas seguintes etapas:

1. **Formulação do problema** – definição do objetivo e das métricas.
2. **Leitura e compreensão dos dados** – análise inicial das variáveis.
3. **Pré‑processamento**:
   - Remoção de colunas irrelevantes (`PassengerId`, `Name`, `Ticket`, `Cabin`).
   - Tratamento de valores nulos (imputação por média e moda).
   - *One‑hot encoding* para variáveis categóricas (`Sex`, `Embarked`).
   - Padronização dos dados com `StandardScaler`.
4. **Análise exploratória (EDA)** – visualizações e correlações para entender os padrões de sobrevivência.
5. **Modelagem** – treino e avaliação de três algoritmos:
   - `GaussianNB`
   - `LogisticRegression`
   - `KNeighborsClassifier` (com *GridSearchCV* para ajuste de hiperparâmetros).
6. **Submissão ao Kaggle** – geração do arquivo `.csv` com as predições.


## 🛠️ Pré‑requisitos e Instalação

Para executar o notebook localmente ou no Google Colab, você precisará das seguintes bibliotecas:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## 📂 Dados

1. Faça o download dos arquivos **`train.csv`** e **`test.csv`** disponíveis na página da competição no [Kaggle](https://www.kaggle.com/competitions/titanic/data).
2. Salve os arquivos em uma pasta no seu **Google Drive**.
* **Estrutura recomendada no Drive:** `dados/titanic/` (ficando no caminho `/content/drive/My Drive/dados/titanic/`).
3. **Atenção:** Se optar por salvar em um diretório diferente, lembre-se de atualizar os caminhos no notebook onde os arquivos são lidos e salvos:
* **Leitura dos dados:** `pd.read_csv(...)`
* **Exportação dos resultados:** `.to_csv(...)`

## 📊 Análise Exploratória
A análise inicial revelou informações importantes:

Gênero: mulheres tiveram uma taxa de sobrevivência de ~75%, enquanto homens ~25%.

Classe social: passageiros da 1ª classe sobreviveram em maior proporção; a maioria das mortes ocorreu na 3ª classe.

Idade: crianças (especialmente do sexo feminino) e jovens adultos tiveram maior chance de sobreviver.

Preço da passagem: quanto mais caro, maior a probabilidade de sobrevivência (correlacionado com a classe).

Porto de embarque: a maioria dos sobreviventes embarcou em Southampton (S)

## 🤖 Modelagem e Resultados
Os dados foram divididos em treino (891 registros) e teste (418 registros). Três algoritmos foram testados:

### 📊 Comparação de Desempenho dos Modelos

| Modelo | Acurácia (Treino) | Score Kaggle |
| :--- | :---: | :---: |
| Naive Bayes | 78,90% | 0.75358 |
| Regressão Logística | 80,02% | 0,76794 |
| k-NN (k=16, Euclidiana) | 83,61% | 0.75598 |

## 📌 Conclusão
Este projeto demonstra um fluxo de trabalho completo de Ciência de Dados:

Limpeza e preparação dos dados são etapas críticas para o sucesso do modelo.

A análise exploratória revelou padrões claros de sobrevivência, como a forte influência do gênero e da classe social.

A comparação de algoritmos mostrou que o k‑NN, com ajuste de hiperparâmetros, superou os demais modelos.

Apesar do resultado razoável, há espaço para melhorias, como:

Engenharia de features adicionais (ex.: extrair título do nome, criar variáveis de família).

Testar outros algoritmos (Random Forest, XGBoost).

Utilizar técnicas de balanceamento de classes.

## 👤 Autor
Caio Santos de Almeida

📧 caiosantal.cd@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/caiosantal/)
🐙 [GitHub](https://github.com/caiosantal)

