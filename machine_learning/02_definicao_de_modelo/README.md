# Definição de modelo

*Aula 02 da disciplina de "Machine Learning Aplicada ao Jornalismo" 18/10/2021.*

Durante a aula foi aprendido a definição de modelo, frameworks de desenvolvimento e ferramentas que podem ser utilizadas. Além disso, fizemos um exemplo de modelo preditivo para eleição de vereadores.


#### Definição de modelo
"Trata-se de uma grande simplificação do que de fato ocorre na realidade, por basear-se em pressupostos nem sempre reais e por eliminar muitas das variáveis suscetíveis de mensuração".

Ou seja, um modelo é uma representação simplificada da realidade, onde pode ser feita através de uma expressão matemática e parâmetros do modelo pode ser estimados com dados do passado. Por definição, todos os modelos estão errados, mas alguns podem ser úteis.


#### Glossário básico

**Tipos de modelo** - O que quero prever? Classe, número, segmentação;

**Base de treino** - Dados do passado que usarei para encontrar padrões;

**Variável resposta** - O que quero prever;

**Variáveis explicativas** - Quais informações vou usar para ajudar a prever a variável resposta;

**Técnica** - Como usarei os dados do passado para encontrar padrões (regressão linear, random forest, rede neural);

**Valor predito** - Valor previsto pelo modelo;

**Erro** - Valor observado x Valor predito


#### CRISP-DM

![image](https://user-images.githubusercontent.com/89416633/138615538-459a4e91-3f88-48d8-b8c9-21aa66c7b56f.png)


*Na imagem o framework "CRISP-DM" da IBM. Ele é o mais conhecido e utilizado. Não é um dogma, mas pode ser visto como um gruia.*


### Prática da aula

Na parte prática da aula foi feito um modelo para prever a eleição de vereador em São Paulo.

Para isso, foi utilizado as [bases de dados do TSE](https://www.tse.jus.br/eleicoes/estatisticas/repositorio-de-dados-eleitorais-1) das eleições de 2020, também disponível na [pasta "Dados"](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/tree/main/machine_learning/02_definicao_de_modelo/dados).

Foi feita a transformação dos dados, separando as variáveis de interesse, limpando as bases e juntando-as. Além do treinamento do modelo e da previsão do modelo.

Esse é um modelo simples, utilizado para aprendizado, não sendo possível, de fato, prever eleição de vereador através dele. Porém, o objetivo é aprimorá-lo ao longo do curso.

O notebook completo está disponível no arquivo ["2021_10_18_vereadores_sp.ipynb"](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/machine_learning/02_definicao_de_modelo/2021_10_18_vereadores_sp.ipynb).

Como exercício, criei um modelo semelhante para a cidade de Belo Horizonte. O notebook completo está disponível no arquivo ["2021_10_18_vereadores_bh.ipynb"](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/machine_learning/02_definicao_de_modelo/2021_10_18_vereadores_bh.ipynb).
