# Looping Descendente

## Contagem regressiva

Este loop for conta de **1** a **5**. Vamos aprender como alterá-lo para fazer um loop decrescente de **5** a **1**.

```js
for (let i = 1; i < 6; i++) {
    console.log(i)
}
```

Primeiro, vamos mudar onde o loop começa definindo a variável de contagem para **5**.

```js
for (let i = 5; i < 5; i++) {
    console.log(i)
}
```

Em seguida, vamos mudar a condição para que o loop **pare** quando **i** for maior que **0**.

```js
for (let i = 5; i > 0; i--) {
    console.log(i)
}
```
Em vez de incrementar a variável contador, nós a decrementamos com **i--**.

```js
for (let i = 5; i > 0; i--) {
    console.log(i)
}
```

Para incluir **0** ao contar regressivamente, usamos **>=** em vez **>**.

```js
for (let i = 5; i >= 0; i--) {
    console.log(i)
}
```