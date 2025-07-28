# Definindo Tamanho e Bordas

## Bordas

Os elementos de uma página da web podem ter **bordas** ao redor deles.

Para fazer a borda aparecer, definimos o valor como **solid**

```css
.coupon {
    border: solid;
}
```
Podemos definir a largura de uma borda adicionando um número em pixels logo depois **solid**.

Aqui, podemos criar uma borda mais larga definindo sua largura como **10px**.

```css
.title {
    border: solid 10px;
}
```

Para definir a cor, vamos adicionar **red** no final o valor de border.

```css
.caution {
    border: solid 10px red;
}
```
**border-radius** é uma propriedade que arredonda os cantos de em elemento. Se definimos o raio como **10px**, a borda se curva **10px** antes do canto.

```css
p {
    border-radius: 10px;
    background-color: lightBlue;
    border: solid;
}
```

**border-radius** funciona em todos os elementos, até mesmo em imagens. É uma maneira fácil de fazer com que as imagens tenham uma ótima aparência em uma página da web.

```css
img {
    border-radius: 100px;
    border: solid 5px black;
}
```

Para transformar uma imagem em um círculo, definimos **boorder-radius** a largura com metade da imagem. Mas isso só funciona se a imagem for quadrada!

```css
img {
    height: 100px;
    width: 100px;
    border-radius: 50px;
}