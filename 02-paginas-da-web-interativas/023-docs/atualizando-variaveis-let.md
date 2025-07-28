# Usando Variáveis

## Atualizando Variáveis com Let

Já vimos que variáveis **let**, ao contrário de **const**, podem mudar e atualizar os valores que armazenam.

```js
let currentStatus = "Watching Netflix";
currentStatus = "Relaxing at the beach";
console.log(currentStatus);
```

Podemos atualizar variáveis **let** quantas vezes quisermos.

```js
let currentStatus = "Watching Netflix";
currentStatus = "Relaxing at the beach";
console.log(currentStatus);

currentStatus = "Reading";
console.log(currentStatus);
```

Também podemos dar às variáveis os valores de outras variáveis, definindo uma variável para a outra.

```js
let defaultStatus = "Hi there!";
let currentStatus = "Playing football";

currentStatus = defaultStatus;
console.log(currentStatus);
```

Quando atualizamos uma variável, ela esquece seu valor anterior.

```js
let currentStatus = "Playing football";
console.log(currentStatus);

currentStatus = "Walking the dog";
console.log(currentStatus);