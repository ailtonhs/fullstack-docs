# Como Acessar um Elemento HTML

## Selecionar por ID

Já vimos que podemos usar variáveis JavaScript, como **element** aqui, para armazenar elementos HTML.

```html
<!doctype html>
<html>
<body>
    <h3>Breaking News</h3>
    <p id="messages">New messages</p>

    <script src="script.js"></script>
</body>
</html>
```
```js
const element = document.getElementById("messages");
```
Podemos acessar o texto do parágrafo através do nome da variável, com **.innerHTML**.

```js
const element = document.getElementById("messages");

console.log(element.innerHTML);
```
Podemos também usar a variável para atualizar o conteúdo do parágrafo, adicionando **=** e novo valor **"No messages"**.

```js
const element = document.getElementByid("messages");

element.innerHTML = "No messages";
```