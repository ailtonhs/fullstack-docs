# Criando Links
## Links e Atributos

Para começar a criar um link, adicionamos o texto entre as tags **&lt;a&gt;** e **&lt;/a&gt;. Isso ainda não destacará o texto.

```html
<a>Learn to Code</a>
```

Para vincular o  texto a uma página da web, adicionamos **href=""** junto um Uniform Resource Locator **(URL)**. **href** é a abreviação de "referência de hipertexto".

```html
<a href="https:caminho.com">Learn to Code</a>
```

**href** é um **atributo**. Todos os atributos têm duas coisas em comum: fornecem informações extras e ficam dentro da tag de abertura.

```html
<a href="https:caminho.com">Learn to Code</a>
```

Criamos um link para uma página da web adicionando **=** depois do atributo um URL com um valor entre aspas.

```html
<!DOCTYPE html>
<html>
<body>
    <a href="https:www.google.com">Learn to Code</a>
</body>
</html>
```