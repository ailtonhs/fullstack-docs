# Usando Flex Direction

## Direção Flexível

O Flexbox nos permite alterar o layout do conteúdo sem mexer no HTML.

Para controlar a direção em que os elementos são exibidos, usamos a propriedade **flex-direction**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">1</div>
			<div class="item">2</div>
			<div class="item">3</div>
			<div class="item">4</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

O valor padrão para **flex-direction** é **row**. Os elementos Flexbox têm esse valor mesmo que não o codifiquemos.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**flex-direction: row** significa que os itens começam do lado esquerdo do contêiner e são e são exibidos horizontalmente na ordem em que estão no HTML.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Podemos também definir **flex-direction** como **column**. Aqui, os itens começam no topo e são colocados verticalmente na ordem em que estão no HTML.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">1</div>
			<div class="item">2</div>
			<div class="item">3</div>
			<div class="item">4</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: column;
    height: 300px;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Quando **flex-direction** é definido como **column**, os elementos se estendem para preencher a **width** do contêiner.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">1</div>
			<div class="item">2</div>
			<div class="item">3</div>
			<div class="item">4</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: column;
    width: 200px;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```