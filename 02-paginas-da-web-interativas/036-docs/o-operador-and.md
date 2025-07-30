# Operadores Lógicos

## O operador AND

Com operadores lógicos, podemos conectar duas ou mais condições para decidir um resultado.

O operador **AND &&** retorna **true** somente se todas as condições forem **true**

```js
let isBatteryOn = true;
let isSwitchOn = true;
console.log(isBatteryOn && isSwitchOn); //true
```
O operador **&&** retornará **false** se uma ou mais condições forem **false**.

```js
let isBatteryOn = true;
let isSwitchOn = false;

console.log(isBatteyOn && isSwitchOn); //false
```
Quando operandos e operadores computam um valor booleano juntos, formam uma expressão lógica, como **isBatteryOn && isSwitchOn**.


```js
let isBatteryOn = false;
let isSwitchOn = false;
console.log(isBatteryOn && isSwitchOn); //false
```
Você também pode armazenar o resultado de uma expressão lógica em uma variável.

```js
let isBatteryOn = false;
let isSwitchOn = false;
let result = isBatteryOn && isSwitchOn;

console.log(result);
```