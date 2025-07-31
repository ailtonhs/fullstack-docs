# Reutilizando Código com Funções

## Construa uma Função

Em vez de criar muitos códigos diferentes, os sites usam **funções** para agrupar códigos relacionados e executar a tarefa em um só lugar.

Para começar a agrupar código relacionado, começamos codificando a palavra-chave **function**

```js
function
```

Em seguida vem o nome da função em camel case, como **greetUser**, seguido por parênteses, **()**.

```js
function greetUser()
```

Chaves **{}**, delimitam o bloco de código que pertence à função.

```js
function greetUser() {

}
```

O código que queremos agrupar vai entre as chaves. Esta função agrupa duas instruções **console.log()** relacionadas.

```js
function greetUser() {
    console.log("Good morning Anna");
    console.log("Welcome back");
}
```
Para executar o código, precisamos **chamar** a função. Fazemos isso codificando seu nome seguido por parênteses, como **greetUser();**.

```js
function greetUser() {
    console.log("Good morning Anna");
    console.log("Welcome back");
}

greetUser();
```