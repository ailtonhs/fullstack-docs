# Construindo Listas

## Listas Aninhada

Os itens de lista podem conter mais do que apenas texto. Eles também podem conter imagens ou links.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h2>Useful Links</h2>
		<ul>
			<li><a href="https://weather.com">weather</a></li>
		</ul>
	</body>
</html>
```
Os itens de lista podem até conter outras listas.

Para criar uma lista aninhada, começamos com uma lista não ordenada simples e um item de lista.

Adicionamos itens de lista a uma lista aninhada da mesma forma que os adicionamos a outras listas.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>

		<ul>
			<li>Best Comic Book Movies:
				<ol>
					<li>The Dark Knight</li>
					<li>Spider-man 2</li>
				</ol>
			</li>
		</ul>
	</body>
</html>
```