# Justificando Grupos de Itens

Podemos usar Flexbox para justificar itens dentro de um contêiner pai.

Justificar significa mudar como os elemento são **agrupados** e **espaçados** no **eixo principal**. Para justificar itens flex, usamos a propriedade **justify-content**.

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
    justify-content: flex-start;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Por padrão, **justify-content** é definido como **flex-start**.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    justify-content: flex-start;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**flex-start** significa que todos os itens flex são agrupados no início do contêiner.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    justify-content: flex-start;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Para agrupar todos os itens no final do container, usamos **flex-end**.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    justify-content: flex-end;
    
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**justify-content** também funciona quando **flex-direction** está definido como **column**.

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
    height: 300px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Com **flex-direction** definido como **column**, **flex-end** significa que todo o conteúdo está agrupado na parte inferior do contêiner.

```css
.container {
    border: 2px solid #806868;
    height: 300px;
    display: flex;
    flex-direction: column;
    justify-content: end;
    
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```