# Variáveis e Tipos

*Aula 02 da disciplina "Pensamento Computacional" 13/08/2021*


Durante a aula foi aprendido os conceitos de variáveis, formas de utilizá-las e boas práticas.

Os **nomes das variáveis** possuem regras:

*   Devem começar com letras ou "_";
*   Podem conter letras (inclusive "especiais", com acentos), números e "_";
*   Não podem conter espaços, nem outros caracteres, como "-", "(".


#### Tipos

Alguns tipos em Python:

`str`

`int`

`float`...

A função `type` nos ajuda a identificar o tipo dos valores que passamos para el.


#### Concatenando variáveis com texto literal

As formas de utilizar número e strings em uma frase. Exemplo:

```python
print(f"Você deve ter {possivel_idade} anos")
```


#### Cálculo da média

Exercício em sala:
* Peça ao usuário dois número inteiros de 0 a 10 e armazene-os em uma variável;
* Calcule a média e armazene-a em uma variável;
* Mostre na tela o resultado.


#### Condições

A estrutura `if`, `else` e `elif`. Quando e como utilizar as condições em um programa.

```python
if condição:
  comando_caso_condição_seja_verdadeira
else:
  comando_caso_condição_seja_falsa
```

Podemos utilizar diversos operadoers em nossas condições, tais como:

* `a > b`: verifica se `a` é **maior** que `b`;
* `a >= b`: verifica se `a` é **maior ou igual** a `b`;
* `a < b`: verifica se `a` é **menor** que `b`;
* `a <= b`: verifica se `a` é **menor ou igual** a `b`;
* `a == b`: verifica se `a` é **igual** a `b`;
  * `=` é um **operador de atribuição**, enquanto que `==` **verifica a igualdade**;
* `a != b`; verifica se `a` é **diferente** de `b`.

Podemos também compor as condições utilizando os operadores `and` e `or`, mas atente-se: `and` sempre terá precedência sobre `or`, ou seja, na expressão `x or y and z` primeiro será compultado `y and z` (vamos chamar de "resultado1") para depois computar `x or resultado1`. Além disso, podemo **negar** uma condição com not, exemplos:

* `not a == b` é o equivalente a `a != b`;
* `not a > b` é o equivalente a `a <= b`.



## Resultado

O notebook completo é o arquivo "2021_08_03_variaveis_e_tipos.ypynb" e [pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/pensamento_computacional/02_variaveis_e_tipos/2021_08_13_variaveis_e_tipos.ipynb).


## Exercício

* Elabore 5 perguntas com 4 possíveis opções cada;
* Crie um programa que, para cada pergunta:
  * Exibe a pergunta;
  * Exibe as opções;
  * Pergunta qual a resposta correta.
* Ao final, exibe a pontuação (0 a 5);

O notebook com o exercício completo é o arquivo "exercicio_quiz.ipynb" e [pode ser acessado aqui](https://github.com/jessicaavelar/master-dados-automacao-data-storytelling-insper/blob/main/pensamento_computacional/02_variaveis_e_tipos/exercicio_quiz.ipynb).

O resultado é um quiz sobre a COVID-19.
