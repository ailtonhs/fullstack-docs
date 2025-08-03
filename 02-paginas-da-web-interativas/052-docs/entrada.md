# Coletando Entrada

## Entrada

Em HTML, usamos o **elemento input** para obter todos os tipos de entrada do usuário, como e-mails, senhas, datas e mais.

Vamos aprender a usar entrada do usuário em um site mais tarde. Por enquanto, vamos nos concentrar em criar o elemento e definir seus atributos.

Criamos elementos de entrada usando a tag vazia **&lt;input&gt;**.

```html
<!doctype html>
<html>
    <body>
        <h4>Sign Up</h4>
        <input>
    </body>
</html>
```
O atributo **placeholder** sugere o que um usuário deve digitar no campo.

```html
<!doctype html>
<html>
    <body>
        <h4>Sign Up</h4>
        <input placeholder="Email">
        <br>

        <input placeholder="Password">
    </body>
</html>
```
Assim comoo botões, elementos de input precisam de uma tag ***lt;br&gt;** para colocar um abaixo do outro.

```html
<!doctype html>
<html>
    <body>
        <h4>Sign Up</h4>
        <input placeholder="Email">
        <br>

        <input placeholder="Password">
    </body>
</html>
```
O atributo **type** especifica o tipo de entrada. Por exemplo, podemos ocultar o que os usuário digitam para melhor segurança com **type="password"**.

```html
<!doctype html>
<html>
    <body>
        <h4>Sign Up</h4>
        <input type="text" placeholder="Email">
        <br>

        <input type="password" placeholder="Password">
    </body>
</html>
```

O valor padrão para o type é **text**, o que permite que os usuário insiram texto que podem ver.

```html
<!doctype html>
<html>
    <body>
        <h4>Sign Up</h4>
        <input type="text" placeholder="Email">
        <br>

        <input type="password" placeholder="Password">
    </body>
</html>
```

Não há necessidade de memorizar todos os tipos de input. Vamos te dar prática para os mais interessantes, como **range**, **checkbox**, **date** e **color**.


```html
<!doctype html>
<html>
    <body>
        <p>Range:</p>
        <input type="range">

        <p>Checkbox:</p>
        <input type="checkbox">

        <p>Date:</p>
        <input type="date">

        <p>Color:</p>

        <input type="color">
    </body>
</html>
```