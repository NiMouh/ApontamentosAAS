# Aula 2 - Detetor de SPAM

## Processo de desenvolvimento para detetor de SPAM?
 - Classificação binária (SPAM ou não SPAM).
 - Text mining
 - Modelo de Classificação
 - Algoritmo de otimização

## Text mining
É o processo de derivar informação relevante a partir de um texto.

### Processamento de linguagem natural (NLP)
Tem como propósito dar ao computador a capacidade de entender o texto, combinando sintaxe e semântica.

## Modelo de Classificação
É um modelo que classifica os dados em duas ou mais classes. O melhor modelo é aquele que tem a maior precisão e sensibilidade (pouca interseção entre estas duas métricas).

### Naive Bayes
É um modelo probabilístico que utiliza o teorema de Bayes para classificar os dados. É um modelo simples e rápido, que pode ser utilizado em problemas de classificação binária ou multiclasse.

### Logistic Regression
É um modelo de classificação que utiliza a regressão logística (técnica estatística) para classificar os dados. É um modelo simples e rápido, que pode ser utilizado em problemas de classificação binária ou multiclasse.

### Matriz confusão
É uma tabela que permite a visualização do desempenho de um algoritmo de classificação. Cada coluna representa as instâncias numa classe predita, enquanto cada linha representa as instâncias numa classe real (ou vice-versa). O nome deriva do fato de que ela facilita detetar se o sistema confunde duas classes (ou seja, se elas estão a ser confundidas por erro).

É definida como:
 - **True Positive (TP)**: é quando o modelo prevê que é SPAM e é SPAM.
 - **True Negative (TN)**: é quando o modelo prevê que não é SPAM e não é SPAM.
 - **False Positive (FP)**: é quando o modelo prevê que é SPAM e não é SPAM.
 - **False Negative (FN)**: é quando o modelo prevê que não é SPAM e é SPAM.

A **precisão** do modelo é dada por: (TP + TN) / (TP + TN + FP + FN).

A **sensibilidade** do modelo é dada por: TP / (TP + FN).


## Algoritmo de otimização
É um algoritmo que tenta encontrar o melhor valor para um determinado problema.

### Gradiente descendente
É um algoritmo de otimização iterativo que tenta encontrar o **mínimo** de uma função. O caminho é traçado pelo **learning rate** (taxa de aprendizagem), que define o tamanho do passo que o algoritmo dá em cada iteração, e pela **derivada** da função, que define a direção do passo.