# Adicionando Cor com Valores Hexadecimais

## Cores

Até agora, usamos cores padrão do CSS, que têm alguns nomes únicos. No entanto, existem milhões de outras cores que podemos usar.

Podemos adicionar cores com um **valor hexadecimal**, também conhecido como **valor hex**. Por exemplo, preto em hex é **#000000**.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<h1>Contrast</h1>
	<p>Web development with a punch</p>
</html>
```

```css
body {
    text-align: center;
    font-family: 'Courier New';
    color: white;
}

h1 {
    background-color: #000000;
}
```
Os valores hexadecimais sempre começam com um **#**.

```css
h1 {
    background-color: #000000;
}
```
O **#** seguido por seis caracteres que são números de **0** a **9** ou letras de **A** a **F**. Por exemplo, **#FFFFFF** é branco puro.

```css
body {
    color: #FFFFFF;
}
```
Com valores hexadecimais, estamos misturando três cores principais: vermelho, verde e azul. 
Abaixo, codifique o valor hex **FF0000**, que é vermelho.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<h4>Order balloons in one of the following colors</h4>
	
	<button class="red">Red #FF0000</button>

	<button class="green">Green #00FF00</button>

	<button class="blue">Blue #0000FF</button>
</html>
```
```css
.red {
    background-color: #FF0000;
}

.green {
    background-color: #00FF00;
}

.blue {
    background-color: #0000FF;
}

button {
    color: #FFFFFF;
    padding: 5px;
    border-radius: 10px;
    font-weight: bold;
}
```

Os valores hexadecimais nos dão acesso a mais de 16 milhões de combinações de cores. Você não precisa memorizá-los, saber como codificá-los é suficiente.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h1 class="gradient1">Gradient 1</h1>
		<h1 class="gradient2">Gradient 2</h1>
		<h1 class="gradient3">Gradient 3</h1>
		<h1 class="gradient4">Gradient 4</h1>
	</body>
</html>
```
```css
body {
    color: #FFFFFF;
    text-align: center;
    background-color: #FAF5F1;
}

h1 {
    border: 4px solid #FFFFFF;
    border-radius: 20px;
    padding: 20px;
}

.gradient1 {
    background: linear-gradient(to right, #EE9CA7, #FFDDE1);
}

.gradient2 {
    background: linear-gradient(to right, #2193B0, #6DD5ED);
}

.gradient3 {
    background: linear-gradient(90deg, #00416A, #E4E5E6);
}

.gradient4 {
    background: linear-gradient(90deg, #334D50, #CBCAA5);
}
```