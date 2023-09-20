# Aula 1 - Machine learning

## Objetivo
Agregar um determinado conjunto de dados, de modo a que possamos fazer decisões/previsões. Portanto no modo do ML resolver os problemas, a engenharia humana tem uma função crucial.

## Problemas a enfrentar
Estes são os **dois problemas** a enfrentar com ML:
- **estimativa**: por vezes, os dados podem ter algum noise, podendo afetar o resultado final obtido.
- **generalização**: pode ser dificil prever resultados de uma situação bastante improvável no nosso conjunto de dados.

## Caracterização dos problemas
Podemos caracterizar os problemas em seis categorias:
 - **Problemas de classe**: Qual é a natureza dos dados de treino e que tipos de consultas serão efetuadas na altura do teste?
 - **Assunções**: O que é sabemos sobre a fonte dos dados ou a forma da solução?
 - **Critérios de avaliação**: Qual é o objetivo do sistema de previsão ou de estimativa? Como serão avaliadas as respostas a consultas individuais? Como será medido o desempenho global do sistema?
 - **Tipo de modelo**: Será criado um modelo intermédio? Que aspetos dos dados serão modelados? Como o modelo será utilizado para fazer previsões?
 - **Classe de modelo**: Que classe paramétrica específica de modelos será utilizada? Que critério será utilizado para selecionar um modelo específico da classe de modelos?
 - **Algoritmo**: Que processo computacional será utilizado para ajustar o modelo aos dados e/ou para efetuar previsões?

## Supervised Learning
É quando a informação é dada em pares (x,y) onde x representa a entrada e o y uma possível saída. Ou seja, a aprendizagem está a ser supervisionada por nós pois estamos a controlar os dados que entram e a sua possível solução, para que possamos mais tarde fazer previsões.

Esta aprendizagem podem ser **dividida** em:
- **classificação**: As saídas são dadas através de um conjunto pequeno e finito.
- **regressão**: As saídas são dadas através de um conjunto grande finito ou um conjunto contínuo.

## Unsupervised Learning
Aqui a abordagem é diferente, pois não envolve encontrar uma solução através de um par (entrada,saída). Mas sim, recebe um conjunto de dados e geralmente é esperado ele encontrar alguns padrões ou estrutura nele.

Dentro da aprendizagem não-supervisionada temos **três tipos**:
- *density estimation*: é feita uma estimativa através do elemento do conjunto de dados anterior (tentar sempre prever a P(x(n+1)) para um conjunto de amostras x(1) até x(n)).
- *clustering*: agrupa automaticamente dados semelhantes sem usar rótulos, de modo a encontrar padrões e grupos naturais.
- *dimensionality reduction*: simplifica dados complexos, eliminando atributos redundantes ou pouco informativos, mantendo a essência dos dados.

## Reinforcement Learning
O objetivo é conseguir um mapeamento dos dados de entrada para os dados de saída, mas sem uma supervisão direta para especificar qual valor de saída seria o melhor. Não tem um conjunto de treino a priori, no entando o mesmo vai ganhando forma à medida que o agente interage com um ambiente.

Estes são os seguintes **passos**:
1. O agente observa o estado atual, x(0).
2. Seleciona uma ação, y(0).
3. Recebe uma recompensa, r(0) , que depende de x(0) e possivelmente de y(0).
4. O ambiente transita probabilisticamente para um novo estado, x(1) , com uma distribuição que depende apenas de x(0) e y(0).
5. O agente observa o estado atual, x(1).
6. (Processo repete-se).

Nota: Aqui as ações que o agente faz afetam tanto a **recompensa** (indicador que estamos a seguir o caminho certo) como a habilidade para **observar** (avaliar) o ambiente.

## Bias vs Variance
O **bias** é o erro que é introduzido devido a suposições simplificadas no algoritmo de aprendizagem. A **variância** é o erro que é introduzido devido à sensibilidade a pequenas flutuações no conjunto de treino.

Por exemplo num tiro ao alvo:
 - **high bias**: o alvo está longe do centro.
 - **high variance**: têm uma dispersão grande.
 - **low bias**: o alvo está no centro.
 - **low variance**: valores têm uma dispersão pequena.