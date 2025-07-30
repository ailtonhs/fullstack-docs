# Usando Condições

## Condições

Para tomar decisões mais inteligentes em nossos programas, precisamos de declarações **if** que dependam de condições mais inteligentes. como no aplicativo de pergutas e respostas.

Um programa como esse usa o operador **===** para verificar se a **answer** de um participante em um quiz de perguntas e respostas está correta.

```js
let answer = "Picasso";

if (answer === "Picasso") {
    console.log(answer + " is correct!");
}
```
E se a resposta do quiz de curiosidades não estiver correta? Podemos usar **!==** para verificar se **answer** não é igual a **"Picasso"**.

```js
let answer = "matisse";
if (answer !== "Picasso") {
    console.log(answer + " is wrong!");
}
```

As declarações **if** funcionam com todos os operadores de comparação que exploramos até agora. Como verificar se **age** é maior ou igual a **55**.

```js
let age = 75;
if (age >= 55) {
    console.log("Discount applied");
}
```
As instruções **if** também podem usar **===** para comparar variáveis como **isDay** a valores booleanos.

```js
let isDay = true;

if (isDay === true) {
    console.log("Lights off!");
}
```
Para usar o resultado de uma comparação várias vezes, podemos armazená-lo em uma variável como **pass**.

```js
let score = 51;
let pass = score > 50;

if (pass) {
    console.log(pass);
}
```