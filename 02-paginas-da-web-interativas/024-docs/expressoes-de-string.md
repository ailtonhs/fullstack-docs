# Usando Variáveis

## Expressões de Strings

Podemos adicionar valores de string juntos com um sinal de **+**.

```js
"Followers:" + "55";
```

Chamamos a soma de valores de string de uma **espressão** porque ela cria um único valor de string.

```js
console.log("Followers: " + "55");
```

Quando expressões contêm variáveis, elas usam os valores nas variáveis.

```js
const followers = "55";
"Followers: " + followers;
```
Podemos usar **console.log()** para ver os resultados de expressões.

```js
const numberOfFollowers = "55";
console.log("Followers:" + numberOfFollowers);
```
Como expressões se tornam valores, podemos atribuí-las a variáveis assim como fazemos com valores.

```js
const label = "Post:" + "13";
console.log(label);
```