# Folha de Estilo e Seletores Básicos

## Seletores de Elementos

Se quisermos que um estilo seja aplicado à página inteira, podemos usar o seletor  **body**.

```css
body {

}
```

Definir a cor de fundo para **blue;** dentro da **body** regra define o fundo para todo o corpo.

```css
body {
    background-color: blue;
}
```

Estilos como **color: white;** quando definidos dentro da **body** regra serão aplicados a todos os elementos dentro da tag **body**.

```css
body {
    background-color: blue;
    color: white;
}
```
Podemos estilizar quantos elementos quisermos, desde que adicionemos um espaço entre as diferentes regras.

```css
body {
    background-color: blue;
    color: white;
}

h1 {
    font-family: Helvetica;
}
```

Usar a tag **body** é uma das maneiras mais fáceis de adicionar regras sobrepostas em elementos.

```css
body {
 background-color: cornSilk;
}

h1 {
 font-family: Helvetica;
 color: darkGray;
}

p {
 color: gray;
 font-weight: bold;
 font-family: cursive;
}
```