# Obtendo Entrada do Usuário

## Interagindo com Elementos de Input

Para acessar a entrada do usuário de um elemento **input**, precisamos adicionar **.value** aoo final de **document.getElementById()**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<input type="text" id="usernameInput" placeholder="Username">

		<button onclick="register()">Register</button>

		<p id="message"></p>

		<script src="script.js"></script>


	</body>
</html>
```
```js
const username = document.getElementById("usernameInput").value;
```
Depois de acessar a entrada do usuário, podemos usá-la como qualquer outro valor.

```js
function register() {
    const paragraph = document.querySelector("p");

    const username = document.getElementById("usernameInput").value;

    paragraph.innerHTML = username;
}

```
Sabendo como obter a entrada do usuário, podemos usá-la para atualizar uma página da web.

```js
function register() {
    const paragraph = document.querySelector("p");

    const username = document.getElementById("usernameInput").value;

    paragraph.innerHTML = username + " , you're signed";
}
```
Acessar a entrada do usuário de ume elemento **textarea** funciona da mesma maneira.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h1>Customer Reviews</h1>

		<textarea id="reviewText" rows="5" cols="18" placeholder="Write your review here"></textarea>
		<br>

		<button onclick="addReview()">Add Review</button>
		<p id="addedReview"></p>

		<script src="script.js"></script>


	</body>
</html>
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h1>Customer Reviews</h1>

		<textarea id="reviewText" rows="5" cols="18" placeholder="Write your review here"></textarea>
		<br>

		<button onclick="addReview()">Add Review</button>
		<p id="addedReview"></p>

		<script src="script.js"></script>


	</body>
</html>
```

```js
function addReview() {
    const review = document.getElementById("reviewText").value;

    const addedReview = document.getElementById("addedReview");

    addedReview.innerHTML = review;
}
```