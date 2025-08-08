# Posição Absoluta

Vamos aprender como posicionar elementos com base nas bordas de uma página da web.

Para começar a colocar um elemento em um local específico na tela, definimos **position** como **absolute**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<a href="#">Sign up to our Newsletter!</a>
	</body>
</html>
```
```css
a {
    background-color: #fdefdf;
    position: absolute;
}
```
Para colocar o elemento à direita, usamos **right: 0px;**. Isso significa que o elemento está a **0px** de distância do lado direito da página.

```css
a {
    background-color: #fdefdf;
    position: absolute;
    right: 0px;
}
```
Podemos usar as propriedades **top**, **bottom**, **right** ou **left** para posicionamento. **top: 30px;** posiciona o elemento exatamente a **30px** do topo da página.

```css
a {
    background-color: #fdefdf;
    position: absolute;
    right: 0px;
    top: 30px;
}
```
Vamos comparar o posicionamento **relativo** e **absolute**. Perceba como em uma posição **relative** a imagem está depois do link?

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<a href="#">Sign up now</a>
		<img src="https://mimo.app/i/homekia-bedroom.png">
	</body>
</html>
```
```css
a {
    background-color: #fdefdf;
    position: relative;
    
}

img {
    width: 300px;
}
```
Definir o link como **position: absolute** o remove do fluxo normal e faz com que ele se sobreponha à imagem.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<a href="#">Sign up now</a>
		<img src="https://mimo.app/i/homekia-bedroom.png">
	</body>
</html>
```
```css
a {
    background-color: #fdefdf;
    position: absolute;
    
    
}

img {
    width: 300px;
}
```