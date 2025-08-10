# Repetindo Código com For Loops

## Iteração de Código

Sabemos como repetir código usando um loop while. Como este programa que repete instruções para exibir a Bandeira Americana.

```js

let counter1 = 0;

 while (counter1 < 5) {
     console.log("***********--------------------");
     counter1++;
 }

 let counter2 = 0;

 while (counter2 < 4) {
     console.log("------------------------------------");
     counter2++;
 }
 ```

 Usando **loops for**, podemos reescrever o mesmo programa tornando-o mais fácil de entender para outros programadores.

 ```js
 for (let i = 0; i < 4; i++) {
    console.log("********---------------------")
}

for (let i = 0; i < 4; i++) {
    console.log("-------------------------")
}
```

Para criar um loop **for**, começamos com a palavra-chave **for**, parênteses **( )** e chaves **{ }**.

```js

for () {

}
```

Um loop for nos permite criar a variável de contador dentro dos parênteses, como **let counter = 1;**.

```js
for (let counter = 1;)
```
Um nome comum para uma variável contador é a letra **i**, que significa índice. Vamos usá-la para aprender sobre loops **for**.

```js
for (let i = 3;) {

}
```

Após o ponto e vírgula, colocamos uma condição como **i < 5** e adicionamos outro ponto e vírgula **;**.

```js
for (let i = 1; i < 5;) {

}
```

Por último, incrementamos a variável contador com **i++**.

```js
for (let i = 1; i < 5; i++) {

}
```

O código de um loço **for** é mais fácil de ler porque a informação sobre quantas vezes o laço se repete está dentro dos parênteses.

```js
for (let i = 1; i < 5; i++) {
    console.log(i)
}