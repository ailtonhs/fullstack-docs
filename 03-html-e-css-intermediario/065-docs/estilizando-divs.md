# Estilizando Grupos de Elementos

## Estilizando Divs

Vamos aprender como estilizar grupos de elementos em uma página da web com a ajuda de elemento **&lt;div&gt;**.

Agrupe esses elementos dentro de um elemento **&lt;div&gt;** para começar.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<h1>Sesame Ventures</h1>

			<h4>A fund that invests in education.</h4>
		</div>
	</body>
</html>
```
Podemos estilizar o grupo de elementos que criamos, usando **div** como um seletor de tag.

```css
div {
    border: solid 3px lightgray;
    text-align: center;
}
```
Podemos adicionar outras propriedades para estilizar o grupo de elementos. Por exemplo, definir **background-color** como **bisque**.

```css
div {
    border: solid 3px lightgray;
    text-align: center;
    background-color: bisque;
}
```
Para melhorar o espaçamento dentro e fora do grupo de elementos, podemos adicionar margens e preenchimento. Como **margin: 20px;**.

```css
div {
    border: solid 3px lightgray;
    text-align: center;
    background-color: bisque;
    margin: 20px;
}
```