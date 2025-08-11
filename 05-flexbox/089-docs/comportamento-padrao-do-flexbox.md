# Entendendo o Flexbox

## Comportamento Padrão do Flexbox

Vamos dar uma olhada em todas as mudanças que acontecem apenas ao adicionar **display: flex;** ao nosso código.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">Have Drones Gone Too Far?</div>
			<div class="item">What Are The Games Everyone is Waiting For This Year</div>
			<div class="item">What Are The Top Coding Tricks Bill Gates Can Share With Us?</div>
		</div>
	</body>
</html>
```

```css
.container {
    border: 2px solid #806868;
    display: flex;
   
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Por padrão, o flexbox tenta ajustar os itens dentro de um contêiner em apenas **uma linha**.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    
   
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Os itens flex automaticamente **se estendem** para preencher a altura do seu contêiner.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">This text is content</div>
			<div class="item">Content</div>
			<div class="item">content</div>
		</div>
	</body>
</html>
```

```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 200px;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Os itens flex são tão largos quanto o conteúdo dentro deles. Adicione o texto mais longo para ver.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">This text is content</div>
			<div class="item">Content</div>
			<div class="item">content</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Os itens flex podem **encolher** em largura para que todos caibam em uma linha dentro do container.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">This is content</div>
			<div class="item">This is content</div>
			<div class="item">This is content</div>
			<div class="item">This is content</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    
}

.item {
    border: 2px solid #457081;
    margin: 5px;
}
```
Às vezes, os itens flex podem ter conteúdo dentro deles que é muito largo e não pode ser quebrado, como uma palavra longa.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>15 Letter Words</h3>
		<div class="container">
			<div class="item">Algorithmically</div>
			<div class="item">Accomplishments</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    width: 200px;
}

.item {
    border: 2px solid #457081;
    margin: 5px;
}
```

Se a largura total dos itens flex for maior que a do contêiner, os itens transbordam para fora do contêiner.

**display: flex;** afeta elementos inline e block da mesma forma.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>15 Letter Words</h3>
		<div class="container">
			<div class="item">Div</div>

			<button class="item">Button</button>

			<h3 class="item">Accomplishments</h3>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 100px;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**display: flex;** é o primeiro passo para usar o flexbox. Em seguida, vamos aprender sobre as diferentes propriedades que podemos adicionar a contêineres e itens.