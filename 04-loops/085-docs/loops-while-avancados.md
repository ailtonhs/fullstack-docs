# Controlando While Loops

## Loops While Avançados

Para controlar o número de vesez que um loop **while** se repete, começamos com uma variável definida para um número. Chamamos essa variável de **variável contador**.

```js
let counter = 1;
```
Então, usamos uma comparação na condição para comparar a variável contador a um número. Neste caso, **counter < 4**.

```js
let counter = 1;

while (counter < 4) {

}
```
Dentro do bloco de código, fazemos a condição retornar **false** e paramos o loop incrementando a variável de contagem. Tente **counter++**.

```js
let counter = 1;
 while (counter < 4) {
     console.log(counter);
     counter++;
 }
 ```

 Mudar a condição informa ao loop quando parar. Por exemplo, mudar a condição para **counter < 10**.

 ```js
 let counter = 1;
 while (counter < 10) {
     console.log(counter);
     counter++;
 }
 ```

 Mudar o valor da variável contador altera quando o loop começa. Como definir **counter** para **5**.

 ```js
 let counter = 5;
 while (counter < 10) {
     console.log(counter);
     counter++;
 }
 ```

 Como todo o bloco de código é executado, a ordem em que você escreve o código afeta o que o console exibe. Coloque **counter++** primeiro para exibir de **6** a **10**.

 ```js
 let counter = 5;
 while (counter < 10) {
     counter++;
     console.log(counter);
 }
 ```
 