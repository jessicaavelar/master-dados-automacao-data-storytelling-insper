# Conceitos iniciais de Métodos em Inferência Causal

*Aula 01 da disciplina 13/10/2021*


### O que é inferêncial causal?

De forma resumida, é "provar" que a variável **x** causa **y** através de um modelo teórico.


### Distribuição de variável:

* Descreve quanto cada valor de uma variável ocorre;
  *  Por exemplo, a distribuição de uma moeda é 50% cara e 50% coroa.
* Há diferentes tipos de variáveis e diferentes maneiras de representá-las;
  * Categóricas ou ordinais: tabelas;
  * Contínuas: distribuições que não descrevem quanto a variável atinge determinado valor, mas a probabilidade de estar próxima de um valor;
    * Histogramas;
    * Densidade;
    * A probabilidade de estar em um intervalo é dado pela área abaixo da distribuição.

### Relação causal:

Para identificar uma relação causal, devemos remover a variação que possa existir por outros motivos além daquele que queremos identificar:

* Experimental.
* Model-based - regressão multivariada;
* Design-based.


## Exercício:

Utilizando os dados eleitorais, preparem os seguintes itens:

* Uma tabela com três variáveis e as seguintes colunas: variável, média, mediana, desvio-padrão, valor mínimo (min), valor máximo (max);
* Um histograma de uma variável contínua de alguma das bases;
* Uma tabela de distribuição de alguma variável discreta;
* Um gráfico de dispersão (scatterplot).

O notebook com o exercício completo é o arquivo "2021_10_20_eleicoes_rj_2020.ipynb" e [pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/inferencia_causal/01_conceitos_iniciais/2021_10_20_eleicoes_rj_2020.ipynb).
Os dados utilizados são do TSE e [estão disponíveis aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/tree/main/inferencia_causal/01_conceitos_iniciais/dados) em um arquivo .zip.
