# Comparando String

## Operador de Desigualdade

Para verificar se uma string não é igual a outra string, usamos o **operador de desigualdade estrita**, **!==**.

```js
console.log("apple" !== "orange");
```

Se a string à esquerda não for igual à string à direita, como em **"apple" !== "orange"**, o resultado é **true**.

```js
console.log("apple" !== "orange");
```
Se a string à esquerda for igual à string à direita, como em **"orange" !== "orange"**, o resultado é **false**.

```js
console.log("orange" !== "orange");
```
Para armazenar o resultado de uma comparação em uma variável, usamos o sinal **=**.

```js
const isNotDuplicate = "apple" !== "orange";
```