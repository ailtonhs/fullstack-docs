# Posicionamento Relativo

Vamos aprender como posicionar elementos em relação à sua posição original.

Podemos mudar a posição dos elementos usando a propriedade **position**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<p>He <strong>dropped</strong> the mic.</p>
	</body>
</html>
```
```css
p {
    background-color: #edbaa6;
}

strong {
    position: relative;
}
```
Quando definimos **position** como **relative**, mudamos a posição de um elemento em relação à sua **posição original** no fluxo normal.

```css
p {
    background-color: #edbaa6;
}

strong {
    position: relative;
}
```
Podemos empurrar o elemento **strong 30px** para longe do topo de sua posição original, codificando **top: 30x;**.

```css
p {
    background-color: #edbaa6;
}

strong {
    position: relative;
    top: 30px;
}
```
Além de **top**, podemos usar as propriedades **right**, **bottom** e **left** para posicionar elementos exatamente onde queremos.

```css
p {
    background-color: #edbaa6;
}

strong {
    position: relative;
    top: 30px;
    left: 60px;
}
```
Codar **left: 30px** significa que empurramos o elemento **30px** para longe da esquerda de sua posição normal.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<p>"I have spoken"<em>-Kuiil, the Mandalorian</em></p>
	</body>
</html>
```
```css
em {
    background-color: #ffecd2;
    position: relative;
    left: 30px;
}
```

O posicionamento **relativo** não altera o fluxo normal. Outros elementos age como se ele ainda estivesse lá.