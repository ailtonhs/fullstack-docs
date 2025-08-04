# Definindo Atributos Dinamicamente

## Mundaça de Atributo

Já vimos como alterar o textoo de um elemento HTML. Agora vamos aprender como alterar atributos HTML com JavaScript.

Depois de acessarmos um elemento com JavaScript, podemos obter seus atributos adicionando um **.** seguido pelo nome do atributo. 

Por exemplo, depois de armazenarmos um elemento **img** dentro da variável **el**, escrevemos **el.src** para obter o valor do atributo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="showAttribute()">Show Attribute Value</button>
		<br>

		<img src="https://mimo.app/r/cat.png">
		
		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function showAttribute() {
    const el = document.querySelector("img");

    const paragraph = document.querySelector("p");

    paragraph.innerText = el.src;
}
```

A maioria dos atributos pode ser acessada dessa forma. Acesse e exiba o atributo **href** do elemento **a**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="showAttribute()">Display Attribute Value</button>
		<br>

		<a href="https://mimo.app/r/cat.png">Profile Photo</a>
		
		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function showAttribute() {
    const el = document.querySelector("a");

    const paragraph = document.querySelector("p");

    paragraph.innerText = el.href;
}
```
Também podemos atualizar os valores dos atributos. Ao fazer isso, temos que lembrar de colocar os valores entre aspas.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="changeAttribute()">Update Photo</button>
		<br>

		<img src="https://mimo.app/r/cat.png">
		

		<script src="script.js"></script>
	</body>
</html>
```
```js
function changeAttribute()  {
    const el = document.querySelector("img");

    el.src = "https://mimo.app/r/kittles.png";
}
```
Podemos até usar atributos para mudar como os elementos funcionam e se comportam em uma página da web. 

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="changeQuestionType()">Change Survey Option</button>
		<p>Submit answer</p>

		<input type="range">
		

		<script src="script.js"></script>
	</body>
</html>
```
```js
function changeQuestionType() {
    const el = document.querySelector("input");

    el.type = "checkbox";
}
```
Mudar atributo pode ser muito poderoso. Ao adicionar o link para a folha de estilo, mudamos completamente a aparência desta página da web.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="">
	</head>
	<body>
		<button onclick="addStyleSheet()">Update website design</button>
		<br>


		<img src="https://mimo.app/r/forest.png">
		

		<script src="script.js"></script>
	</body>
</html>
```
```css
body {
	background-color: #7e947e;
    text-align: center;
    height: 300px;
}

button {
    margin:  20px;
}

img {
    padding: 20px;
    background-color: aliceblue;
    margin: 20px;
    border-radius: 30px;
}
```
```js
function addStyleSheet() {
   const el = document.querySelector("link");
   el.href = "style.css";
}
```