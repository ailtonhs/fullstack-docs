## Alterando Class CSS

## ClassList

Há uma razão pela qual não usamos **setAttribute()** para definir classes. Se o usarmos para mudar uma classe, ele substitui a classe anterior.

podemos ver o problema se executarmos este código e tentarmos fazer o texto aparecer em negrito e itálico ao mesmo tempo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
        <link rel="stylesheet" href="style.css">
	</head>
	<body>
		<button onclick="turnBold()">Turn Bold</button>

		<button onclick="turnItalic()">Turn Italic</button>

		<br>

		<p>It was a bright cold day in April, and the clocks were striking thirteen.</p>

		<script src="script.js"></script>
	</body>
</html>
```
```css
body {
    text-align: center;
}

button {
    margin: 30px;
    padding: 3px 12px;
    border-radius: 20px;
    font-weight: bold;
    border: 0 solid;
    outline: nome;
    background-color: #d9e8fb;
    color: #4d4d87;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```

```js
function turnBold() {
    const el = document.querySelector("p");

    el.setAttribute("class", "bold")
}

function turnItalic() {
    const el = document.querySelector("p");
    el.setAttribute("class", "italic");
}
```
Existe uma maneira melhor de adicionar e remover classes, que é com uma propriedade chamada **classList**.

Para adicionar uma nova classe sem substituir a anterior, primeiro, precisamos adicionar a propriedade **classList**. Em seguida, podemos usá-la para acessar o método **add()**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="addBold()">Turn Bold</button>

		<br>

		<p class="italic">It was a bright cold day in April, and the clocks were striking thirteen.</p>

		<script src="script.js"></script>
	</body>
</html>
```
```css
body {
    text-align: center;
}

button {
    margin: 30px;
    padding: 3px 12px;
    border-radius: 20px;
    font-weight: bold;
    border: 0 solid;
    outline: nome;
    background-color: #d9e8fb;
    color: #4d4d87;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```
```js
function addBold() {
    const el = document.querySelector("p");

    el.classList.add();
}
```
Dentro do método **add()**, nós codificamos a classe que queremos adicionar ao elemento.

```js
function addBold() {
    const el = document.querySelector("p");

    el.classList.add("bold");
}
```
Classes também podem ser removidas de um elemento. Para remover uma classe, codifique o método **remove().

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="removeBold()">Remove Bold</button>

		<br>

		<p class="italic bold">It was a bright cold day in April, and the clocks were striking thirteen.</p>

		<script src="script.js"></script>
	</body>
</html>
```
```css
body {
    text-align: center;
}

button {
    margin: 30px;
    padding: 3px 12px;
    border-radius: 20px;
    font-weight: bold;
    border: 0 solid;
    outline: nome;
    background-color: #d9e8fb;
    color: #4d4d87;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```
```js
function removeBold() {
    const el = document.querySelector("p");

    el.classList.remove("bold");
}
```
Se quisermos adicionar ou remover automaticamente uma classe quando chamamos a função, podemos usar o método **toggle()**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="toggleBold()">Bold</button>

		<br>

		<p class="italic bold">It was a bright cold day in April, and the clocks were striking thirteen.</p>

		<script src="script.js"></script>
	</body>
</html>
```
```css
body {
    text-align: center;
}

button {
    margin: 30px;
    padding: 3px 12px;
    border-radius: 20px;
    font-weight: bold;
    border: 0 solid;
    outline: nome;
    background-color: #d9e8fb;
    color: #4d4d87;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```

```js
function toggleBold() {
    const el = document.querySelector("p");

    el.classList.toggle("bold");
}
```
Podemos adicionar várias classes a um elemento ao mesmo tempo. Vamos adicionar duas novas classes ao nosso elemento de parágrafo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="addClasses()">Style 1</button>

		<br>

		<p class="italic bold">It was a bright cold day in April, and the clocks were striking thirteen.</p>

		<script src="script.js"></script>
	</body>
</html>
```
```css
body {
    text-align: center;
}

button {
    margin: 30px;
    padding: 3px 12px;
    border-radius: 20px;
    font-weight: bold;
    border: 0 solid;
    outline: nome;
    background-color: #d9e8fb;
    color: #4d4d87;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}

.highlight {
    background-color: yellow;
}

.underline {
    text-decoration: underline;
}
```

```js
function addClasses() {
    const el = document.querySelector("p");

    el.classList.add("highlight", "underline");
}
```
Podemos facilmente remover várias classes também. Remova as classes **highight** e **underline** do nosso elemento.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="addClasses()">Style 1</button>

		<br>

		<p class="italic bold highlight underline">It was a bright cold day in April, and the clocks were striking thirteen.</p>

		<script src="script.js"></script>
	</body>
</html>
```

```css
body {
    text-align: center;
}

button {
    margin: 30px;
    padding: 3px 12px;
    border-radius: 20px;
    font-weight: bold;
    border: 0 solid;
    outline: nome;
    background-color: #d9e8fb;
    color: #4d4d87;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}

.highlight {
    background-color: yellow;
}

.underline {
    text-decoration: underline;
}
```

```js
function addClasses() {
    const el = document.querySelector("p");
    el.classList.remove("highlight", "underline")
}
```