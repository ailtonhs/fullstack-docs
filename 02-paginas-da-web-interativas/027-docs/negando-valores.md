# Usando True e False

## Negando Valores

Um sinal de **!** na frente de **true** faz com que a expressão resulte em **false**. Se algo não é verdadeiro, tem que ser falso.

O sinal **!** é o **operador de negação**. Ele transforma valores em seu **oposto**

Quando mudamos um valor para o seu oposto com **!**, nós o negamos.

```js
console.log(!true);
```
O operador **!** antes de **false** também altera seu valor. Se um valor não é **false**, ele tem que ser **true**.

```js
console.log(!false);
```
Podemos usar o operador **!** com variáveis para negar os valores que elas armazenam.

```js
const isMorning = true;
console.log(!isMorning);
```
Podemos salvar uma negação inteira em outra variável também.

```js
const isMorning = true;
const isEvening = !isMorning;

console.log(isEvening);
```