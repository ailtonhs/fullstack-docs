# Como Acessar um Elemento HTML

## Consultar 1 Elemento com Várias Classes

Sabemos que **querySelector()** obtém o primeiro elemento que encontra. Isso pde ser um problema se o elemento que estamos procurando aparecer mais tarde no código.


```html
<body>
    <button onclick="publish()">Publish</button>

    <h3 class="prompt">Website status</h3>

    <p class="prompt">Website not published</p>

    <script src="script.js"></script>
</body>

```
```js

function publish() {
    const el = document.querySelector(".prompt");

    el.innerHTML = "Website published!";
}
```

Se vários elementos compartilham uma classe, como **.prompt** aqui, podemos especificar sua tag.

Especificamos **p.prompt** entre parênteses para selecionar o parágrafo com a classe **.prompt**.

```js
function publish() {
    const el = document.querySelector("p.prompt");

    el.innerHTML = "Website publicado";
}
```

Também podemos procurar em elemento que tenha várias classes.
Antes de vermos isso em ação, adicione o nome da classe **update** ao segundo parágrafo.

```html
<body>
	<button onclick="publish()">Publish</button>

	<p class="prompt">Website status</p>

	<p class="prompt update">Website not published</p>
</body>
```
Para acessar um elemento com duas classes, incluímos ambas juntas. Aqui, é **.prompt.update** ou **update.prompt**.

Agora não precisamos especificar a tag HTMl porque há apenas um elemento com essas classes.

```js
function publish() {
    const el = document.querySelector(".prompt.update");

    el.innerHTML = "Website publicado";
}
```
**querySelector** é muito poderoso e podemos usá-lo para acessar qualquer **elemento específico** em uma página da web.

```html
<body>
	<button onclick="refresh()">Refresh</button>

	<h2 class="order title">Ykea order update</h2>

	<p class="order info">Delivery request received</p>
</body>
```
```js
function refresh() {
    const element = document.querySelector(".order.info");

    element.innerHTML = "Your order has been shipped. Happy self-assembly!";
}
```