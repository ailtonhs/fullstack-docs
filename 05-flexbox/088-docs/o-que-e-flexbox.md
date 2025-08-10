# Entendendo o Flexbox

## O que é Flexbox?

Vamos aprender sobre flexbox, um dos recursos mais novos do CSS, e como ele nos ajuda a criar página web responsiva.

Flexbox oferece aos desenvolvedores muita flexibilidade que eles nunca tiveram antes. É uma habilidade essencial que permite fazer mais com menos código.

Com flexbox, os elementos se adaptam em tamanho para se ajustar perfeitamente em diferentes telas.

Para aplicar flexbox, primeiro temos que garantir que a página da web tenha um elemento pai com elementos filhos aninhados dentro.


```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<div>1</div>
		</div>
	</body>
</html>
```

O elemento pai é chamado de **flex container**. Neste exemplo, também daremos ao elemento o nome de classe **container**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div>1</div>
			<div>2</div>
			<div>3</div>
			<div>4</div>
		</div>
	</body>
</html>
```

```css
.container {
    border: 2px solid #806868;
}
```

Elementos dentro do contêiner flex são chamados de **itens flex**. Este são os elementos que mudarão de tamanho para se adaptar ao seu contêiner.

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
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Para aplicar flexbox aos itens dentro do container, adicionamos **display: flex;** ao container.

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

E esse é o primeiro passo! Se adicionarmos mais texto dentro dos itens flex, podemos vê-los se adaptando para caber em seu contêiner.

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