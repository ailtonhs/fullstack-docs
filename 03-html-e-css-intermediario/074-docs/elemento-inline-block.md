# Exibindo Elementos

## Elementos Inline-block

Você pode ter notado que botões e imagens são exibidos de forma diferente dos elementos **inline** ou **block**.

Elementos como **button** e **img** têm **inline-block** como seu valor padrão de **display**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<button>Open Catalogue</button>
		<button>Create Your own</button>
	</body>
</html>
```
```css
button {
    display: inline-block;
}
```

**inline-block** coloca elementos na mesma linha, enquanto também nos permite alterar seu tamanho.

```css
button {
    display: inline-block;
    height: 50px;
    width: 120px;
}
```

Podemos definir a propriedade **display** de um elemento para um valor diferente quando queremos mudar como eles aparecem e se comportam em uma página web.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<p>The <em>drop</em>.</p>
	</body>
</html>
```
```css
em {
    display: inline-block;
    background-color: #efa536;
    height: 100px;
}
```