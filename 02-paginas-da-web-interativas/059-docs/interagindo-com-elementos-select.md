# Interagindo com Elementos Select

Para acessar a entrada de um elemento **select**, precisamos obter o elemento e usar **.value**. Podemos usar **document.getElementById()** para fazer isso.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<select id="colorSelect">
			<option value="red">Red</option>
			<option value="blue">Blue</option>
			<option value="green">Green</option>
		</select>

		<script src="script.js"></script>
	</body>
</html>
```
```js
const selectedColor = document.getElementById("colorSelect").value;
```
Após acessar a seleção do usuário, podemos usá-la como qualquer outro valor.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<select id="colorSelect">
			<option value="red">Red</option>
			<option value="blue">Blue</option>
			<option value="green">Green</option>
		</select>

		<button onclick="showSelection()">Submit</button>

		<p id="result"></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function showSelection() {
    const selectedOption = document.getElementById("colorSelect").value;

    const paragraph = document.getElementById("result");

    paragraph.innerText = "You picked: " + selectedOption;
}
```
Sabendo como obter a entrada do usuário, podemos usá-la para atualizar uma página da web.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<select id="ageSelect">
			<option>Below 18</option>
			<option>18 to 65</option>
			<option>Above 65</option>
		</select>

		<button onclick="register()">Submit</button>

		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function register() {
    const selected = document.getElementById("ageSelect").value;

    const paragraph = document.querySelector("p");

    paragraph.innerHTML = selected + ", welcome!";
}
```
Quando adicionamos o atributo **disabled**, a opção será exibida, mas não poderá ser selecionada.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<select id="mealSelect">
			<option disabled>Select preference</option>
			<option>Meat</option>
			<option>Vegetarian</option>
			<option>Vegan</option>
		</select>

		<button onclick="register()">Order meal</button>

		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function register() {
    const selected = document.getElementById("mealSelect").value;

    const paragraph = document.querySelector("p");

    paragraph.innerHTML = selected;
}
```
Ao combinar **disabled** com **selected**, a opção será selecionada por padrão, mas uma vez que for alterada, você não poderá selecioná-la novamente.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<select id="mealSelect">
			<option selected disabled>Select preference</option>
			<option>Meat</option>
			<option>Vegetarian</option>
			<option>Vegan</option>
		</select>

		<button onclick="register()">Order meal</button>

		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```