# Elemento Span

## Elementos Inline e Block

Às vezes, queremos estilizar apenas uma pequena parte de uma página da web, como apenas algumas palavras. Vamos aprender a fazer isso usando a tag **&lt;span&gt;**.

O elemento **&lt;span&gt;** é usado para aplicar estilos a partes do texto.

Vamos usar a tag **&lt;span&gt;** para fazer o texto **pinch** parecer diferente do resto do texto.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>Simple Cake Recipe</h3>

		<ul>
			<li>1 cup white sugar</li>
			<li>0.5 cup butter</li>
			<li>1 <span>pinch</span> of salt</li>
			<li>1.5 teaspoons baking powder</li>
			<li>2 teaspoons vanilla extract</li>
		</ul>
	</body>
</html>
```
```css
span {
    color: #0078e6;
}
```
Assim como outros elementos, podemos usar o seletor de tag **span** para estilizar todas as tags **&lt;span&gt;** ao mesmo tempo.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>Simple Cake Recipe</h3>

		<ul>
			<li>1 <span>cup</span> white sugar</li>
			<li>0.5 <span>cup</span> butter</li>
			<li>1 pinchn of salt</li>
			<li>1.5 teaspoons baking powder</li>
			<li>2 teaspoons vanilla extract</li>
		</ul>
	</body>
</html>
```
```css
span {
    color: #0078e6;
}
```
Se houver muitos elementos **&lt;span&gt;** diferentes em uma página da web, podemos usar seletores de ID ou classe para aplicar estilos diferentes.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>Simple Cake Recipe</h3>

		<ul>
			<li>1 <span class="cup">cup</span> white sugar</li>
			<li>0.5 <span class="cup">cup</span> butter</li>
			<li>1 <span class="pinch">pinchn</span> of salt</li>
			<li>1.5 <span class="teaspoon">teaspoons</span> baking powder</li>
			<li>2 <span class="teaspoon">teaspoons</span> vanilla extract</li>
		</ul>
	</body>
</html>
```
Podemos então adicionar diferentes estilos aos seletores de classe para criar páginas da web mais intuitivas.

```css
.cup {
    color: #0078e6;
}

.pinch {
    color: #a8561e;
}

.teaspoon {
    color: #6d3acf;
}
```
