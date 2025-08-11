# Eixos do Flexbox

## Eixo Principal

Web site é composta por todos os tipos de sites diferentes de todo o mundo que estão em diferentes idiomas.

Flexbox é um recurso mais recente do CSS projetado para funcionar da mesma forma para uma comunidade global de desenvolvedores e usuários da web.

Os sites podem exibir conteúdo da esquerda para direita, de cima para baixo ou de muitas outras maneiras.

O Flexbox é projetado para ser adaptável a qualquer um desses casos de uso.

Ao usar flexbox, tentamos descrever layouts de acordo com onde os itens flexíveis **começam** e **termina** como base na **direção do flex**.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="container">
			<div class="item">1</div>
			<div class="item">2</div>
			<div class="item">3</div>
			<div class="item">4</div>
		</div>
	</body>
</html>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row-reverse;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

O **flex-direction** define o que é conhecido como o **eixo principal**, uma linha imaginária que se refere à direção e orientação dos itens flexíveis.

Nos sites em que estamos trabalhando, **flex-direction: row** significa que o eixo principal é horizontal, começa da esquerda e termina à direita.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

**flex-direction: row-reverse** significa que o eixo principal é horizontal, mas agora começa da direita e termina no lado esquerdo.

```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: row-reverse;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```

Para definir o eixo vertical como o eixo principal, podemos definir **flex-direction** como **column** ou **column reverse**.

**fle-direction: column** significa que o eixo principal é vertical, começa do topo e termina na parte inferior.


```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: column;
    height: 300px;
}

.item {
    border: 2px solid #457081;
    margin: 10px;
}
```