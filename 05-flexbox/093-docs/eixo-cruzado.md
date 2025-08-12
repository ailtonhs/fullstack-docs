# Eixos do Flexbox

## Eixo Cruzado

Até agora, estabelecemos que o **eixo principal** é baseado em **flex-direction**.

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

Os containers Flexbox também têm um **eixo cruzado**, que é uma linha imaginária perpendicular ao eixo principal.

A propriedade **flex-direction** denota o eixo principal. Assim, com **flex-direction: row**, o **eixo principal** será horizontal e o **eixo transversal** vertical.

Ao usar **row** ou **row-reverse** como a propriedade **flex-direction**, podemos tornar o eixo transversal vertical.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
    height: 100px;
}
```

Se adicionarmos uma altura aos itens e ao container, podemos ver que o eixo transversal para **row** e **row-reverse** começa na parte superior e termina na parte inferior.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row-reverse;
    height: 200px;
    
}

.item {
    border: 2px solid #457081;
    margin: 10px;
    height: 50px;
}
```

Para **column** e **column-reverse**, o eixo transversal é sempre horizontal.

Se adicionarmos largura aos itens, podemos ver que o eixo transversal para **column** e **column-reverse** começa à esquerda e termina à direita.

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
    align-items: flex-start;
    height: 300px;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
    width: 150px;
}
```

