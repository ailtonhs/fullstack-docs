# Z-index

Vamos aprender como controlar elementos sobrepostos.

Vamos começar com uma imagem com um cabeçalho abaixo dela. Defina a **width** da imagem para **300px**.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<div>
		<img src="https://mimo.app/i/minimalist_living_room.png">
		<h1>Sale</h1>
	</div>
</body>

</html>
```
```css
img {
    width: 300px;
}

h1 {
    color: #ff6042;
}
```

Definir uma imagem com **position: absolute** a remove do fluxo normal. É por isso que a imagem se sobrepõe ao cabeçalho.

```css
img {
    width: 300px;
    position: absolute;
}

h1 {
    color: #ff6042;
}
```
Podemos controlar como as imagens se sobrepõem com uma propriedade chamada **z-index**. Defina **z-index** como **0**, seu valor padrão.

```css
img {
    width: 300px;
    position: absolute;
    z-index: 0;
}

h1 {
    color: #ff6042;
}
```
Como todos os elementos têm seu **z-index** definido como **0** padrão, o navegaodr coloca a imagem na frente porque é o primeiro elemento no HTML.

```css
img {
    width: 300px;
    position: absolute;
    z-index: 0;
}

h1 {
    color: #ff6042;
}
```

Para colocar um elemento atrás de outro, definimos **z-index** para um número menor. Neste caso, codifique **-1**.

```css
img {
    width: 300px;
    position: absolute;
    z-index: -1;
}

h1 {
    color: #ff6042;
}
```

Qualquer número inteiro funciona. Coloque a imagem da classe **logo** na frente da outra imagem definindo o **z-index** para **1**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<img class="logo" src="https://mimo.app/i/snapcat.png">
		<img src="https://mimo.app/i/forrest-fall.png">
	</body>
</html>
```
```css
.logo {
    position: absolute;
    z-index: 1;
}
```
Elementos com um número de **z-index** mais alto estão sempre na frente. Defina oo **z-index** da terceira imagem para **2** para que ela sobreponha as duas primeiras imagens.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<img class="first-photo" src="https://mimo.app/i/nacho.png">
		<img class="second-photo" src="https://mimo.app/i/cat.png">
		<img class="third-photo" src="https://mimo.app/i/kittles.png">
	</body>
</html>
```
```css
img {
    position: absolute;
    width: 150px;
}

.first-photo {
    z-index: 1;
}

.second-photo {
    z-index:  1;
    top: 120px;
    left: 40px;
}

.third-photo {
    z-index: 2;
    left: 150px;
}
```