# Definindo Atributos Dinamicamente

## Objeto Style

Vamos aprender como acessar estilos CSS e alterá-los com JavaScript.

Para acessar o estilo de um elemento, primeiro precisamos adicionar o atributo **style**. Podemos então especificar o estilo exato que queremos, como **.color**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		
	</head>
	<body>
		<button onclick="showColor()">Show style</button>

		<p style="color: teal">Flowers by Muriel</p>


		<div></div>
		

		<script src="script.js"></script>
	</body>
</html>
```
```js

function showColor() {
   const el = document.querySelector("p");
   
   const container = document.querySelector("div");

   container.innerHTML = el.style.color;
}
```

Se quisermos mudar o estilo de um elemento, temos que garantir que colocamos o valor entre aspas.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		
	</head>
	<body>
		<button onclick="chargeColor()">Charge Color</button>

		<p>Spygame III - Coming January</p>


		<div></div>
		

		<script src="script.js"></script>
	</body>
</html>
```
```js
function chargeColor() {
   const el = document.querySelector("p");
   el.style.color = "#d7465f";
   
}
```
Se tivermos propriedades com várias palavras como **background-color**, precisamos transformá-las em **camel case**. Aqui, usaremos **backgroundColor**

```js
function chargeColor() {
   const el = document.querySelector("p");
   el.style.backgroundColor = "#d7465f";
}
```
Mudar o estilo com JavaScript funciona independentemente de o estilo anterior ter sido definido inline ou através de uma folha de estilo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<button onclick="chargeStyle()">Update Profile Design</button>
		<br>

		<img src="https://mimo.app/i/hacker.png">


		<script src="script.js"></script>
	</body>
</html>
```
```css
img {
    background-color: aliceblue;
    border-radius: 10px;
    border: 2px solid lightgray;
}

button, img, p {
    margin: 10px 0 0 0;
}
```
```js

function chargeStyle() {
   const el = document.querySelector("img");
   el.style.borderRadius = "45px";
   
}
```