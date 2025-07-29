# Comparando Números

## Verificação de Igualdade

Para verificar se um número é menor ou igual a outro número, usamos o **operador menor ou igual a**, **<=**.

```js
console.log(1 <= 3);
```
Se o número à esquerda for menor ou igual ao número à direita, como em **11 <= 11**, o resultado é **true**.

```js
console.log(11 <= 11);
```
Para verificar se um número é maior ou igual a outro número, usamos o **operador maior ou igual a**, **>=**.

```js
console.log(3099 >= 3099);
```
Para armazenar o resultado de uma comparação em uma variável, usamos o sinal **=**. Este é o **operador de atribuição**.

```js
const result = 1 <= 15;
console.log(result);
```
Podemos também usar o operador de comparação para comparar uma variável com outra variável, como em **min <= max**.

```js
const min = 5;
const max = 10;
const result = min <= max;
console.log(result);
```