# Acessar Múltiplos Elementos HTML

## Query Selector All

Sabemos como recuperar múltiplos elementos se eles tiverem a mesma tag ou nome de classe. Como todos os **h3** aqui.

```html
<body>
	<h3>Breaking news</h3>
	<h3>The Next Olympic Sport?</h3>
	<button onclick="displayItem()">Display the first heading element</button>
	<p></p>

	<script src="script.js"></script>
</body>
```

```js
function displayItem() {
    const el = document.getElementsByTagName("h3");

    const p = document.querySelector("p");

    p.innerHTML = el.length;
}
```

Há também outra maneira poderosa de obter listas de elementos semelhantes a arrays, que é o método **querySelectorAll()**.

```html
<body>
	<h3>Breaking news</h3>
	<h3>The Next Olympic Sport?</h3>
    <h3>The New Y-Phone</h3>

	<button onclick="displayItem()">Display the first heading element</button>
	<p></p>

	<script src="script.js"></script>
</body>
```
```js
function displayItem() {
    const el = document.querySelectorAll("h3");

    const p = document.querySelector("p");

    p.innerHTML = el[2].innerHTML;
}
```

A grande vantagem do **querySelectorAll()** é que ele funciona tantoo para nomes de tag quanto para nomes de classe.

```html

<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<ul>
			<li class="urgent">buy milk</li>
			<li class="urgent">call grandma</li>
			<li>workout</li>
		</ul>
		
		<button onclick="displayItems()">Display number of urgent tasks</button>
		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function displayItems() {
    const el = document.querySelectorAll(".urgent");

    const p = document.querySelector("p");

    p.innerHTML = el.length;
}
```
Podemos também usar **querySelectorAll** para procurar elementos específicos, como um elemento **h3** da classe **news**.
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h3 class="movie gossip">Oscar Nominations Drama</h3>
		<h3 class="sports news">The Next Olympic Sport?</h3>
		<h3 class="tech news">The New Y-Phone</h3>

		<button onclick="displayItems()">Display number of news headings</button>
		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function displayItems() {
    const el = document.querySelectorAll("h3.news");

    const p = document.querySelector("p");

    p.innerHTML = el.length;
}
```
O **querySelectorAll()** nos permite fazer buscas mais avançadas, como acessar elementos de duas classes diferentes ao mesmo tempo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h3 class="movie">Oscar Nominations Drama</h3>
		<h3 class="sports">The Next Olympic Sport Annouced</h3>
		<h3 class="tech">The New Y-Phone</h3>

		<button onclick="displayItems()">Display number of news and movie headings</button>
		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function displayItems() {
    const el = document.querySelectorAll(".movie, .tech");

    const p = document.querySelector("p");

    p.innerHTML = el.length;
}
```
Para obter elementos que pertencem a duas classes diferentes, basta adicionar uma classe após a outra separada por uma vírgula.

```js
function displayItems() {
    const el = document.querySelectorAll(".movie, .tech");

    const p = document.querySelector("p");

    p.innerHTML = el.length;
}
```
Podemos até combinar seletores como classes, tags ou IDs. Adicione o nome da tag **button** para recuperá-la também e exibir seu texto no parágrafo.
```js
function displayItems() {
    const el = document.querySelectorAll(".movie, .tech, button");

    const p = document.querySelector("p");

    p.innerHTML = el[2].innerHTML;
}
```