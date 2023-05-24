<h1 align="center">
    Box Model (Modelo de caixa)
    <img src="https://cdn-icons-png.flaticon.com/512/4327/4327005.png" alt="html icon" width="90px" align="center" >
</h1>

Todo element tem um box model, contendo: <br>

<img src="https://miro.medium.com/max/640/1*sKnLrT1TtqWDZg7GWoBCow.webp" alt="box model iamge" width="350px" align="center">

- `margin` --> Área de fora da borda. Distância entre os elements.

- `border` --> Borda ao redor do padding e do content.

- `padding` --> Espaçamento entre a borda e o conteudo

- `content` --> conteúdo do elemento (texto,images,etc...)

<hr>
<br>


## border

### border shorthand
É interessante usarmos a `border` property shorthand.

Com essa shorthand, definimos as properties:
1. `border-width`
2. `border-style`
3. `border-color`

```css
.praticando{
    border: 2px solid tomato;
}
```
<br>

## border-radius
Arredonda as bordas

```css
.image_bolada{
    border: 2px solid tomato;
    border-radius: 50%;
}
```
:bulb: É legal usar para arredondar uma imagem.

<hr>
<br>

## margin
Vamos usar o `margin` shorthand:

### 2 values
```css
.praticando{
    margin: 20px 50px;
    border: 4px solid tomato;
    /* top and bottom margin --> 20px */
    /* right and left margin --> 50px */
}
```
<br>

### 1 value
Setamos todas as margin (top,right,bottom,left)

```css
.praticando{
    margin: 50px;
    border: 4px solid tomato;
}
/* 
margin-top:50px;
margin-right:50px;
margin-bottom:50px;
margin-left:50px;
*/
```

<hr>
<br>

## padding
Funciona igualzinho o `margin` shorthand. Setamos primeiro o top-bottom e depois o right-left.

`padding` shorthand:

### 2 values:
```css
.container{
    border: 3px solid tomato;
    padding: 50px 20px;
}
 /* top and bottom padding --> 50px */
/* right and left padding --> 20px */
```

<br>

### 1 value:
Setamos todos os padding (top,right,bottom,left)
```css
.container{
    border: 3px solid tomato;
    padding: 50px;
}
/* 
padding-top:50px;
padding-right:50px;
padding-bottom:50px;
padding-left:50px;
*/
```

<hr>
<br>

## Formatando um texto
Principais propriedades:

- `color`
- `background-color`
- `text-align`

### color
Setar a cor de um texto.

```css
.container{
    color: tomato;
}
```

<br>

### background-color
Setar a cor de fundo de um element.

```css
.container{
    background-color: #ec8572;
}
```

<br>

### text-align
Alinhar o texto de forma horizontal.

```css
.container{
    border: 3px solid tomato;
    text-align: center;
}
```

- `text-align: center`;
- `text-align: left`;
- `text-align: right`;

<br>

:bulb: Para remover a underline dos links, use o `text-decoration:none;`.

<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../2.fonts/fonts.md)