# Estilizando Texto

## Propriedades da fonte

Umas das partes mais importantes de um site é o texto. Podemos modificá-lo de diversas maneiras, desde o tamanho até o estilo ou a espessura.

Vamos começar criando uma regra para alterar a aparência dos nossos parágrafos.

```css
p {

}
```

Para alterar o tamanho do texto, usamos a propriedade **font-size**.

```css
p {
    font-size:
}
```
Medimos elementos em uma página da web com pixels. Para especificar um tamanho, adicionamos um número.

Após o número, seguimos com a abreviação para pixels, **px**.

```css
p {
    font-size: 60px;
}
```

Para definir o tipo de fonte de um elemento, comece adicionando a propriedade **font-family**.

Existem todos os tipos de valores possíveis para **font-family**, de **Times New Romam** até **Helvetica**. Aqui, vamos usar **Courier New**.
```css
p {
    font-size: 60px;
    font-family: "Courier New";
}
```

Para colocar o texto de um elemento em itálico, usamos a propriedade **font-style** e definimos o valor como **italic**.

```css
p {
    font-size: 60px;
    font-family: Arial;
    font-style: italic;
}
```

Para colocar o texto de um elemento em negrito, usamos a propriedade **font-weight** e definimos o valor como **bold**.

```css
 p {
    font-size: 60px;
    font-family: Arial;
    font-style: italic;
    font-weight: bold;
 }

