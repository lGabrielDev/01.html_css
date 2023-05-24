<h1 align="center">
    Fonts
    <img src="https://cdn-icons-png.flaticon.com/512/8048/8048843.png" alt="html icon" width="90px" align="center" >
</h1>

## Introduction

Todas as fontes derivam de 3 fontes genéricas:

- `Serif` --> Tem uma curvinha no fim das extremidades da letra.
- `Sans-serif` --> Letras retas, sem serief.
- `Monospace` --> Todas as letras possui a mesma largura.

<img src="https://about.easil.com/wp-content/uploads/blog-graphic-02-800x284.png" alt="html icon" width="400px" align="center">

<br>

Para mudar a fonte de um texto, vamos usar a property `font-family.`

:warning: Além da fonte que você quer utilizar, coloque também uma font genérica (serif,sans-serif, monospace). Assim, se por algum motivo sua fonte não funcionar, usamos as genéricas.

```css
.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}
/* 
Perceba que colocamos várias fontes em cada seletor, onde a última fonte é uma fonte genérica.

Se não conseguir ler a primeiro fonte, rode a segunda fonte... Se não conseguir ler, rode a fonte genérica.
 */
```

<hr>
<br>

## font properties

- `font-family` --> Define qual vai ser a font.
- `font-weight` --> Define o peso da font(bold,normal,300,etc...). Uma fonte pode ter vários pesos.
- `font-size` --> Define o tamanho da font.

<hr>
<br>

## Importando uma font do google
Basta ir no google fonts, escolher a font que deseja e colar o command.

### Importando com HTML
Basta copiar o command e colar no `<head>`.
```html
<head>
    <!-- google font -->
    <link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Ranga:wght@400;700&display=swap" rel="stylesheet">
    <!-- CSS external -->
    <link rel="stylesheet" href="style.css">
    <title>Praticando</title>
</head>
```

<br>

### Importando com CSS
Basta copiar o command e colar no `arquivo CSS` ou no elemento `<style>`.
```css
/* google font - Inspiration */
@import url('https://fonts.googleapis.com/css2?family=Inspiration&display=swap');

```
É bem simples mesmo. Só copiar e dale.

<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../3.position/position.md)