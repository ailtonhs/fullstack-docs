# Introdução ao Select

Vamos mergulhar nos elementos **input**. Eles são úteis se quisermos fornecer uma lista predefinida de opções.

Em HTML, usamos o **elemento select** para criar uma lista suspensa de opções para entrada do usuário.

Criamos elemento de seleção usando a tag **&lt;select&gt;.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h4>Choose a Language</h4>

		<select>

        </select>

	</body>
</html>
```
Dentro da tag **&lt;select&gt;, incluímos tags **&lt;option&gt;**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h4>Choose a Language</h4>

		<select>
			<option>English</option>
		</select>

	</body>
</html>
```

Podemos incluir quantas opões quisermos. Para cada opção, precisamos de uma tag de abertura e de fechamento **option**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h4>Choose a Language</h4>

		<select>
			<option>English</option>
			<option>French</option>
			<option>German</option>
		</select>

	</body>
</html>
```
O atributo **selected** determina a opção pré-selecionada em uma lista suspensa.

Se você não definir explicitamente um atributo **selected** em nenhuma das opções, o navegador selecionará e exibirá automaticamente a primeira.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h4>Favorite Color</h4>

		<select>
			<option>Blue</option>
			<option selected>Green</option>
			<option>Red</option>
		</select>

	</body>
</html>
```
Assim como botões, elementos de seleção precisam de uma tag **&lt;br&gt; para colocar um abaixo do outro.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h4>Sign UP</h4>

		<select>
			<option value="volvo">Volvo</option>
		</select>
		<br>
		<select>
			<option value="saab">Saab</option>
		</select>

	</body>
</html>
```
Adicionar um atributo **name** aos seus elementos é como dar a eles um crachá em uma festa - isso ajuda todos a identificá-los facilmente.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<h4>Select your country</h4>

		<select name="countries">
			<option value="usa">USA</option>
			<option value="canada">Canada</option>
		</select>
		
	</body>
</html>
```