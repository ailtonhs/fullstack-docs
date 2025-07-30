# Tomando Decisões

## Condicionais Verdadeiras e Falsas

As istruções **if** não decidem pular ou executar o código inteiro. Elas apenas tomam decisões sobre um pedaço de código.

Este trecho de código é chamado de **bloco de código**. Nós o escrevemos entre chaves **{}**

```js
if (true) {
    console.log("I'am a code block!");
}
```

Um bloco de código pode ter mais de uma linha. Podemos adicionar quantas linhas quisermos.

```js
if (true) {
    console.log("Look at me!");
    console.log("I'm a code block!");
}
```
Em vez de usar o booleano **true**. Podemos salvá-lo em uma variável e usá-la como uma condição.

```js
const greet = true;
if (greet) {
    console.log("Hello!");
}
```
Usar uma variável definida como **false** nos permite pular o bloco de código.

```js
const greet = false;
if (greet) {
    console.log("Hello!");
}
```