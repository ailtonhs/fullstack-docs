# Agrupando Elementos

## Contêineres

Desenvolvedores agrupam elementos relacionados em grupo para criar layouts únicos para seus sites.

Para criar um grupo de elementos nós envolvemos os elementos com as tags **&lt;div&gt;** e **&lt;/div&gt;**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<div>
			<h1>Latest News</h1>

			<h3>Where VC's are investing in Fintech</h3>

			<p>Arman</p>

		</div>

	</body>
</html>
```
As tags **&lt;div&gt; &lt;/div&gt;** e os elementos entre elas formam um grupo em uma página da web. **&lt;div&gt;** é a abreviação de divisão.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<div>
			<h1>Latest News</h1>

			<h3>Where VC's are investing in Fintech</h3>

			<p>Arman</p>

		</div>

	</body>
</html>
```

Chamamos elementos dentro de outros elementos de **elementos aninhados**, por exemplo, aninhando **&lt;h1&gt;Top Story&lt;/h1&gt;** dentro de **&lt;div&gt;&lt;/div&gt;**.

```html
<div>
    <h1>Top Story</h1>
</div>
```