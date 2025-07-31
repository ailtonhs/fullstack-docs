# Interagindo com Páginas da Web

## Incluindo JavaScript

Por trás de todo site dinâmico, há algum código JavaScript.

Para adicionar código JavaScript a uma página da web, começamos com as tags **&lt;script&gt;** e **&lt;/script&gt;**.

```html
<!doctype HTML>
<html>
<body>
    <script></script>
</body>
</html>
```

O elemento **script** é o último elemento antes da tag de fechamento **&lt;/body&gt;** na estrutura HTML.

```html
<!doctype HTML>
<html>
<body>
    <h3>Tweeter</h3>

    <script></script>
</body>
</html>
```

Semelhante ao CSS, usamos um arquivo separado para escrever JavaScript. Para fazer isso, incluímos um atributo **src** que vincula ao arquivo que queremos usar.


```html
<!doctype HTML>
<html>
<body>
    <h3>Tweeter</h3>

    <script src="script.js"></script>
</body>
</html>
```

No arquivo JS, podemos escrever JavaScript como **const username = "Lee";**.

```js
const username = "Lee";
```
O JavaScript é executado automaticamente quando a página da web é exibida.

```js
const username = "Lee";
const tweets = 50;
console.log(username);
```