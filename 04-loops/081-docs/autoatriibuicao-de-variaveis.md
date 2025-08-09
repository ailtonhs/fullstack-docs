# Autoatribuição de Variáveis

Vamos aprender um novo conceito que explica como as variáveis acompanham coisas como adicionar ou remover dólares de uma carteira.

Quando criamos uma variável, nós **atribuímos** a ela um valor, como atribuir **3** a **wallet**.

```js
const wallet = 3;
console.log(wallet);
```

**Atribuição a si mesmo** é quando definimos uma variável para o seu próprio valor. Por exemplo, podemos definir **wallet** para o seu valor **3** com **wallet = wallet**.

```js
let wallet = 3;
wallet = wallet;
console.log(wallet);
```
Como podemos auto-atribuir variáveis, podemos aumentar ou diminuir variáveis definidas como números.

```js
let wallet = 3;
wallet = wallet + 1;
console.log(wallet);
```
Variáveis auto-atribuídas nos permitem rastrear dados que mudam ao longo do tempo. Por exemplo, um usuário pode adicionar **2** dólares a uma carteira e depois remover **1**.

```js
let wallet = 3;
wallet = wallet + 2;

wallet = wallet - 1;
console.log(wallet);
```
Variáveis definidas como strings funcionam da mesma maneira. Tente definir **nameInfo** como **nameInfo + " john"**.

```js
let nameInfo = "Account name:";

nameInfo = nameInfo + " Elton";

nameInfo = nameInfo + " John";

console.log(nameInfo);
```
