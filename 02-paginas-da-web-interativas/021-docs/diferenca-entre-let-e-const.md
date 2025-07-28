# Criando Variáveis

## Diferenças entre Let e Const

Já sabemos que podemos declarar variáveis com **let** e **const**. Vamos descobrir a diferença entre eles!

Usamos **const** para declarar variáveis cujos valores não devem mudar. **const** é a abreviação de "constante".

```js
const norwayCapital = "Oslo";
```

Se tentarmos atualizar um valor armazenado em uma variável **const**, receberemos um erro.

```js
const age = 90;
age = 91; //TypeError
```

No entanto, podemos atualizar variáveis **let** com o operador de atribuição **=**

```js
let age = 90;
age = 91;
```
Para deixar claro que uma variável é do tipo **const** e não deve mudar, podemos opcionalmente nomeá-la com letras maiúsculas.

```js
const BIRTHDAY = "25/02/1882";
```

Não podemos usar **camelCase** se usarmos este padrão de maiúsculas, então usamos um **snake_case** em maiúsculas para nomear variáveis com mais de uma palavra.

```js
const SPEED_OF_LIGHT = "3*18 m/s";
```
Ambos **let** e **const** são variáveis úteis e poderíamos usá-los de forma intercambiável. No entanto, devemos tentar usar **const** como padrão.

```js
const MIDDLE_NAME = "Francesca";
```