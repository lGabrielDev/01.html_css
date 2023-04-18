<h1 align="center">
    Images &lt;img&gt;
    <img src="https://cdn-icons-png.flaticon.com/512/2659/2659360.png" alt="html icon" width="90px" align="center" >
</h1>

Para usar uma image, basta usarmos a tag `<img>`. Essa tag sempre vêm acompanhada dos attributes `src` and `alt`

- `src` --> source. Qual a fonte em que essa imagem está.
- `alt` --> Valor alternativo. Se essa imagem por algum motivo não aparecer, será mostrado esse textinho. Serve como acessibilidade para pessoas com problemas visuais.

```html
<img src="https://cdn-icons-png.flaticon.com/512/2659/2659360.png" alt="ícone de uma fotografia">
```

<hr>
<br>

## width and height attribute
Esses attributes definem o tamanho da imagem. A largura e a altura.

```html
<img src="https://cdn-icons-png.flaticon.com/512/2659/2659360.png" alt="ícone de uma fotografia" width="200px" height="300px">
```

:bulb:Outra forma de definir a width and height é estilizar com css. Essa forma é bem melhor.

```html
<img src="https://cdn-icons-png.flaticon.com/512/2659/2659360.png" alt="ícone de uma fotografia" style="width:200px; height:400px">
```

<hr>
<br>


## faveicon
A faveicon é o ícone que aparece na aba da sua página.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
    <!-- ícone na aba da página -->
    <link rel="shortcut icon" href="https://cdn-icons-png.flaticon.com/512/2822/2822342.png" type="image/x-icon">
</head>
<body>
    <p>Salve quebrada</p>
    <h2>Teste</h2>
</body>
</html>
```
:bulb: Use a IDE (vsCode) a seu favor. Escreva `link` e dale.


<hr>
<br>

<h2>Diferença entre PNG e JPGE</h2>


**JPGE**
- Arquivo mais leve.
- Não possui transparência.
- Qualidade não é tão boa.



**PNG**
- Arquivo mais pesado.
- Permite transparência.
- Qualidade é melhor quando damos zoom.

<br>

⚠️ Atenção com o direito de imagem. Trabalhe sempre com images com permissão de utilização.


<br>
<br>

<!-- Next page button-->
<a href="https://github.com/lGabrielDev/01.html_css/blob/main/1.HTML/6.tables/tables.md">
    <img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">
</a>