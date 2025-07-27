# Adicionando Imagens

# Imagens

Para adicionar **imagens** a uma página da web, começamos com a tag **&lt;img&gt;**.

```html
<h3>Drawing of <em>Earthise</em></h3>
<img>
```
Assim como **&lt;br&gt;**, **&lt;img&gt; é uma tag vazia. Isso significa que ela não tem uma tag de fechamento.

```html
<h3>Drawing of <em>Earthise</em></h3>
<img>
```

Para exibir uma imagem, uma tag de imagem precisa do atributo **src**. **src** significa fonte.

```html
<h3>Drawing of <em>Earthise</em></h3>
<img src="https://font.app.png">
```

Definimos a imagem que queremos exibir com um sinal **=** e o endereço da imagem entre aspas duplas.

```html
<h3>Drawing of <em>Earthise</em></h3>
<img src="caminho-imagem.png">
```

Podemos usar atributo para alterar o tamanho das imagens. Os atributos **width** e **height** usam pixels como unidade de medida padrão.

```html
<h3>Drawing of <em>Earthise</em></h3>
<img src="caminho-imagem.png" width="200" height="200">
```

E o **height** atributo ajusta a altura de uma imagem.

```html
<h3>Drawing of <em>Earthise</em></h3>
<img src="caminho-imagem.png" width="200" height="300">
```