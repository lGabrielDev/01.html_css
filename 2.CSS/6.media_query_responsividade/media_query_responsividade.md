<h1 align="center">
    <span>@Media Query - Responsividade</span>
    <img src="https://img.icons8.com/?size=512&id=KttbKzBn2Ndi&format=png" alt="displays icons" width="140px" align="center">
</h1>


Media queries são usados para estilizar nossa página HTML em diferentes telas/displays de dispositivos (celular, table, computador, tv).


<br>
<hr>


## Syntax:

As mais usadas são:

```css
/* min-width */
@media screen and (min-width:1px){}

/* man-width */
@media screen and (max-width:1px){}
```


<br>
<hr>

## min-width

Aqui, tratamos primeiro com as **telas menores** e depois tratamos as maiores.

```css
/* Tratando as telas menores primeiro */

/* Telas a partir de 1px --> Celular */
@media screen and (min-width:1px){
    h2{
        color: red;
        font-size: 5em;
    }
}


/* Telas a partir de  300px --> Tablet */
@media screen and (min-width:300px){
    h2{
        color: purple;
        font-size: 3em;
    }
}

/* --> Tablest telas maiores */
/* --> Computador telas menores */
/* --> Computador telas maiores */
/* --> Tv... tec.. */
/* ... */
```

<br>
<br>
<br>

## max-width


Aqui, tratamos primeiro com as **telas maiores** e depois tratamos as menores.

```css
/* Tratando as telas maiores primeiro */


/* Telas até 500px --> TV */
@media screen and (max-width:500px){
    h2.title1{
        color: red;
        font-size: 2em;
    }
}


/* Telas até 300px --> Monitor Grande */
@media screen and (max-width:300px){
    h2.title1{
        color: purple;
        font-size: 4em;
    }
}


/* Telas até 200px --> Monitor pequeno */
@media screen and (max-width:200px){
    h2.title1{
        color: green;
        font-size: 4em;
    }
}

/* --> Tablest telas maiores */
/* --> Tablest telas menores */
/* --> Celular */
/* ... */
```

<hr>
<br>

## Especificando ainda mais o display/tela

```css
/* Telas de 300px a 500px */
@media screen and (min-width:300px) and (max-width:500px) {
    h2{
        font-size: 6em;
        color: red;
    }
}

/* Telas de 501px a 800px */
@media screen and (min-width:501px) and (max-width:800px) {
    h2{
        font-size: 2em;
        color: green;
    }
}
```

⚠️ As regras de cima ainda continuam... 

- Se você comecou com `min-width`, trate primeiro os celulares (telas menores).


- Se você comecou com `max-width`, trate primeiro as telas grandes.


<br>
<hr>

## Responsividade em landscape

Para trabalharmos com responsividade em dispositivos de lado (landscape), basta usarmos a propriedade `orientation:landscape`, e se quiser, especificar a width do disposito de lado.

Se seu celular tem 393 x 851... O landscape dele vai ter 851 x 393.


```css
@media screen and (orientation:landscape) and (min-width:851) and (max-width:393px){

}
```