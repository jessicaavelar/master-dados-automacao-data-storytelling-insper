# Corpus Textuais

*Aula 01 da disciplina de Mineração e análise de dados de redes, textos e imagens - 14/10/2021*


#### Corpus textuais

“Um corpo de material linguístico que existe em formato eletrônico e que pode ser processado por computador para vários propósitos” (Leech, 1997, p.1).

“Uma coletânea grande e criteriosa de textos naturais” (Biber et. al, 1998, p.4).

Em resumo é uma coleção de textos de livros, gravações telefônicas, tweets…


#### Mineração de texto

Mineração de texto (text mining, text processing, text analytics) pode ser definida como um processo de extração de informações desconhecidas e úteis de documentos textuais
escritos em linguagem natural.

**Processo:**

Esse é um processo padrão, mas pode ter mais etapas (esse é o comum):

* Coleta de documentos;
* Pré-processamento;
* Extração de conhecimento;
* Avaliação e interpretação dos resultados.


**Coleta de documento**

* Objetivos: conseguir documentos relacionados ao tipo de conhecimento que se deseja obter;
* Pode-se utilizar de várias fontes, como livros, emails, redes sociais, fóruns de internet, discursos, etc;
* O conhecimento de mundo e de especialistas não são utilizados pois os algoritmos de agrupamento dos documentos aprende de forma não supervisionada como extrair o conhecimento dos textos, e desta maneira, categorizar os documentos de forma a facilitar os próximos passos do processo de mineração de textos.
* A lematização é a fixação dos lemas, ou seja, da forma canônica de um signo linguístico. É importante para a classificação das formas linguísticas. Por exemplo: as formas flexionadas dos verbos são apresentadas no infinitivo, assim como os adjetivos no masculino singular. Desta maneira, a busca de uma dada lexia acontece nos textos do corpus segundo uma forma canônica.


## Resultado

A primeira prática teve o objetivo de coletar dados do Twitter utilizando a biblioteca [Twint](https://github.com/twintproject/twint).

Coletamos 500 tweets com a hashtag "#BrequeDosApps'.

O notebook completo é o arquivo "2021_10_14_coleta_dados_breque.ipynb", o [arquivo pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/minera%C3%A7%C3%A3o_analise_de_dados/01_corpus_textuais/2021_10_14_coleta_dados_breque.ipynb).

O csv com os tweets coletados é o arquivo "breque.csv", o [arquivo pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/minera%C3%A7%C3%A3o_analise_de_dados/01_corpus_textuais/breque.csv).

Além disso, montamos uma nuvem de palavras:

![breque](https://user-images.githubusercontent.com/89416633/141858210-1541e2dc-4c59-441c-862f-884a0e2c8dfb.png)


## Exercício

O exercício era fazer algo semelhante à prática da aula, porém com um assunto de interesse.

Para tanto, coletei 2000 tweets com as palavras "vacinação", "pandemia", "vacinacao".

o notebook completo é o arquivo "2021_10_14_vacina.ipynb", o [arquivo pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/minera%C3%A7%C3%A3o_analise_de_dados/01_corpus_textuais/2021_10_14_vacina.ipynb).

O csv com os tweets coletados é o arquivo "vacinacao.csv", o [arquivo pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/minera%C3%A7%C3%A3o_analise_de_dados/01_corpus_textuais/vacinacao.csv).

A nuvem de palavras geradas foi:

![vacina](https://user-images.githubusercontent.com/89416633/141858503-72f04d0c-03ea-4531-923e-ab5c742b63d0.png)
