# Adicionando Preenchimento com uma Linha

## Abreviação de Preenchimento

Qualquer elemento tem quatro preenchimentos contados no sentido horário, de cima para a direita, para baixo e para a esquerda.

Até agora, aprendemos a definir o preenchimento para cada lado de um elemento, um de cada vez.

```css
img {
    padding-top: 20px;
    padding-right: 20px;
    padding-bottom: 20px;
    padding-left: 20px;
    border: solid 2px gray;
    width: 100px;
    height: 100px;
    background-color: white;
}
```
Podemos definir cada valor de preenchimento em uma linha usando a propriedade **padding** e um valor em pixel para cada lado.

```css
img {
    padding: 20px 20px 20px 20px;
    width: 100px;
    height: 100px;
    background-color: white;
}
```
Para posicionar o conteúdo mais abaixo dentro de um elemento, adicione um preenchimento superior definindo o primeiro valor como **100px**.

```css
img {
    padding: 100px 0px 0px 0px;

    border: solid 2px gray;
    width: 100px;
    height: 100px;
    background-color: white;
}
```

Para definir o preenchimento direito como **40px**, alteramos o segundo valor. Para definir o preenchimento esquerdo como **100px**, alteramos o quarto valor.

```css
img {
    padding: 0px 40px 0px 100px;
    border: solid 2px gray;
    width: 100px;
    height: 100px;
    background-color: white;
}
```
Para adicionar preenchimento na parte inferior, defina o terceiro valor como **100px**.

```css
img {
    padding: 0px 0px 100px 0px;
    border: solid 2px gray;
    width: 100px;
    height: 100px;
    background-color: white;
}
```

Quando não queremos adicionar preenchimento a um lado, podemos adicionar **0** e omitir, **px** pois é opcional.

```css
img {
    padding: 0 0 0 100px 0;
    border: solid 2px gray;
    width: 100px;
    height: 100px;
    background-color: white;
}
```