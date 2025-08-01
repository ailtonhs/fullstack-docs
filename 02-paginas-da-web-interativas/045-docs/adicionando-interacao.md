# Interagindo com Páginas da Web

## Adicionando Interação

Vimos como podemos adicionar JavaScript aos nossos HTML. Agora vamos usar as tags **script** para **interagir** com elementos HTML.

Para dizer aos elementos como responder, por exemplo, a um clique de botão, precisamso identificá-los.

Para identificar os elementos com os quais queremos interagir, podemos dar a cada um deles um **id** único.

```html
<!doctype html>
<html>
<head>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <h1>Secret Message</h1>

    <button>Show secret</button>

    <p id="secret">*********************</p>
</body>
</html>
```
```css
body {
    background-color: #000000;
    color: red;
}
```

Podemos acessar os elementos HTML da nossa página da web usando a palavra-chave **document.document** representa a nossa página da web.

Agora, para interagir com um elemento HTML, precisamos da instrução **document.getElementById()**.

```js
document.getElementById();
```
Dentro de **document.getElementById()** colocamos o ID do elemento com o qual queremos interagir, como **secret** aqui.

```js
document.getElementById("secret");
```
Página da web interativas frequentemente usam **botões** para reagir a cliques dos visitantes.

No entanto, sem mais informações, uma tag **button** é inútil. Para reagir a cliques de visitantes, uma tag **button** precisa do atributo **onclick**.

```html
<!doctype html>
<html>
<head>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <h1>Secret Message</h1>

    <button onclick>Show secret</button>

    <p id="secret">*********************</p>
</body>
</html>
```
O atributo **onclick** pode chamar funções quando um visitante clica no botão. Defina **onclick** como **show()**.

Nesta função podemos adicionar o código para acionar o comportamento que desejamos.

```html
<!doctype html>
<html>
<head>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <h1>Secret Message</h1>

    <button onclick="show()">Show secret</button>

    <p id="secret">*********************</p>

    <script src="script.js"></script>
</body>
</html>
```

Podemos usar a função **show** para mudar o conteúdo de um elemento, como seu texto, quando clicamos em um botão.

Primeiro, acesse o texto do **p** com a instrução **innerHTML**.

```js
function show() {
    document.getElementById("secret").innerHTML;

}
```

Agora que acessamos o texto do elemento **p**, podemos alterá-lo.

```js
function show() {
    document.getElementById("secret").innerHTML = "not telling you";

}
```
