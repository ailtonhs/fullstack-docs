# Usando Classes para Layouts

## Classes

Vamos ver como podemos adicionar classes aos elementos **&lt;div&gt;** para estilizar diferentes partes de uma página da web.

Vamos começar adicionando uma classe a um elemento filho.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>List of royal family</h3>

		<div>
			<p class="throne-successor">Prince George</p>
			<p>Princess Charlotter</p>
			<p>Prince Louis</p>
		</div>
	</body>
</html>
```
Classes CSS nos permitem **sobrescrever** propriedades herdadas. Aqui, podemos usar a classe CSS **throne-successor** para mudar a cor da fonte de apenas um elemento **&lt;p&gt;**.

```css
div {
    border: 3px solid lightgray;
    color: brown;
}

.throne-successor {
    color: gold;
}
```

Adicionar classes aos elementos **&lt;div&gt;** é uma das melhores maneiras de estilizar diferentes grupos de elementos simultaneamente.

```html
<!DOCTYPE html>
<html>

<head>
	<title>Page Title</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<div class="headline">
		<h3>Sesame Ventures</h3>
		<h6>Replacing the cookie habit with entrepreneurship</h6>
	</div>

	<div class="main-story">
		<h6>About</h6>
		<p>Sesame Ventures is a fund that invests in education technology, as pathway to a brighter future.</p>
		
	</div>
</body>

</html>
```
```css
.headline {
    background-color: orange;
    padding: 10px;
}

.main-story {
    border: 3px solid darkgreen;
    padding: 20px;
}
```