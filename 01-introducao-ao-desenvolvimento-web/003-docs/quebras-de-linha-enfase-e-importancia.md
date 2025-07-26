# Estruturando Texto com Tags

## Quebras de linhas, ênfase e importância

## Quebras de linha 
Às vezes, queremos formatar parágrafos com quebras de linhas.
Podemos separar linhas com ajuda da tag de quebra de linha: **br**.

```html
<h1>My favorite things</h1>
<p> Raindrops on roses<br>

Whiskers on kittens<br> 
Bright copper kettles <br>
 
Warm woolen mittens
 </p>
 ```

 **&lt;br&gt;** é uma tag vazia. Tags vazias não possuem tag de fechamento nem conteúdo. Elas também são chamadas de tags de fechamento automático.

### Ênfase
 Há um elemento para dar ênfase ao texto, tornando-o itálico. Chama-se **em** elemento.

 ```html
 <h1>My favorite things</h1>
<p>
 Raindrops on <em>roses</em><br>
 Whiskers on kittens<br>
 Bright copper kettles<br>
 Warm woolen mittens
</p>
```

### Importância

Para definir como importantes, usamos as tags **&lt;strong&gt;** e **&lt;/strong&gt;**. Isso deixa o texto em negrito.

```html
<h1>My favorite things</h1>
<p>
 Raindrops on <em>roses</em><br>
 Whiskers on <strong>kittens</strong>
</p>
```