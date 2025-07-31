# Projeto: Previsão de Sobreviventes do Titanic 🚢

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Status](https://img.shields.io/badge/status-conclu%C3%ADdo-green)
![License](https://img.shields.io/badge/license-MIT-green)

Este projeto foi desenvolvido para treinar meus conhecimentos em **Machine Learning** utilizando Python e algumas bibliotecas do ecossistema **Scikit-learn**.  
O desafio faz parte da competição [**Titanic: Machine Learning from Disaster**](https://www.kaggle.com/c/titanic) do Kaggle.

## 📊 Dados Utilizados

Os datasets `train.csv` e `test.csv` foram obtidos diretamente do Kaggle e contêm informações sobre os passageiros do Titanic, incluindo:

- `Pclass` — Classe do bilhete (1ª, 2ª, 3ª)
- `Sex` — Gênero
- `Age` — Idade
- `SibSp` — Nº de irmãos/cônjuges a bordo
- `Parch` — Nº de pais/filhos a bordo
- `Fare` — Tarifa paga
- `Embarked` — Porto de embarque (C, Q, S)
- **Variável-alvo:** `Survived` (1 = Sobreviveu, 0 = Não Sobreviveu)

## 🧠 Técnicas Utilizadas

- Imputação de valores faltantes em `Age` e `Fare`
- Codificação de variáveis categóricas (`Sex` e `Embarked`)
- Criação de feature combinada `Sex_Pclass` + dummies
- Divisão treino/validação com `train_test_split` e `cross_val_score`
- Ajuste de hiperparâmetros com `GridSearchCV`
- Modelo final: **RandomForestClassifier**

**Resultado da submissão no Kaggle:**  
- **Acurácia pública:** `0.77033`

## ⚙️ Como Rodar o Notebook

1. Clone o repositório:
   ```bash
   git clone https://github.com/moreiraDavi/kaggle-titanic.git
   cd kaggle-titanic
   ```

2. Crie um ambiente Python e instale as dependências:
   ```bash
   pip install pandas numpy scikit-learn matplotlib
   ```

3. Execute o notebook `kaggle-titanic.ipynb` para:
   - Treinar o modelo
   - Gerar o arquivo `submission.csv` para envio ao Kaggle

## 👤 Autor

Desenvolvido por **Davi Moreira**  
[🔗 GitHub](https://github.com/moreiraDavi) · [🔗 LinkedIn](https://linkedin.com/in/davi-moreira-631974289)
