# Acessar Múltiplos Elementos HTML

## Tag e Classe

Até agora, só vimos maneiras de acessar um elemento de cada vez com métodos como **getElementById()** ou **querySelector()**.

```html
    <ul>
		<li>Michael</li>
		<li>Jonas</li>
		<li>Ellen</li>
	</ul>

	<button onclick="displayItem()">Display item</button>
	<p></p>

	<script src="script.js"></script>
```

```js
function displayItem() {
    const el = document.querySelector("li");
    const p = document.querySelector("p");


    p.innerText = el.innerHTML;
}
```
Mas e se quisermos acessar mais de um elemento ao mesmo tempo? Por exemplo, e se quisermos contar itens em uma lista?

Podemos obter uma **coleção** de elementos do mesmo tipo de tag com **getElementsByName()**.

```html
<body>
	<ul>
		<li>Michael</li>
		<li>Jonas</li>
		<li>Ellen</li>
	</ul>
	<button onclick="displayItem()">Display length</button>
	<div></div>

	<script src="script.js"></script>
</body>
```

```js
function displayItem() {
    const el = document.getElementsByTagName("li")
    const div = document.querySelector("div");


    div.innerHTML = el.length;
}
```
Coleções são semelhantes a **arrays**. Elas trabalham com índice que começam em **0**.

```js
function displayItem() {
    const el = document.getElementsByTagName("li")
    const div = document.querySelector("div");


    div.innerText = el[0].innerHTML;
}
```
Assim como arrays, também podemos acessar a propriedade **length** da coleção.

```html
<body>
	<ul>
		<li>Michael</li>
		<li>Jonas</li>
		<li>Ellen</li>
	</ul>

	<button onclick="displayLength()">Display length</button>
	<p></p>

	<script src="script.js"></script>
</body>
```
```js
function displayLength() {
    const el = document.getElementsByTagName("li")
    const p = document.querySelector("p");


    p.innerText = el.length;
}
```
Se quisermos retornar uma coleção que contém elementos especificos de uma classe, podemos usar o método **getElementsByClassName** em vez disso.

```html
<body>
	<ul>
		<li class="urgent">buy milk</li>
		<li class="urgent">call grandma</li>
		<li>workout</li>
	</ul>

	<button onclick="displayItem()">Display length</button>

	<p></p>

	<script src="script.js"></script>
</body>
```
```js
function displayItem() {
    const el = document.getElementsByClassName("urgent")
    const p = document.querySelector("p");


    p.innerText = "You have " + el.length + " urgent tasks";
}
```
Como **getElementsByClassName()** também retorna uma coleção, podemos então acessar cada elemento através do índice.

```js
function displayItem() {
    const el = document.getElementsByClassName("urgent")
    const p = document.querySelector("p");


    p.innerText = el[0].innerHTML;
}
```
Para acessar vários elementos que têm mais de uma classe, basta adicionar as classes com um espaço entre elas.

```html
<body>
	<ul>

	    <li class="urgent important">buy milk</li>
		<li class="urgent important">call grandma</li>
		<li>workout</li>
	</ul>

	<button onclick="displayItem()">Display number od urgent of important items</button>

	<p></p>

	<script src="script.js"></script>
</body>
```

```js
function displayItem() {
    const el = document.getElementsByClassName("urgent important")
    const p = document.querySelector("p");


    p.innerText = el.length;
}
```