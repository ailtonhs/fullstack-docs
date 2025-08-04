# Definindo Atributos Dinamicamente

## Obter e Definir Atributos com Métodos

Vimos como podemos alterar atributos HTML. Existe também uma maneira masi rápida de fazer isso com **métodos** JavaScript.

Depois de acessar e armazenar a imagem, também precisaremos do atributo **src** do elemento **img**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="displayAttribute()">Dispaly Attribute</button>
		<br>

		<img src="https://mimo.app/r/cat.png">

		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function displayAttribute() {
    const img = document.querySelector("img");

    const imageLink = ;
}
```
Para obter o valor de um atributo, podemos usar o método **getAttribute()**. Colocamos o elemento primeiro, seguido por **.** e **getAttribute()**.

```js
function displayAttribute() {
    const img = document.querySelector("img");

    const imageLink = img.getAttribute();
}
```
Dentro dos parênteses, especificamos qualquer atributo que queremos obter. Aqui, vamos codificar **src** entre aspas para obter a fonte da imagem.

```js
function displayAttribute() {
    const img = document.querySelector("img");

    const imageLink = img.getAttribute("src");

}
```

Podemos confirmar que obtivemos o valor imprimindo a variável **imagemLink** no **p** do nosso arquivo **index.html**.

```js
function displayAttribute() {
    const img = document.querySelector("img");

    const imageLink = img.getAttribute("src");

    const p = document.querySelector("p");

    p.innerText = imageLink;
}
```
**getAttribute()** também funciona se quisermos obter todos os valores de um determinado atributo atributo, como os múltiplos valores de **style**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="displayAttribute()">Dispaly Styles</button>
		<br>

		<a style="color: red; font-size: 12px;" href="https://instagram.com">About Me</a>

		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function displayAttribute() {
    const el = document.querySelector("a");

    const linkStyle = el.getAttribute("style");

    const p = document.querySelector("p");

    p.innerText = linkStyle;
}
```
Além de obter atributos, também podemos **definir** ou atualizar atributos!

Para definir o valor do atributo, precisamos usar o método **setAttribute()**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<button onclick="displayAttribute()">Dispaly Attribute</button>
		<br>

		<img src="https://mimo.app/r/cat.png">

		<p></p>

		<script src="script.js"></script>
	</body>
</html>
```
```js
function displayAttribute() {
    const img = document.querySelector("img");
    const imgLink = img.getAttribute("src");
    const p = document.querySelector("p");

    p.innerText = imgLink;

    img.setAttribute();
}
```
Semelhante ao **getAttribute()**, primeiro temos que especificar qual atributo queremos definir dentro dos parênteses. 

Vamos definir **src** como atributo que queremos definir.

```js
function displayAttribute() {
    const img = document.querySelector("img");
    const imgLink = img.getAttribute("src");
    const p = document.querySelector("p");

    p.innerText = imgLink;

    img.setAttribute("src");
}
```
Depois de especificar qual atributo queremos definir dentro dos parênteses, também precisamos especificar o valor.

Vamos definir **"https://mimo.app/r/kittles.png"** como o valor do atributo **src** da imagem. Desta forma, vamos mudar a imagem do gato.

```js
function displayAttribute() {
    const img = document.querySelector("img");
    const imgLink = img.getAttribute("src");
    const p = document.querySelector("p");

    p.innerText = imgLink;

    img.setAttribute("src", "https://mimo.app/r/kittles.png");
}
```