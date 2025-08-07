# Definindo Tamanho com Percentuais

## Porcentagens

Definir o tamanho dos elementos usando valores absolutos, como **200px**, significa que eles terão exatamente o mesmo tamanho em qualquer tela.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>Furniture Magazine</h3>

		<img src="https://mimo.app/i/minimalist-living-room.png">
	</body>
</html>
```
```css
h3 {
    background-color: aliceblue;
}

img {
    width: 200px;
}
```
Podemos dimensionar um elemento **relativo ao seu pai** usando uma porcentagem. Aqui, **100%** significa que a imagem ocupa 100% da largura do elemento **body**.

```css
img {
    width: 100%;
}
```
Definir **width** para **50%** ocupa metade do elemento **body**, ou seja, metade da página.

```css
img {
    width: 50%;
}
```
Agora, vamos fazer um elemento **&lt;div&gt;** ser o pai da imagem para tentar algo diferente.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
		<h3>Furniture Magazine</h3>
	<div>

		<img src="https://mimo.app/i/minimalist-living-room.png">
	</div>
</body>

</html>
```

```css
h3 {
    background-color: aliceblue;
}

img {
    width: 50%;
}
```
Para ver como as porcentagens dependem do elemento pai, defina a **width** do novo elemento **&lt;div&gt;** para **250px**.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
		<h3>Furniture Magazine</h3>
	<div>

		<img src="https://mimo.app/i/minimalist-living-room.png">
	</div>
</body>

</html>
```

```css
h3 {
    background-color: aliceblue;
}

div {
    border: 2px solid lightskyblue;
    width: 250px;
}

img {
    width: 100%;
}
```
Defina o tamanho da imagem para **50%** significa que ele terá metade da largura do elemento pai. Isso significa que a imagem agora tem **125px**.

```css
h3 {
    background-color: aliceblue;
}

div {
    border: 2px solid lightskyblue;
    width: 250px;
}

img {
    width: 50%;
}
```