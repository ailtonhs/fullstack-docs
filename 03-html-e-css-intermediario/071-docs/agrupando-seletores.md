# Agrupando Seletores

## Múltiplos seletores

Às vezes, queremos aplicar as mesmas propriedades em vários elementos. Como definir o mesmo **font-family** para todos os botões e parágrafos.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h2>Brand New Courses</h2>

		<p>Leran CSS today!</p>

		<button class="offer">FREE LESSON</button>
</html>
```
```css
p {
    font-family: 'Courier New';
}

button {
    font-family: 'Courier New';
}

.offer {
    font-size: 30px;
}
```

Em vez se escrever uma nova regra para cada elemento, podemos usar uma vírgula para estilizar os elementos **&lt;p&gt;** e **&lt;button&gt;** usando a mesma regra.

```css
p, button {
    font-family: 'Courier new';
}

.offer {
    font-size: 30px;
}
```
**p**, **button** é chamado de **seletor de agrupamento** pois agrupa diferentes elementos sob uma única regra.

```css
p, button {
    font-family: 'Courier new';
}

.offer {
    font-size: 30px;
}
```

Podemos adicionar seletores de qualquer tipo. Por exemplo, podemos usar o seletor de classe **.offer** em vez do seletor **button**.

```css
p, .offer {
    font-family: 'Courier new';
}

.offer {
    font-size: 30px;
}
```

Podemos adicionar quantos seletores quisermos. Tente adicionar outro codificando, **h2**.

```css
p, .offer, h2 {
    font-family: 'Courier new';
}

.offer {
    font-size: 30px;
}
```