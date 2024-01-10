<!-- title -->
<h1 align="center">
    <span>Flexbox</span>
    <img src="https://cdn-icons-png.flaticon.com/512/210/210561.png" alt="html icon" width="90px" align="center" >
</h1>

## Introduction <img src="https://cdn-icons-png.flaticon.com/512/1436/1436664.png" alt="imagem" width="50px" align="center">

Display flex é uma das formas para manipular/movimetar os elementos filhos de um container pai.

- display:block;
- display:inline;
- display:inline-block;
- `display:flex;`

Para alinhar os items dentro de um container, fazemos a movimentação desses items no propŕio container pai.

1. Setamos o display do container pai para `flex`. Assim, conseguimos movimentar todos os items filhos desse container.
2. Movimentamos esses filhos no próprio container com as properties:

   - `flex-direction` --> setamos o eixo principal / direção dos items (`row/column`)
   - `justify-content` --> alinha os items no eixo principal x (horizontal).
   - `align-items` --> alinha os items no eixo secundário y (vertical).
   - `flex-wrap` --> se os elementos não couberem no container, quebra a página e eles vão pra baixo. Se os items tiverem um tamanho maior que o container, eles ficariam espremidos.
   - `align-content` --> alinha no eixo secundário (y) os items que quebraram a página com o `wrap`.

<hr>
<br> 

## flex-direction
A primeira coisa que devemos fazer depois de declarar um container pai como `flex`, é setarmos a direção do eixo principal com o `flex-direction`.

- `row` --> Eixo principal é o x (horizontal)
- `row-reverse`
- `column` --> Eixo principal é o y (vertical)
- `column-reverse`


⚠️ Dependendo do valor que setarmos, as propriedades ficam ao contrário.

<hr>
<br>

## justify-content
Alinha os items no eixo principal

- `justify-content: center` --> centraliza no eixo principal.
- `justify-content: flex-start` --> no começo do eixo principal.
- `justify-content: flex-end` --> no final do eixo principal.
- `justify-content: space-around` --> space ao redor dos items. Como se tivesse uma margin ao redor.
- `justify-content: space-between;` --> space somente entre os items.


⚠️ Atenção! Dependendo do eixo principal, as propriedades vão inverter:

### flex-direction:row (eixo principal x):
- `justify-content`--> alinhamento na horizontal
- `align-items` --> alinhamento vertical

### flex-direction:column (eixo principal y):
- `justify-content`--> alinhamento na vertical
- `align-items` --> alinhamento horizontal


<hr>
<br>

## align-items
Alinha os items no eixo secundário

- `justify-content: center` --> centraliza no eixo secundário.
- `justify-content: flex-start` --> no começo do eixo secundário.
- `justify-content: flex-end` --> no final do eixo secundário.

<hr>
<br>

## flex-wrap
Se os items forem maior que o container, usamos o `flex-wrap` para movê-los para baixo. Assim, os items não ficam expremidos.

- `flex-wrap:nowrap` --> valor default. Os items continuam na mesma linha, expremidos.
- `flex-wrap:wrap` --> Os items que estão expremidos no final, são movidos para a pŕoxima linha.

<hr>
<br>

## align-content
Alinha os items que quebraram  no flex-wrap. O `align-content` só dá pra usar, quando usamos o flex-wrap.

- `justify-content: center` --> centraliza no eixo secundário.
- `justify-content: flex-start` --> no começo do eixo secundário.
- `justify-content: flex-end` --> no final do eixo secundário.
- `justify-content: space-around` --> space ao redor dos items. Como se tivesse uma margin ao redor.
- `justify-content: space-between;` --> space somente entre os items.

Basicamente, usamos o `align-content` para alinhar os elementos que quebraram no flex-wrap.

<hr>
<br>

## Relembrando

1. Setamos o container pai como `display flex.` Assim, podemos mover os items do container.
2. Setamos a direction do eixo principal com o `flex-direction`.
3. Alinhamos o eixo principal com o `justify-content`.
4. Alinhamos o eixo secundário com o `align-items`.
5. Quebramos os items que estão expremidos com o `flex-wrap`.
6. Alinhamos os items que quebraram no  `flex-wrap` com o `align-content`.

Se quisermos alinhar um elemento sozinho, usamos o `align-self`.


<br>

💡 Agora fica fácil centralizar os items na página. Basta usar o flexbox bolado!

```css
*{
    margin: 0px;
    padding:0px;
}

body{
    width: 100vw;  /* vw --> viewport width -- O body vai ocupar toda a width da tela */
    height: 100vh; /* vh --> viewport height -- O body vai ocupar toda o height da tela */
    display: flex;
    justify-content: center;
    align-items: center;
}
    /* Easy! */
```

<br>

Pratique jogando <a href="https://flexboxfroggy.com/"><img src="https://cdn.iconscout.com/icon/free/png-512/frog-face-animal-aquatic-33968.png?f=avif&w=256" alt="froggy icon" width="60px" align="center"></a> <img src="https://files.softicons.com/download/web-icons/stock-web-icons-by-snap2objects/png/128/arrow2.png" alt="arrow icon" width="60px" align="center"> 


<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../5.css_variables/css_variables.md)
