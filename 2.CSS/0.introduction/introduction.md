<!-- title -->
<h1 align="center">
    <span>CSS</span>
    <img src="https://cdn-icons-png.flaticon.com/512/3308/3308160.png" alt="html icon" width="90px" align="center" >
</h1>

CSS --> Cascading Style Sheets (Folhas de estilo em cascata)

Usamos o CSS para estilizar nossas páginas.

<br>

## Syntax <img src="https://cdn-icons-png.flaticon.com/512/1442/1442581.png" alt="curly braces icon" width="30px" align="center">

<img src="https://www.w3schools.com/css/img_selector.gif" alt="css syntax image" width="470px">

<br>

- `selector` --> É o elemento/id/class que queremos estilizar.
- `declaration block {}` --> Bloco de declaração contendo uma propriedade e um valor.
- `property` --> Tipo de estilo que queremos colocar.
- `value` --> Valor dessa propriedade.

```css
p{
    /* declaration 1 */
    background-color: tomato;
    /* declaration 2 */
    color: black;
    /* declaration 3 */
    border: 2px solid black;
}
```

- `p` --> selector que queremos estilizar
- `background-color` --> property | `tomato` --> value
- `border` --> property | `2px solid black` --> value

<hr>
<br>

## Selectors
Como vimos antes, os seletores são os elementos que queremos estilizar. Podemos estilizar os seletores de várias formas:


### Estilizando pelo element selector
Quando queremos estilizar todos os elementos.
```css
p{text-align: center;}

h2{text-align: center;}
/* Estamos estilizando todos os parágrafos */
/* Estamos estilizando todos os h2 */
```
<br>

### Estilizando multiple elements
```css
h2, div, p{
    text-align: center;
}
/* Estamos estilizando todos os <h2>, todas as <div> e todos os <p> */
```

<br>

### Estilizando pelo id selector
Quando queremos estilizar apenas 1 elemento específico, estilizamos pelo `id`.
```css
#p_importante{text-align: center;}
```
💡 Usamos os character `#` para id.

<br>


### Estilizando pela class selector
```css
.p_destacados{
    text-align: center;
    border: 2px solid black;
    width: 300px;
    height: 200px;
}
/* todos os elements que tiverem a class "tal" vão ser estilizados */
```
💡 Usamos o character `.` para class.

<br>

Podemos também especificar quais elements dessa class vão ser estilizados

```css
p.p_destacados{
    text-align: center;
    border: 2px solid black;
    width: 300px;
    height: 200px;
}
/* Vamos estilizar todos os <p> que tiverem a class tal */

div.p_destacados{
    text-align: center;
    border: 2px solid black;
    width: 300px;
    height: 200px;
}

/* Vamos estilizar todas as <div> que tiverem a class tal */
```

<br>

### Estilizando os filhos diretos de um elemento:

```html
<div class="container">
    <p>item 1</p>
    <p>item 2</p>
    <p>item 3</p>
    <ol>
        <p>item 4</p> <!-- Nao é filho direto, nao vai ser alterado -->
    </ol>
</div>
```

```css
div > p{ /* Queremos estilizar todos os 'p' que forem filhos diretos de div */
    background-color: tomato;
}
```

<br>


### Estilizando todos os elementos dentro de um elemento:

```html
<div class="container">
    <p>item 1</p>
    <p>item 2</p>
    <p>item 3</p>
    <ol>
        <p>item 4</p> <!-- Ele também vai ser alterado, porque está dentro da div. Por mais que nao seja filho direto, ele ainda está dentro da div -->
    </ol>
</div>
```

```css
div p{ /* Queremos estilizar todos os 'p' que estiverem dentro de uma 'div' */
    background-color: tomato;
}
```

<hr>
<br>

## CSS colors
As 3 melhores formas de colocar o valor de uma cor, são:

- `Color Names` (tomato,Orange,Blue,etc...)
- `RGB Colors` --> rgb(red, green, blue)
- `hexadecimal colors` --> #RRGGBB

<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../1.box_model/box_model.md)