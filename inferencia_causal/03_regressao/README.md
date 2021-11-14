#  Análise de regressão

*Aula 03 da disciplina "Métodos em Inferência Causal" - 27/10/2021*

#### Distribuição normal:

* Como sabemos, a distribuição de gasto de campanha (e o histograma) é bastante variado;
* Entretanto¹, se a gente a gente estimar a média de gasto de diversas populações diversas vezes, a distribuição das médias irá se aproximar da distribuição normal;
* E se a gente (fazer a normalização da variável):
    * Pegar a média;
    * Subtrair de todos os valores coletado;
    * Dividir tudo pelo desvio-padrão;
    * Construiremos uma distribuição normal centrada no zero

*¹ Através do teorema do limite central.*

* É a distribuição de uma variável dado o valor de outra variável;
  *  Por exemplo, a probabilidade de um feto ser XX e aproximadamente 50%;
  * Entretanto, a probabilidade de ser XX se o nome é Josefina é maior que 0,5.

#### Teorema de Bayes:

Se um teste (digamos um mamograma) identifica um nódulo cancerígeno 99% das vezes e um teste volta positivo, qual é a probabilidade da pessoa que fez o teste ter de fato um nódulo cancerígeno?

**A resposta não é 99%.**


#### Média condicional:

* Dado um certo valor x, qual é a média esperada de y?
    * Dado o valor de gastos de campanha, qual o número esperado de votos?
* Se a média de y é maior dado um valor maior de x, as duas variáveis estão relacionadas positivamente;
* Podemos ir mais adiante e calcular as médias condicionais de y para todos os valores de x;
    * Se x for discreta (ou categórica), a nossa vida fica mais fácil.

#### Como colocar uma reta em um gráfico de dispersão?

* Vamos supor que a relação entre x e y é linear;
* Por exemplo, y = 20 + 3x;
* Com essa regressão saberemos o valor médio de y para qualquer valor de x;
* Se a inclinação é positiva, sabemos que y varia proporcionalmente em relação a x. Se negativa, então será uma relação inversa.


#### Mínimos quadrados ordinários (ordinary least squares):

* É a maneira mais utilizada para estimar uma linha de regressão;
* OLS nos dá a linha com a menor soma dos quadrados dos resíduos. Em outras palavras, minimiza os erros.


#### Controlando por uma variável:

* Uma das vantagens da regressão é que você pode controlar as variações de x e y condicional a uma outra variável z;
* Y pode estar relacionado a diversos outros fatores além de x;
* A regressão nos dá a média condicional de y dado um valor de x. A diferença entre x observado e y é o resíduo;
* Este resíduo nos informa o quanto não sabemos de y;
* Se x relacionado a esses fatores também, controlando por outros fatores nos permite encontrar a relação entre x e y, sem nos preocupar com a variável z.


*OBS: a quantidade de variáveis que você utilizará para um modelo depende da quantidade de observações que você tem. Nunca utilizar um número maior de variáveis do que de observações, porque matematicamente é impossível estimar um modelo assim.

A quantidade de observações também diminui a variância. Quanto mais observações, melhor.*


# Resultado:

Como exercício feito em aula, utilizamos a base de dados de candidatos e de gastos de prefeitos em 2020, os [dados estão disponíveis aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/tree/main/inferencia_causal/03_regressao/dados).

O notebook completo é o arquivo "2021_10_27_regressao.ipynb" e [pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/inferencia_causal/03_regressao/2021_10_27_regressao.ipynb).
