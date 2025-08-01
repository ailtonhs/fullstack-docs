# Como acessar um Elemento HTML

## Usando o Quey Selector

Se quisermos recuperar um elemento HTML individual, podemos usar o método **querySelector()** do **document**.

```html
<body>
<button onclick="publish()">Publish website</button>

<p>Website not published</p>

<script src="script.js"></script>
</body>
```
```js
function publish() {
    const el = document.querySelector();
}
```
Para selecionar um elemento específico, adicionamos um seletor dentro de parênteses. Podemos usar uma **tag** HTML, comoo a tag **p** se quisermos obter o parágrafo.

```js
function publish() {
    const el = document.querySelector("p");
}
```

Depois de armazenarmos o elemento em uma variável, podemos alterá-lo. 

Aqui, estamos usando a propriedade **innerHTML** para mudar seu conteúdo.

```js
function publish() {
    const el = document.querySelector("p");

    el.innerHTML = "Website published!";
}
```
**querySelector()** funciona com todos os seletores, como tags, classes e IDs, Se estivermos procurando por um ID, adicionamos o **#** no início.

```html
<button onclick="publish()">Publish website</button>

<p id="prompt">Website not published</p>

<script src="script.js"></script>
</body>
```
```js
function publish() {
    const el = document.querySelector("#prompt");

    el.innerHTML = "Website published!";
}
```
Se estamos procurando por uma classe, temos que adicionar **.** no início.

```html
<button onclick="publish()">Publish website</button>

<p class="prompt">Website not published</p>

<script src="script.js"></script>
</body>
```
```js
function publish() {
    const el = document.querySelector(".prompt");

    el.innerHTML = "Website published!";
}
```
**querySelector()** recupera apenas o **primeiro** elemento que encontra. 

Então, se tivermos dois elementos com a mesma tag ou classe, só acessamos o primeiro.

```html
<button onclick="publish()">Publish website</button>

<h3>First heading</h3>
<h3>Second heading</h3>
<h3>Third heading</h3>

<script src="script.js"></script>
</body>
```
```js
function publish() {
    const el = document.querySelector("h3");
    
    el.innerHTML = "Website ppublished!";
}

