# Exibindo Elementos

## Elementos de Bloco

Elementos como **p**, **div** ou **h3** funcionam de maneira diferente no fluxo normal do que elementos **inline**. Eles sempre aparecem em linhas separadas.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<h3>Terms and conditions</h3>

	<p>We win't share your data with anyone.
</body>

</html>
```
```css
h3 {
    background-color: lightGray;
}

```
O valor **display** para elementos que ocupam toda a largura do elemento pai é **block**.

```css
p {
    display: block;
    border: solid 2px black;
}
```
Como  ocupam toda a largura do elemento pai, os elementos **block** sempre começam em nova linha.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<a href="#">Buy Now</a>

	<p>40% OFF</p>
</body>

</html>
```
```css

p {
    background-color: #58fccf;
}
```