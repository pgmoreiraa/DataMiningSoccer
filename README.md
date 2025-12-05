# ⚽ Análise de Padrões Táticos no Futebol Europeu
### Mineração de Dados & Inteligência Competitiva no Esporte

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)

</div>

---

## 📖 Sobre o Projeto

Este projeto foi desenvolvido como requisito avaliativo da disciplina de **Mineração de Dados**, no 2º Semestre do curso de **Inteligência Artificial** da **Fatec Rio Claro**.

O objetivo principal foi aplicar técnicas avançadas de **Data Mining (Mineração de Dados)** para transformar dados brutos de partidas de futebol em inteligência tática. Através de algoritmos de aprendizado de máquina não supervisionado e supervisionado, buscamos eliminar a subjetividade da análise esportiva, identificando matematicamente o "segredo da vitória" e os padrões que diferenciam times campeões de times rebaixados.

## 📊 Base de Dados

Utilizamos o **European Soccer Database**, criado por Hugo Mathien. É uma das bases mais completas de futebol europeu, contendo dados de:
* +25.000 partidas
* 10.000 jogadores
* 11 Ligas Europeias
* Atributos detalhados de jogadores e times (via série FIFA)

🔗 **Fonte:** [Kaggle - European Soccer Database](https://www.kaggle.com/datasets/hugomathien/soccer)

---

## 🛠️ Metodologia e Técnicas Aplicadas

O projeto seguiu um pipeline robusto de Ciência de Dados:

### 1. Clusterização (Definição de Estilos)
Utilizamos o algoritmo **K-Medoids** para agrupar os times baseados em seus atributos táticos (velocidade, passe, pressão, agressividade). Identificamos **4 Estilos de Jogo** distintos:
* **Cluster 1:** Jogo Lento / Baixa Pressão (Menor eficiência).
* **Cluster 2:** Alta Intensidade e Pressão (Maior saldo de gols médio).
* **Cluster 3:** Jogo Cadenciado / Posse de Bola.
* **Cluster 4:** Ataque Direto Desorganizado (Estilo mais comum e vulnerável).

### 2. Classificação (Predição)
Treinamos modelos de Machine Learning para prever automaticamente o estilo tático de um time com base em suas estatísticas.
* **Melhor Modelo:** SVM (Support Vector Machine).
* **Acurácia:** **95.6%** na identificação do perfil tático.

### 3. Regras de Associação (O Segredo da Vitória)
Aplicamos o algoritmo **Apriori** para encontrar padrões ocultos ("Se X acontece, então Y acontece").
* *Insight Chave:* A **Velocidade de Construção** (*BuildUp Play Speed*) tem uma correlação mais forte com a vitória do que a simples posse de bola ou troca de passes curtos.

---

## 🚀 Principais Resultados

A análise provou que a mineração de dados é essencial para a tomada de decisão moderna no esporte. Destaques:

1.  **Objetividade:** Conseguimos classificar times rivais (ex: Real Madrid e Barcelona) em clusters opostos baseados apenas em dados, validando a precisão do modelo.
2.  **Eficiência Tática:** O estilo de "Alta Intensidade" (Cluster 2) apresentou um saldo de gols médio de **+0.18** por partida, superior a todos os outros estilos.
3.  **Ferramenta Preditiva:** O sistema desenvolvido pode ser utilizado por analistas de desempenho para diagnosticar rapidamente o estilo de jogo de um próximo adversário.

---

## 🧰 Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Manipulação de Dados:** Pandas, NumPy, SQLite
* **Visualização:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn (SVM, Random Forest, KNN, Naive Bayes)
* **Clusterização:** Scikit-learn-extra (K-Medoids)
* **Regras de Associação:** MLxtend (Apriori)

---

## 👨‍💻 Autores

Equipe responsável pelo desenvolvimento e análise:

* **Marvin Cristhian Gomes Pinto**
* **Paulo Guilherme Moreira**
* **Raphael Culim Neves**

---

<div align="center">
  <small>Projeto acadêmico - Fatec Rio Claro - 2025</small>
</div>
