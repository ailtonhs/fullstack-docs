# Construindo Lista

## Listas Ordenadas

**Listas** em HTML são muito parecidas com listas de compras ou de tarefas. Elas são uma excelente ferramenta para organizar informações em uma página da web.

Um tipo de ista é uma **lista ordenada**.

Uma lista ordenada exibe uma lista de itens numerados.

Uma lista ordenada é feita com as tags **&lt;ol&gt;** e **&lt;/ol&gt;**. A letra **O** significa **"ordered"** e a letra **L** significa **"list"**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<ol>
			
		</ol>

	</body>
</html>
```
Para adicionar um **item de lista**, adicionamos texto entre as tags **&lt;li&gt;** e **&lt;/li&gt;**. Neste caso, o **L** significa **"list"** e o **I** significa **item**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<ol>
			<li>Tortoise</li>
		</ol>

	</body>
</html>
```
Para que as lista sejam exibidas corretamente, os itens da lista precisam estar dentro do elemento de lista ordenada.

```html
    <ol>
		<li>Tortoise</li>
	</ol>
```
Listas podem ter qualquer número de itens. Para adicionar à lista, coloque itens adicionais entre as tags **&lt;ol&gt;** e **&lt;/ol&gt;**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
	</head>
	<body>
		<ol>
			<li>Tortoise</li>
            <li>Hare</li>
		</ol>
	</body>
</html>
```