# Código Padrão
## Cabeçalho, Título e Doctype

### Head
O **head** elemento HTML, **&lt;head&gt;&lt;/head&gt;**, é um contêiner para informações sobre uma página da web, como seu título. Ele vem antes da tag body.

```html
<html>
<head>

</head>
 <body>
  <h1>My favorite things</h1>
  <p> Raindrops on <em>roses</em><br> Whiskers on
   <strong>kittens</strong>  </p>  
 </body>
</html>
```
### Title
O **título** de uma página da web aparece na aba ou janela do navegador da web. Para dar um título a uma página da web, adicionamos **&lt;title&gt;** e **&lt;/title&gt;** dentro das tags head.
Observe que o **title** não é visível, mas fornece informações ao navegador.

```html
<html>
<head>
   <title>My webpage</title>

</head>
<body>
  <h1>My favorite things</h1>
  <p>
  Raindrops on <em>roses</em><br>
  Whiskers on <strong>kittens</strong> 
  </p>
</body>
</html>
```
## Doctype
O **doctype** informa ao navegador qual verão do HTML estamos usando. Sem ele, o navegador pode não exibir a página corretamente. Como estamos usando a versão mais recente, usamos **&lt;!doctype html&gt;**

```html

<!doctype html>
<html>
 <head>
  <title>My webpage</title>
 </head>
 <body>
  <h1>My favorite things</h1>
  <p> Raindrops on <em>roses</em><br>Whiskers on
   <strong>kittens</strong></p>  
 </body>
</html>
```