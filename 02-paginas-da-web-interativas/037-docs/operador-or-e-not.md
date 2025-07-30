# Operadores Lógicos

## Operadores OR e NOT

Usamos o operador **OR ||**, que retorna **true** desde que pelo menos uma das condições seja **true**

```js
let isBatteryOn = true;
let isPowerOn = false;
console.log(isBatteryOn || isPowerOn); //true
```
Se todas as condições forem **false**, então o operador **||** retorna **false**.

```js
let isBatteryOn = false;
let isPowerOn = false;
console.log(isBatteryOn || isPowerOn); //false
```
Sabemos que o operador **NOT !** nega um valor booleano. Isso significa que ele retorna **true** se uma condição for **false** e vice-versa.

```js
let isBulbOn = true;
console.log(!isBulbOn); //false
```
Podemos usar **!** para negar expressões lógicas também. Para fazer isso, colocamos a expressão lógica entre parênteses.

```js
let isBatteryOn = true;
let isPowerOn = false;

console.log(!(isBatteryOn && isPowerOn)); //true
```
A expressão lógica retorna **false**, mas ao negá-la, obtemos **true**.

```js
let isBatteryOn = true;
let isPowerOn = false;

console.log(isBatteryOn && isPowerOn);// false

console.log(!(isBatteryOn && isPowerOn)); //true
```
