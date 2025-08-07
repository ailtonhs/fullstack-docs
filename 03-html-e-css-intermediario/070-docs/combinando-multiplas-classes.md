# Combinando Múltiplas Classes

## Classes Poderosas

Vamos usar três classes CSS: **color**, **italic** e **bold**, para aprender como combiná-las em HTML.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<p class="bold">Font Style</p>

		<p class="color">Color</p>

		<p class="italic">Italic</p>
	</body>
</html>
```
```css
.color {
    color: brown;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```
Para combinar estilos, adicionamos **múltiplas classes CSS** a um elemento HTML. Como adicionar **italic** como uma segunda classe CSS a este parágrafo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<p class="bold">Font Style</p>

		<p class="color italic">Color and italic</p>

		<p class="color">Color</p>

		<p class="italic">Italic</p>
	</body>
</html>
```

```css
.color {
    color: brown;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```
Podemos usar quantas classes CSS quisermos para combinar estilos sem mexer no CSS. Adicione **bold** como uma terceira classe CSS ao mesmo atributo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<p class="bold">Font Style</p>

		<p class="color italic bold">Color, italic and bold</p>

		<p class="color">Color</p>

		<p class="italic">Italic</p>
	</body>
</html>
```
```css
.color {
    color: brown;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```
Várias classes CSS nos permitem criar combinações de diferentes estilos dentro do nosso HTML. Adicione a classe **bold** ao terceiro parágrafo também.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<p class="bold">Font Style</p>

		<p class="color italic bold">Color, italic and bold</p>

		<p class="color bold">Color</p>

		<p class="italic">Italic</p>
	</body>
</html>
```
```css
.color {
    color: brown;
}

.italic {
    font-style: italic;
}

.bold {
    font-weight: bold;
}
```