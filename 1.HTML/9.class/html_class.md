<h1 align="center">
    class attribute
    <img src="https://cdn-icons-png.flaticon.com/512/1357/1357616.png" alt="html icon" width="90px" align="center" >
</h1>

O `class` attribute serve para especificar qual é a class que aquele elemento pertence.

Se temos elementos que fazem parte da mesma class, conseguimos formatá-los através da class. 

Se tívermos trabalhando com javascript, podemos criar um method para modificar todos os elementos de tal class.

O character que representa o attribute "class" é `.`

- `.` --> class
- `#` --> id


<hr>
<br>

## Formatando todos os elementos da mesma class
### Exemplo 1:

:pencil2: Crie 3 `<div>` e adicione a mesma classe pra elas. Depois, faça uma estilização no css através da class que elas têm em comum.

```html
<body>
    <div class="div_destacada">
        <p>Salve gurizada</p>
    </div>
    
    <div class="div_destacada">
        <p>Salve gurizada</p>
    </div>

    <div class="div_destacada">
        <p>Salve gurizada</p>
    </div>
</body>
```

```css
/* CSS */
.div_destacada{
    padding: 5px 5px;
    margin: 10px 10px;
    border: 2px solid tomato;
}
```
Viu?? Todos os elements da class "div_destacada" sofreram alteração. Quando queremos que vários elementos tenham a mesma formatação, basta colocarmos eles na mesma class.

<br>
<br>

## Exemplo 2:

:pencil2: Crie um `<p>` com uma frase grande. Formate alguma palavras utilizando o elemento `<span>`. Como queremos a mesma formatação, vamos estilizar através da class.

```html
<body>
    <p> Lorem ipsum <span class="palavraDestacada">dolor</span> sit amet consectetur <span class="palavraDestacada">adipisicing</span> elit. Corporis eius <span class="palavraDestacada">suscipit</span> voluptates.</p>
</body>
```

```css
/* CSS */
span.palavraDestacada{
    color: red;
    background-color: rgba(179, 106, 106, 0.312);
}
```

Se ligou?? Estamos formatando todos os elements `<span>` que tenham a class "palavraDestacada"

<hr>
<br>

## Multiple classes
Um elemento pode receber mais de uma class

:pencil2: Crie 2 classes:
- Uma class para estilizar a cor do elemento
- Uma class para aumentar a fonte do elemento

```html
<body>
    <p class="palavraDestacada">Salve</p>
    <p class="palavraGrande">Salve</p>
    <p class="palavraDestacada palavraGrande">Salve</p>
</body>
```

```css
/* CSS */
.palavraGrande{
    font-size: 25px;
}

.palavraDestacada{
    color: red;
}
```

Perceba que o último `<p>` sofreu as duas formatações. Isso, porque ele pertence as duas classes.

<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../10.html_id/id.md)