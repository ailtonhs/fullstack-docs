# Exibindo Elementos

## Elementos Inline

**Fluxo normal** é a forma como os elementos são exibidos em uma página da web por padrão.

Por exemplo, cabeçalhos e parágrafos aparecem em sua própria linha, enquanto links e botões são agrupados na mesma linha.

A propriedade **display** decide se um elemento aparece ou não na mesma linha.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<a href="#">Accept</a>

		<a href="#">Decline</a>

		<a href="#">Maybe?</a>
</html>
```
```css
a {
    display: inline;
}
```

Para elemento **a**, o valor padrão da propriedade **display** é **inline**.

```css
a {
    display: inline;
}
```
**height** e **width** não funcionam em elementos **inline**. Em vez disso, eles mantêm o tamanho do conteúdo dentro deles.

```css
a {
    display: inline;
    width: 3000px;
    border: 3px solid #000000;
}
```

Exemplos de elementos inline incluem **a**, **em** e **strong**. Todos eles aparecem na mesma linha quando codificados um após o outro.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<a href="#">Links</a>

		<em>Emphasized text</em>

		<strong>Important text</strong>
</html>
```
Se vários elementos inline não cabem dentro da largura de seu elemento pai, os elementos mais ao final se movem para próxima linha.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<h3>Tags</h3>

		<a href="#">#learninghowtocodeisawesome</a>

		<a href="#">#workHardPlayHrd</a>

		<a href="#">#yolo</a>

		<a href="#">#tbt</a>

		<a href="#">#100DaysOfCode</a>
</html>
```

```css
a {
    display: inline;
    border: 1px solid gray;
}
```