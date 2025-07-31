# Codificando Else Statement

## Declaração Else

Um ótimo software não apenas decide o que fazer quando uma condição é **true**, ele também tem um plano de contingência se a condição for **false**.

Já sabemos que as instruções **if** nos ajudam a executar o código se uma determinada **condition** for **true**.

```js
let condition = true;

if (condition) {
    console.log("1");
}
```
Vamos adicionar outra declaração **if** que usa **!condition** para executar um código diferente se a condição for **false**.

```js
let condition = true;
if (condition) {
    console.log("1");
}

if (!condition) {
    console.log("2");
}
```

Em vez de criar duas declarações **if**, usamos uma declaração **if/else** para alcançar o mesmo resultado.

```js
let condition = false;

if (condition) {
    console.log("1");

} else {
    console.log("2");
}

```
A declaração **else** de uma instrução **if/else** sempre vai no final.

```js
let condition = false;
if (condition) {
    console.log("1");
} else {
    console.log("2");
}
```
Vamos analizar um caso de uso: se **isDay** for **true** queremos apagar as luzes.

```js
let isDay = true;
if (isaDay === true) {
    console.log("Lights off!");
}
```
Se **isDay** for **false**, podemos adicionar uma declaração **else** para acender as luzes.

```js
let isDay = false;

if (isDay) {
    console.log("Lights off!");
} else {
    console.log("Lights on!");
}
```
A declaração **else** não precisa de sua própria condição. Isso porque ela lida com os casos em que a condição **if** é **false**.

```js
let number = 99;

if (number === 1) {
    console.log("It's 1");
} else {
    console.log("It's not 1");
}
```
A declaração **else** é como uma resposta padrão. Aqui, ela exibe **"It's not 1"** para todos os números diferentes de 1.

```js
let number = 99;

if (number === 1) {
    console.log("It's 1");
} else {
    console.log("It's not 1");
}
```
