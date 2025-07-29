# Comparando Strings

## Operador de Igualdade

Podemos usar comparações para verificar se uma string é igual ou diferente de outra string.

Para verificar se uma string é igual a outra string, podemos usar o **operador de igualdade estrita**, **===**.

```js
console.log("apple" === "apple");
```
Se a string à esquerda for igual à string à direita, como em **"apple" === "apple"**, o resultado é **true**.

```js
console.log("apple" === "apple");
```
Se a string à esquerda não for igual à string à direita, como em **"apple" === "orange"**, o resultado é **false**

```js
console.log("apple" === "orange");
```
Também podemos comparar variáveis que armazenam estring entre si, como em **fruit1 === fruit2**.

```js
const fruit1 = "apple";
const fruit2 = "orange";
console.log(fruit1 === fruit2);
```