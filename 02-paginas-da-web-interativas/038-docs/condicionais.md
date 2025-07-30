# Tomando Decisões

## Condicionais

Programas inteligentes usam **booleans** para tomar decisões sobre se devem executar linhas de código ou pular elas.

Como podemos escrever código que se adapta a diferentes situações? Usando a **instrução if**.

Nós codificamos a palavra-chave **if** para uma instrução if.

```js
if (true) {
    console.log("Hello!");
}
```

A instrução if executa o código apenas se o booleano no qual está se baseando for **true**. É como dizer, se algo é verdadeiro, então faça issso. 

**Hello!** será exibido no console se definirmos o valor booleano como **true**

```js
if (true) {
    console.log("Hello!");
}
```
Mas e se quisermos pular código? Usamos **false** em vez disso. Ao definir o valor como **false** evitaremos exibir **"Hello!"**.

```js
if (false) {
    console.log("Hello");
}
```
Valores como **true** são chamados de **condições**. Declarações que dependem de condições são chamadas de **condicionais**.

Condições decidem se o código é executado ou ignorado. Elas vêm entre parênteses.

```js
if (true) {
    console.log("Hello there");
}
```