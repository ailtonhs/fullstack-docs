## Descobrindo Elementos Filhos

# Elementos Pai e Filhos

Aprendemos que o HTML usa algo chamado modelo de caixa. A questão é que tudo no HTML é considerado uma **caixa dentro de outra caixa**.

Quando adicionamos um elemento **&lt;div&gt;** em torno de outros elementos, colocamos uma caixa maior em torno de outra caixas.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<p>Prince George</p>
		</div>
	</body>
</html>
```
Porque o elemento **&lt;div&gt;** tem outro elemento aninhado dentro dele, nós o chamamos de **elemento pai**. O elemento **&lt;p&gt;** dentro dele é chamado de **elemento filho**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<p>Prince George</p>
		</div>
	</body>
</html>
```
Se adicionarmos mais dois parágrafos dentro do elemento **&lt;div&gt;**, teremos três elementos filhos dentro de um elemento pai.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div>
			<p>Prince George</p>
            <p>Princess Charlotte</p>
            <p>Prince Louis</p>
		</div>
	</body>
</html>
```
Quando estilizamos um elemento pai, existem algumas propriedades que afetam apenas o pai, como **border**, **padding**, **margin**.

```css
div {
    border: 3px solid lightGray;
}
```
mas outras propriedades, como **color**, são transferidas para os elementos filhos a partir de seu pai.

```css
div {
    border: 3px solid lightGray;
    color: brown;
}
```
Quando um elemento filho recebe uma propriedade de seu pai, chamamos isso de **herança**.

```css
div {
    border: 3px solid lightGray;
    font-weight: bold;
}
```
Não há uma regra rígida sobre quais propriedades são herdadas. Vamos aprender mais sobre como verificar quais são herdadas mais tarde.