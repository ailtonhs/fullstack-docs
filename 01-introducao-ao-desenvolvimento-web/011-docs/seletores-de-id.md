# Folha de Estilo e Seletores Básicos

## Seletores de ID

Se quisermos estilizar um elemento específico, podemos incluir um seletor **id**. Aqui, queremos selecionar apenas o botão com a letra maiúscula.

Primeiro, precisamos identificar o elemento no HTML. Para definir um atributo de ID, digitando **id=""**.

```html

<!doctype html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <h1>Find the Capital Letter</h1>
  <button>x</button>
  <button>x</button>
  <button>x</button>
  <button id="">X</button>
  <button>x</button>
  <button>x</button>
  <button>x</button>
  <button>x</button>
  <p class="text">Click on the correct button!</p>
  <p class="text">Game on!</p>
 </body>
</html>
```

Após o sinal **=**, defina o valor do id, **"capital-letter"** neste caso.

Os valores de ID devem ser únicos dentro do documento HTML. Portanto, não devemos incluir um segundo atributo **id** com o mesmo valor.

```html
<!doctype html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <h1>Find the Capital Letter</h1>
  <button>x</button>
  <button>x</button>
  <button>x</button>
  <button id="capital-letter">X</button>
  <button>x</button>
  <button>x</button>
  <button>x</button>
  <button>x</button>
  <p class="text">Click on the correct button!</p>
  <p class="text">Game on!</p>
 </body>
</html>
```

Agora que incluímos o **id** no elemento HTML, estamos prontos para usar o seletor id para nossos estilos.

Para selecionar o elemento pelo seu id, digitamos **#** seguido do nome do id, como aqui **capital-letter**.

```css
button {
 background-color: lightblue;
 font-weight: bold;
}
.text {
 font-style: italic;
}

#capital-letter {
 
}

```
IDs nos ajudarão com JavaScript e não devemos usá-los em excesso para estilização. No entanto, podemos aplicar estilos normalmente com o seletor **id**.

```css
button {
 background-color: lightblue;
 font-weight: bold;
}
.text {
 font-style: italic;
}

#capital-letter {
 color: blue;
}
```