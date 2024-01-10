<!-- title -->
<h1 align="center">
    <span>HTML semântico</span>
    <img src="https://cdn-icons-png.flaticon.com/512/3447/3447692.png" alt="html icon" width="90px" align="center" >
</h1>
 
 ## Introduction <img src="https://cdn-icons-png.flaticon.com/512/1436/1436664.png" alt="imagem" width="50px" align="center">
 Antigamente, o layout de uma página era feito com várias `<div>`. Assim, ficava muito difícil ler o código e entender a estrutura dessa página.

 Para facilitar, foi implementado o **HTML semântico**. Agora, ao invés de usar várias `<div>`, podemos usar semantic elements para cada parte da nossa página.

- `non-semantic` --> `<div>` and `<span>`
- `semantic` --> `<form>`, `<table>` , `<article>` , `<nav>`, etc... 

Os dois tipos de elementos fazem a mesma coisa, a diferença é na leitura do código que fica mais fácil.

<hr>
<br>

## Entendendo os elementos semânticos

O elementos semânticos mais usados são esses:

<img src="https://1.bp.blogspot.com/-koPDB__CnsU/Wobo6SpFXSI/AAAAAAAABTc/LR0ZB--5dJEpzLw7FHqzG-Fcep5FuO-qACLcBGAs/s1600/head%2Band%2Bfooter.jpg" alt="semantic html image" width="500px">

### `<section>`
São seções da minha página. 

<br>

### `<article>`
Conteúdo independente. Podemos ter várias `<section>` dentro desse artigo.

<br>

### `<header>`
Conteúdo introdutório de um section/article. Geralmente possui um heading (`<h2>`,`<h3>`,etc..) e navegation links (`<nav>`).
```html
<body>
    <header>
        <h1>Aprendendo html semântico</h1>
        <nav>
            <a href="#sectionTal"> Página inicial 
            <a href="#sectionTal"> Produtos mais vendidos 
            <a href="#sectionTal"> Produtos em promoção 
            <a href="#sectionTal"> Categoria 
        </nav>
    </header>
</body>
```

<br>

### `<nav>`
Bloco de links de navegação. Por exemplo, o menu da sua page.

<br>

### `<footer>`
Rodapé da section/article.

<br>

💡 As vezes, não vai ter um elemento semântico para usar. Nesses casos, vamos usar a `<div>` mesmo.

<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../12.forms/forms.md)