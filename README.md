# titanic-kaggle-machine-learning
Leitura dos dados, Limpeza, Tratamento de Nulos, Normalização, Análise Descritiva (EDA) e Classificação comparativa com Naive Bayes, Regressão Logística e KNN.
# 🚢 Titanic - Projeto de Ciência de Dados

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Kaggle](https://img.shields.io/badge/Kaggle-Titanic-20BEFF)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

> **Classificação de sobreviventes do naufrágio do Titanic** – um projeto completo de *machine learning* com análise exploratória, pré-processamento e comparação de modelos.

---

## 📖 Sobre o Projeto

O naufrágio do Titanic é um dos desastres marítimos mais famosos da história. Este projeto utiliza dados reais dos passageiros para construir um modelo preditivo capaz de classificar se um determinado passageiro sobreviveria ou não ao desastre.

O objetivo é aplicar todo o *pipeline* de Ciência de Dados: desde a formulação do problema, limpeza e análise dos dados, até a construção e avaliação de modelos de classificação, culminando em uma submissão para o *Kaggle*.

### 🎯 Objetivo

- Construir um classificador que preveja a sobrevivência de passageiros do Titanic.
- Comparar diferentes algoritmos (*Naive Bayes*, *Regressão Logística* e *k‑NN*).
- Gerar um *submission file* para o Kaggle e avaliar o desempenho.

---

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

---

## 🛠️ Pré‑requisitos e Instalação

Para executar o notebook localmente ou no Google Colab, você precisará das seguintes bibliotecas:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Instale‑as com:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
