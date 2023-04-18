<h1 align="center">
    Block and Inline Elements
    <img src="https://cdn-icons-png.flaticon.com/512/207/207788.png" alt="html icon" width="90px" align="center" >
</h1>

Todos os elements por padrão já vêm com um valor de display.

- block
- inline

<hr>
<br>

## Block-level Elements
Quando criamos um block-level element, esse elemento pula uma linha, dá um espaçamento em cima e embaixo e ocupa toda a width disponível. Como se fosse um "bloco" mesmo.

- `<p>`
- `<div>`
- `<h1>`,`<h2>`,`<h3>`,etc...
- `<ol>`
- `<ul>`
- `<nav>`
- etc...

:pencil2: Crie um `<p>` e uma `<div>` e coloque uma borda.


```html
<body>
    <p> Salve </p>
    <div> div bolada </div>
</body>
```

```css
/* CSS */
p,div{
    border: 2px solid tomato;
}
```

Perceba que aconteceu todas as características acima:
- O elemento pulou uma linha
- Deu uma margin em cima e em baixo
- Ocupou toda a largura disponível

<br>

<img src="https://cdn-icons-png.flaticon.com/512/2810/2810051.png" alt="imagem" width="50px" align="left">

O block-level element mais conhecido é a `<div>`. Geralmente usamos ele como container para formatar outros elements.

<hr>
<br>

## Inline Elements
Quando criamos um elemento inline, ele permanece na mesma linha e ocupa apenas a largura necessária. O elemento mais comum é o `<span>`.

:pencil2: Crie um `<p>` com uma frase e dentro coloque um `<span>` para estilizar.

```html
<body> 
    <p>Salve <span>gurizada</span> bolada.</p>
</body>
```

```css
/* CSS */
span{
    background-color: lightblue;
    border: 1px solid black;
}
```

<br>

<img src="https://cdn-icons-png.flaticon.com/512/2810/2810051.png" alt="imagem" width="50px" align="left">

O inline element mais conhecido é o `<span>`. Geralmente usamos ele para estilizar parte de um texto.


<br>
<br>

<!-- Next page button-->
<a href="https://github.com/lGabrielDev/01.html_css/blob/main/1.HTML/9.class/html_class.md">
    <img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">
</a>

