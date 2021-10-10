# Projeto Final de Pensamento Computacional

A pasta contém o trabalho final da disciplina de "Pensamento Computacional" do professor Álvaro Justen (Turicas), que consiste em criar um programa que executa um processo de ETL - Extract, Transform, Load. Essas 3 etapas são a base para programas que lidam com dados e são encontradas em diversos tipos de programas. O programa deve resolver um problema prático do dia a dia jornalístico.


### Contextualização

Durante apuração sobre o garimpo ilegal em território Yanomami para a disciplina de OSINT - grupo formado por Carina Dourado, Amanda Audi e eu, surgiu a necessidade de encontrar notícias específicas sobre as terras, porém os resultados do Google não satisfazia o que precisávamos.

Mas o site www.terrasindigenas.org.br faz um compilado de notícias sobre as terras indígenas, sendo possível filtrar de acordo com a etnia desejada. Os resultados do site vão ao encontro da necessidade do grupo.

Ainda assim, tínhamos um problema, pois eram 500 notícias e nem todas eram do nosso interesse. Precisávamos de textos que falassem sobre o Rio Uraricoera, uma das principais vias de acesso de garimpeiros às Terras Yanomamis.


### Objetivo

Acessar a URL que contém as notícias da [Terras Indígenas Yanomami](https://www.terrasindigenas.org.br/noticias/4016/TI/500/1), entrar em cada uma delas e verificar se cita o Rio Uraricoera, em caso afirmativo, salvar o link em um arquivo CSV.


### Metodologia

[O projeto](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/pensamento_computacional/projeto_final/noticias_indigenas-jessica_avelar.ipynb) é feito em Python e utiliza as bibliotecas CSV, Requests e BeautifulSoup4. Para o exemplo, utilizamos a Terra Indígena Yanomami, mas qualquer outra do site pode ser utilizada.

Para melhor leitura e com o objetivo de ser utilizado posteriormente, foi criado uma classe e quatro métodos que realiza as etapas de ETL:

`Class NoticiasIndigenas`

`baixar_html(self, site)` -> *A função baixa o HTML do site, deve-se passar a url de interesse*

`noticias_site(self)` -> *A função extrai todas as notícias do site, pode ser usada apenas esta função*

`noticias_especificar(self, palavra)` -> *A função extrai apenas as notícias que contêm a palavra definida, deve-se passar a palavra de interesse*

`escreve_csv` -> *A função salva os links em um arquivo CSV (Data, Título e Link), deve-se passar o nome do arquivo*


# Resultado

Foi criado um código em que é possível extrair as notícias de qualquer uma das Terras Indígenas listadas no site, também é possível fazer a pesquisa que desejar dentro das notícias.

O arquivo final tem o nome "uraricoera_yanomami" e [pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/pensamento_computacional/projeto_final/uraricoera_yanomami.csv).
