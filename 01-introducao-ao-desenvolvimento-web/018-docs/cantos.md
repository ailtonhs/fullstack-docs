# Estilizando Cantos com uma linha

## Abreviação de margin e  border-radius com quatro valores

As abreviações funcionam com as propriedade **margin** e **border-radius**, possibilitando criar estilos interessantes com menos linhas de código.

Para definir as margens direita e esquerda em **15px** uma linha, podemos usar a abreviação de **margin**.

```css
button {
    margin: 0 15px 0 15px;
    width: 100px;
    height: 100px;
    border-radius: 15px;
    background-color: red;
    border: solid 5px dimGray;
}
```

Para adicionar margens superior e inferior, definimos o primeiro e o terceiro valor como **40px**.

```css
button {
    margin: 40px 15px 40px 15px;
    width: 100px;
    height: 100px;
    border-radius: 15px;
    background-color: red;
    border: solid 5px dimGray;
}
```
A propriedade **border-radius** com quatro valores arredonda os cantos no sentido horário, começando do canto superior esquerdo.

```css
img {
    border-radius: 30px 30px 30px 30px;
    width: 250px;
    height: 300px;
}
```
Podemos arredondar apenas o canto superior esquerdo alterando o primeiro valor para **50px** e deixando o restante com **0**.

```css
img {
    border-radius: 50px 0 0 0;
    width: 250px;
}
```
Para ir **border-radius** ao extremo, podemos definir um canto com o mesmo valor da altura ou largura, como **100px** neste caso.

```css
p {
    border-radius: 0 0 0 100px;
    width: 100px;
    height: 100px;
    background-color: lightBlue;
    text-align: center;
}
```
Podemos **border-radius** dar um toque único às imagens fazendo coisas como arredondar os cantos superior direito e inferior esquerdo para **20px**.

```css
img {
    border-radius: 0 20px 0 20px;
    width: 75px;
    height: 75px;
}
```