# Descobrindo Tipos

## Trabalhando com Tipos

**+** é o sinal de juntar ou adicionar. Ao juntar duas variáveis, podemos obter resultados diferentes dependendo de seus tipos.

```js
console.log("10" + "10");//1010
console.log(10 + 10); //20
```
Ao juntar números com strings, o número será automaticamente transformado em uma string.

```js
const result = "10" + 10;
console.log(result); //1010
```
Combine uma string e um número para exibir a pontuação de um jogador.

```js
const result = "Your score: " + 99;
console.log(result);
```

Adicionar um número a uma string também funciona quando usamos uma variável como **score** que armazena um número, em vez de um valor numérico.

```js
const score = 99;
const result = "Your score: " + score;
console.log(result);
```

Também podemos juntar strings e booleans.

```js
const result = "You passed: " + true;
console.log(result);
```
Novamente, adicionar um booleano a uma string também funciona quando usamos uma variável como **pass**, que armazena um booleano.

```js
const pass = true;
const result = "You passe: " + pass;
console.log(result);