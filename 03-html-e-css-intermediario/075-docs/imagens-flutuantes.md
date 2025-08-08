# Imagens Flutuantes

Vamos aprender comoo envolver texto ao redor de imagens.

Para fazer o texto contornar uma imagem, primeiro colocamos um elemento com texto abaixo de uma imagem.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<img src="https://mimo.app/i/bitcoin.png">
			<p>Join us foor a live webinar/crypto party to learn more about the future of currency.
		</div>
	</body>
</html>
```
```css
img {
    width: 30%;
}
```
Em seguida, na imagem, definimos a propriedade **float** como **left** ou **right**.

```css
img {
    width: 30%;
    float: right;
}
```

E se adicionarmos um segundo elemento com texto abaixo do primeiro, mas não quisermos que ele envolva a imagem?

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<img src="https://mimo.app/i/bitcoin.png">
			<p>Join us foor a live webinar/crypto party to learn more about the future of currency.</p>

			<p class="second"> We'll give you insider info on becoming the next trillionaire. With expert insights from Mulah Moe and Jimmy Cash.</p>

		</div>
	</body>
</html>
```
Nesse caso, definimos a propriedade **clear** do elemento para o mesmo valor do elemento **img**.

```css
img {
    width: 30%;
    float: right;
    
}

.second {
    clear: right;
}
```