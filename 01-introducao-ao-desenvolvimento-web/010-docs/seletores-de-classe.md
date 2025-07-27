# Folha de Estilo e Seletores Básicos

## Seletores de Classe

Se houver vários elementos do mesmo tipo em uma página da web, seletores como **h1**, **h2** ou **p** alteram todos esses elemetos.

```html
<!doctype html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <h1>Not On Time Magazine</h1>
  <p> Always first with the last </p>
  <h2>Car Trends</h2>
  <p> Coal powered cars. The future? </p>
  <h2>Fashion Latest</h2>
  <p> Flared jeans </p>
 </body>
</html>
```

```css
h1 {
 font: "Arial";
 color: green;
}

h2 {
 font: "Arial";
 color: blue;
}

p {
 font: "Arial";
 font-weight: normal;
}
```

Se quisermos selecionar um ou mais elementos, podemos definir um atributo **class** para os elementos exatos que queremos alterar.

```html
<!doctype html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <ol> TO DO: <li class="gray-element">Floss</li>
   <li>Feed Cat</li>
   <li class="gray-element">Nap</li>
   <li>Plan holiday</li>
   <li class="gray-element">Order tea</li>
  </ol>
 </body>
</html>
```
Na folha de estilo, podemos definir uma nova regra de classe com um **.** seguido do nome da classe. Como aqui com **gray-element

```css

.gray-element {
 background-color: lightgrey;

}
```

As regras da classe serão aplicadas a todos os elementos que tenham esse atributo de classe no arquivo **html**.

As classes não são únicas, então podemos definir a mesma classe para vários elementos. Como aqui, por exemplo, com **class="gray-element"**.

```html
<!doctype html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <ol> TO DO: <li class="gray-element">Floss</li>
   <li>Feed Cat</li>
   <li class="gray-element">Nap</li>
   <li>Plan holiday</li>
   <li class="gray-element">Order tea</li>
  </ol>
 </body>
</html>
```

Para definir uma classe como seletor em CSS, adicione um ponto final seguido do nome da classe. Neste caso, é **.gray-element**.

```css
.gray-element {
    background-color: lightGray;
}
```