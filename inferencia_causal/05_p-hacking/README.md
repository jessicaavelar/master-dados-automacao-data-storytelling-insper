# Potential Outcomes e experimentos aleatórios

*Aula 05 da disciplina "Métodos em Inferência Causal" - 10/11/2021*


#### Viés:

Viés é como tratamento e controle são diferentes antes do tratamento, isto é, caso nenhum deles receba tratamento.

* Diferença entre E[ Y(0) | T=1 ] e E[ Y(0) | T=1];
* Ou seja, o grupo tratado já estava em um patamar maior e já deveríamos esperar que atingirem um resultado potencial maior, mesmo se não
recebessem tratamento.


#### Independência:

* Como unidades recebem tratamento ou controle é a característica mais importante para descobrir os efeitos de causas;
* E(Y) - o valor médio de Y(u) para todo u - é diferente de E(Y | S = t) - o valor médio de Y(u) para u que recebeu o tratamento;
* Para que os dois seja idênticos necessitamos de um mecanismo de atribuição de tratamento S que seja independente de outras variáveis.


#### PO (Padrão Ouro) na prática:

* Experimentos aleatórios são o padrão ouro;
* Designs quasi-experimentais são caracterizado em termos dos pressupostos nos quais a atribuição de tratamento (não aleatória) é tão boa quanto se tivesse sido aleatorizada;
    * Estudos observacionais baseados no pressuposto de “selection-on-observables”, o tratamento é tão bom quanto se tivesse sido aleatório depois de condicionado a variáveis observáveis;
    * Difference-in-difference designs comparam tratamento e controle onde a trajetória e características fixas no tempo podem ser removidas;
    * Em todos esses casos, tratamento e controle são definidos e, sob certas condições, podem ser comparados ao efeito tratamento médio em uma população de interesse bem definida.

#### Experimentos aleatórios:

Por que experimentos?

* Sob alocação aleatória (random assignment), não há viés de seleção;
* Isto porque o potential outcomes na condição controle - altos ou baixos - são aleatoriamente designados para condição controle e tratamento;
* Ou seja, E[ Y(0) | T = 1] = E[ Y(0) | T = 0] - o inverso também é válido;
    * A esperança do potential outcomes do grupo tratamento, caso não recebam tratamento, é igual ao que acontece no grupo controle.
* Na prática, alocação aleatória garante que características observáveis e não observáveis (incluindo resultados potenciais) seja estatisticamente o mesmo (para n grande);
* Além disso, experimentos podem ser reproduzidos.

#### P-hacking:

Manipulação de variáveis que leva ao resultado que esperamos, uma prática enganosa.

Manipula-se os dados para provar o nosso ponto e responder ao problema de pesquisa.


# Resultado

Como exercício de p-hacking, vamos utilizar os dados do artigo de Cesar Zucco (2013) para rodar um modelo ruim, errado, como exemplo do que não
fazer em uma pesquisa.

Queremos mostrar que o crescimento da população evangélica diminui a busca pelo bolsa família.

Primeiro tentaremos mostrar a relação entre os gastos do bolsa família e o crescimento da população envagélica.

Em seguida, acrescentaremos outras variáveis como controle do modelo para obter o resultado que estamos buscando.

A base de dados na pasta dados, [pode ser acessada aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/tree/main/inferencia_causal/05_p-hacking/dados),
e o dicionário dos dados [pode ser encontrado aqui](https://www.dropbox.com/s/anth1tqxwejqdr3/Replication%20Instructions.pdf?dl=0).

O notebook completo é o arquivo "2021_11_10_p-hacking.ipynb" e [pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/inferencia_causal/05_p-hacking/2021_11_10_p-hacking.ipynb).
