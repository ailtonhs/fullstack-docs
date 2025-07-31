# Incorporando Else If

## Else If

Vamos aprender como escrever declarações condicionais que lidam com condições específicas.

Usando declações if e else, podemos escrever um programa que mostra uma saudação se **hour < 12** for **true** e outra se for **false**.

```js
let hour = 9;
if (hour < 12) {
    console.log("Good morning");
} else {
    console.log("Good night");
}
```
Para uma condição mais específica, como se **hour** não for menor que **12** mas for menor que **17**, podemos codificar **else if (hour < 17)** em vez disso.

```js
let hour = 14;
if (hour < 12) {
    console.log("Good morning");
} else if (hour < 17) {
    console.log("Good afternoon");
}
```
Chamamos isso de **declaração else if**. Esta declaração executa seu bloco de código se a condição anterior for **false** e **hour < 17** for **true**.

```js
let hour = 14;
if (hour < 12) {
    console.log("Good morning");
} else if (hour < 17) {
    console.log("Good afternoon");
}
```
Podemos codificar uma declaração **else** para executar seu bloco de código quando as condição **if** e **else if** forem **false**.

```js
let hour = 18;
if (hour < 12) {
    console.log("Good morning");
} else if (hour < 17) {
    console.log("Good afternoon");
} else {
    console.log("Good night");
}
```
Desde que venham antes da declaração **else**, podemos adicionar quantas declarações **else if** quisermos.


```js
let hour = 20;

if (hour < 12) {
    console.log("Good morning");
} else if (hour < 17) {
    console.log("Good afternoon");
} else if (hour < 21) {
    console.log("Good evening");
} else {
    console.log("Good night");
}
```