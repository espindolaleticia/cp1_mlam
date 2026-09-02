# Checkpoint 01 — Classificação de Dados

## 1. Objetivo do projeto

Este projeto tem como objetivo aplicar técnicas de análise exploratória e classificação de dados utilizando Python e aprendizado de máquina. Foram analisados conjuntos de dados relacionados aos temas **Adult Census Income** e **Parkinsons**, com o objetivo de compreender os dados, identificar padrões e testar algoritmos de classificação.

## 2. Integrantes

* Felipe Mitsuo — RM570692
* Laura Godoy Callegari — RM569181
* Letícia Araújo Espindola — RM569308
* Mariana Dreset Carbollan — RM569207
* Milena de Aguiar Lopes Cardoso — RM570599

**Turma:** 1CCPJ
**Data:** 02/09/2026

## 3. Tema e datasets escolhidos

### Exercício 2 — Adult Census Income

O tema escolhido foi **Adult Census Income**, um conjunto de dados baseado em informações do censo dos Estados Unidos.

**Dataset:** Adult Census Income

**Fonte:** https://www.kaggle.com/datasets/uciml/adult-census-income

### Exercício 3 — Parkinsons

O tema escolhido foi **Parkinsons**, um conjunto de dados relacionado à identificação de características associadas à doença de Parkinson por meio de medidas obtidas a partir da voz.

**Dataset:** Parkinsons

**Fonte:** https://archive.ics.uci.edu/dataset/174/parkinsons

## 4. Variável-alvo

A variável-alvo é a informação que será utilizada pelos modelos para realizar a classificação.

No dataset **Parkinsons**, a variável-alvo é **status**, que indica a classe de cada registro:

* `1` — pessoa com Parkinson;
* `0` — pessoa sem Parkinson.

## 5. Etapas realizadas

Durante a implementação, foram realizadas as seguintes etapas:

1. Importação das bibliotecas necessárias.
2. Carregamento dos datasets.
3. Verificação da quantidade de linhas e colunas.
4. Visualização de amostras dos dados.
5. Verificação dos tipos de dados.
6. Identificação e análise de valores ausentes.
7. Análise exploratória dos dados.
8. Identificação da variável-alvo.
9. Separação dos dados em treinamento e teste.
10. Treinamento dos modelos de classificação.
11. Realização das previsões.
12. Avaliação dos resultados por meio da acurácia e da matriz de confusão.
13. Comparação do desempenho dos modelos.

## 6. Algoritmos utilizados

Foram utilizados dois algoritmos de classificação:

* **Regressão Logística**
* **K-Nearest Neighbors (KNN)**, utilizando `k = 5`.

Os dois modelos foram treinados e avaliados utilizando o mesmo conjunto de treinamento e teste.

## 7. Principais resultados

O dataset Parkinsons possui **195 registros** e apresentou predominância da classe Parkinson.

Durante a análise exploratória, algumas características acústicas, como **PPE, frequência vocal e HNR**, apresentaram diferenças entre as classes. Entretanto, também foi observada sobreposição entre os valores.

Nos testes realizados:

| Modelo              | Acurácia |
| ------------------- | -------: |
| Regressão Logística |    92,3% |
| KNN (k=5)           |    92,3% |

Os dois modelos apresentaram o mesmo desempenho no conjunto de teste neste experimento.

A matriz de confusão também foi utilizada para observar os acertos e erros de cada classe, permitindo identificar falsos positivos e falsos negativos.

## 8. Limitações

Entre as principais limitações encontradas estão:

* número reduzido de participantes;
* desbalanceamento entre as classes;
* utilização de uma única divisão entre treinamento e teste;
* existência de várias gravações pertencentes às mesmas pessoas, o que pode afetar a avaliação da generalização dos modelos.

## 9. Como executar o notebook

Para executar o projeto:

1. Abra o notebook no **Google Colab** ou em um ambiente compatível com Jupyter Notebook.
2. Faça o download ou disponibilize os datasets utilizados.
3. Execute as células do notebook na ordem apresentada.
4. Instale as bibliotecas necessárias, caso sejam solicitadas.
5. Execute as etapas de análise exploratória, treinamento e avaliação dos modelos.
6. Observe os resultados apresentados nas tabelas, gráficos e métricas de avaliação.

## 10. Conclusão

A análise realizada mostrou que os modelos de Regressão Logística e KNN apresentaram bom desempenho neste experimento, ambos alcançando **92,3% de acurácia** no conjunto de teste.

A análise exploratória também mostrou diferenças em algumas características acústicas entre as classes, embora exista sobreposição entre os valores.

Apesar dos resultados positivos, as limitações do dataset e da metodologia utilizada devem ser consideradas. Os resultados não são suficientes para afirmar que os modelos garantem uma classificação correta em novos casos ou que podem substituir uma avaliação clínica.

Como melhorias futuras, poderiam ser utilizadas técnicas como validação cruzada, separação dos dados por participante, outras métricas de avaliação e diferentes algoritmos e configurações.
