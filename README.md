# **Predição de Jogos do Campeonato Brasileiro de Futebol**

Este projeto utiliza técnicas de análise de dados e machine learning para tentar prever o máximo de  resultados de jogos do campeonato brasileiro de futebol com base em estatísticas das partidas e outros fatores.

---

## **Objetivo do Projeto**

O objetivo principal é estudar e aprender mais sobre os temas utilizado no projeto e demonstrar habilidades adiquiridas por mim durante a execução do projeto. Além disso, buscar construir um modelo que possa tentar prever o resultado de partidas (vitória do mandante, vitória do visitante ou empate) com o maior grau de acurácia possível, fornecendo insights úteis sobre os dados de um campeonato de futebol.

---

## **Estrutura do Projeto**

1. **Coleta e Pré-processamento de Dados**
   - **Fonte dos dados:** A fonte de dados foi adquirida no Kaggle[https://www.kaggle.com/] e está disponível pelo link: [https://www.kaggle.com/datasets/adaoduque/campeonato-brasileiro-de-futebol]
   - **Principais colunas:**
     - `mandante_stats`: Estatísticas do time mandante.
     - `visitante_stats`: Estatísticas do time visitante.
     - `resultado`: Resultado da partida (`Mandante`, `Visitante`, `Empate`).

2. **Análise Exploratória de Dados (EDA)**
   - Visualização de estatísticas das partidas.
   - Identificação de padrões e tendências nos dados.
   - Verificação de correlação entre variáveis.

3. **Pré-processamento**
   - Tratamento de valores ausentes.
   - Normalização das variáveis numéricas.
   - Codificação da variável alvo para classificação.

4. **Treinamento do Modelo**
   - **Modelos testados:**
     - XGBoost (principal)
     - Random Forest
     - Regressão Logística
   - **Técnicas de otimização:**
     - Ajuste de hiperparâmetros com `GridSearchCV`.
     - Balanceamento de classes com `SMOTE`.
     - Pesos dinâmicos para lidar com classes desbalanceadas.

5. **Avaliação**
   - **Métricas utilizadas:**
     - Acurácia
     - Matriz de Confusão
     - Relatório de Classificação (precision, recall, f1-score)
   - **Resultados do modelo final.**

---

## **Principais Ferramentas e Tecnologias**

- **Linguagem:** Python
- **Bibliotecas:**
  - **Pandas**: Manipulação de dados.
  - **Seaborn** e **Matplotlib**: Visualização de dados.
  - **Scikit-learn**: Modelagem e avaliação.
  - **XGBoost**: Modelo de machine learning.
  - **Imbalanced-learn**: Balanceamento de classes com SMOTE.
  - **Jupyter**: Criação de notebooks python.

---

## **Como Usar Este Projeto**

1. Clone o repositório:
   ```bash
   git clone [https://github.com/ThiagoYure/Data-Science-Brasileirao.git]
   cd Data-Science-Brasileirao
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Comece a usar.

---

## **Resultados Obtidos**

- **Melhor modelo:** Utilizando Voting Classifier com XGBoost, Random Forest e Regressão Logística.
- **Desempenho:**
  - Acurácia: **68%**.
  - **Relatório de Classificação:**
    | Classe     | Precision | Recall | F1-Score |
    |------------|-----------|--------|----------|
    | Mandante   | 0.62      | 0.66   | 0.64     |
    | Visitante  | 0.73      | 0.73   | 0.73     |
    | Empate     | 0.69      | 0.65   | 0.67     |

---

## **Melhorias Futuras**

1. Incluir mais dados, como condições climáticas, ou estatísticas detalhadas dos jogadores.
2. Testar outros algoritmos, como LightGBM ou Redes Neurais.
3. Implementar técnicas de feature engineering avançadas.

---

## **Contato**

- **Criado por:** [Thiago Yure]  
- **E-mail:** [thigoyure@gmail.com] 
- **Site:** [https://thiagoyure.vercel.app/]
- **Repositório do projeto:** [GitHub](https://github.com/ThiagoYure/Data-Science-Brasileirao)