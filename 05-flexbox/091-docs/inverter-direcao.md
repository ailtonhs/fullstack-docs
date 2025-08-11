# Usando Flex Direction

## Inverter Direção

O Flexbox nos permite mudar o ponto de partida dos itens flex, permitindo que invertamos facilmente um layout, se necessário.

Para mudar a posição inicial dos itens flex para o lado direito de um contêiner, podemos usar **row-reverse**.

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
    flex-direction: row-reverse;
 
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**flex-direction: row-reverse** significa que os itens começam do **lado direito** do contêiner e são exibidos na ordem em que estão no HTML.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row-reverse;
 
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Se quisermos inverter a direção das coluna, podemos usar **column-reverse**.

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
    flex-direction: column-reverse;
   
 
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**flex-direction: column-reverse** significa que os itens começam a partir da **parte inferior** do contêiner e são exibidos na ordem em que estão no HTML.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: column-reverse;
   
 
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Ao usar **column-reverse**, a mudança se torna mais óbvia quando a altura do contêiner é maior do que a dos itens.

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
    flex-direction: column-reverse;
    height: 300px;
   
 
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```