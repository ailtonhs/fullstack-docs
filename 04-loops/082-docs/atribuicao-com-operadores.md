# Atribuição com Operadores

Como a autoatribuição é uma ferramenta poderosa para construir programas, vamos aprender alguns operadores que nos ajudam a escrever código mais rapidamente.

Sabemos que podemos adicionar **1** a uma variável escrevendo o nome da variável. Neste caso, **likes**.

```js
let likes = 5;
likes = likes + 1;
console.log(likes);//6
```

Em vez de reescrever o nome da variável, podemos usar o operador **+=** para adicionar um número como **likes += 1**.
```js
let likes = 5;
likes += 1;
console.log(likes);//6
```

Para subtrair o valor de uma variável, usamos o operador **-=**, como aqui onde diminuímos **likes** por **3**.

```js
let likes = 5;
likes -= 3;
console.log(likes);//2
```

O **operador de incremento**, **++**, colocado após o nome de uma variável, aumenta seu valor em **1**. Aqui, **likes++** aumentará o valor de **5** para **6**.

```js
let likes = 5;
likes++;
console.log(likes);//6
```
Podemos subtrair **1** do valor de uma variável usando o **operador de decremento** (**--**) assim como aqui com **likes--**.

```js
let likes = 5;
likes--;
console.log(likes);//4
```