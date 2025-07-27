# Folha de Estilho e Seletores Básicos

## Vinculando Folhas de Estilo

Agora, passaremos a criar sites com ótima aparência com a ajuda de uma linguagem de estilos chamada CSS, abreviação de Cascading Style Sheets.

Para tornar páginas da web maiores mais gerenciáveis, podemos mover nosso CSS para uma **folha de estilo** ou um arquivo especial apenas para estilizar a página da web.

```html
<!doctype html>
<html>
 <head>
    <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <h1>Water Puns</h1>
  <p> Why does water never laugh at jokes? It's not a fan of dry
   humor. </p>
 </body>
</html>
```

Para incluir uma folha de estilo em um arquivo HTML, usamos o elemento **link**. **&lt;link&gt;** é um elemento vazio de fechamento automático e fica dentro do elemento **head** 

```html
<!doctype html>
<html>
 <head>
  
    <link>

 </head>
 <body>
  <h1>Water Puns</h1>
  <p> Why does water never laugh at jokes? It's not a fan of dry
   humor. </p>
 </body>
</html>
```
Para saber que tipo de arquivo incluir, a tag **link** de abertura precisa do atributo **rel** definido usando **rel="stylesheet"**.

```html
<!doctype html>
<html>
 <head>
  <link rel="stylesheet">
 </head>
 <body>
  <h1>Water puns</h1>
  <p>Why are rivers amazing roommates? They go with the flow. </p>
 </body>
</html>
```

Para especificar a localização da folha de estilo, defina o atributo **href** como **"style.css"**

```html
<!doctype html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
  <h1>Water Puns</h1>
  <p> Why are oceans so meticulous?<br> They like to be pacific. </p>
 </body>
</html>
```

Dentro do arquivo CSS, especificamos qual elemento estilizar com um seletor de tags. Selecione a tag **p**.

```css
p
```

Em seguida, adicionamos uma chave de abertura, **{**, seguida de uma chave de fechamento, **}**.

```css
p {

}
```

Agora, qualquer declaração que adicionamos será aplicada a todos os elementos **p** da página. Adicione a declaração **color: blue;**.

```css
p {
    color: blue;
}
```
Quando adicionamos **p {** seguido por **color:blue;** e então **}**, criamos uma regra CSS.

```css
p {
    color: blue;

}
```

Podemos adicionar outras declarações, como "**background-color: pink;** contando que estejam em outra linha".

```css
p {
    color: blue;
    background-color: pink;
}

