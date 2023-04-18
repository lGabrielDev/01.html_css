<h1 align="center">
    CSS
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

<br>

### Estilizando pelo element selector
Quando queremos estilizar todos os elementos.
```css
p{text-align: center;}

h2{text-align: center;}
/* Estamos estilizando todos os parágrafos */
/* Estamos estilizando todos os h2 */
```
<br>
<br>

### Estilizando multiple elements
```css
h2, div, p{
    text-align: center;
}
/* Estamos estilizando todos os <h2>, todas as <div> e todos os <p> */
```
<br>
<br>

### Estilizando pelo id selector
Quando queremos estilizar apenas 1 elemento específico, estilizamos pelo `id`.
```css
#p_importante{text-align: center;}
```
:bulb: Usamos os character `#` para id.

<br>
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
:bulb: Usamos os character `.` para class.

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
<a href="https://github.com/lGabrielDev/01.html_css/blob/main/2.CSS/1.box_model/box_model.md">
    <img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">
</a>