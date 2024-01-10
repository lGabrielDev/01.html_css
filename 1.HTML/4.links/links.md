<!-- title -->
<h1 align="center">
    <span>HTML Links - Hyperlinks <strong>&lt;a&gt;</strong></span>
    <img src="https://cdn-icons-png.flaticon.com/512/2696/2696513.png" alt="html icon" width="90px" align="center" >
</h1>

Um link serve para redirecionar para outra página html.



## Syntax <img src="https://cdn-icons-png.flaticon.com/512/1442/1442581.png" alt="curly braces icon" width="30px" align="center">
```html
clique <a href="https://google.com.br"> aqui </a>
```

💡 Perceba que o elemento `<a>` vem sempre acompanhado do attribute `href`, que é o caminho da página que vamos ser redirecionados.

<hr>
<br>

## The target attribute

- `_self` --> Abre a página na aba atual.
- `_blank` --> Abre a página em uma nova aba.


<hr>
<br>

## Usando uma imagem como link

```html
<a href="https://google.com.br">
    <img src="https://cdn-icons-png.flaticon.com/128/937/937456.png" alt="imagem" height="30px">
</a>
```

Padrãozin... Ao invés do usuário clicar em um texto, ele clica em uma imagem.


<hr>
<br>

## Linkando para um elemento específico
Basta linkarmos através do `id` do elemento.

- `#` --> id

```html
<p>Clique <a href="#c4">aqui</a> para ir para o capítulo 4.</p> <!-- Passando o caminho relativo -->
<p>Clique <a href="../4.links/teste.html#c4">aqui</a> para ir para o capítulo 4.</p> <!-- Passando o caminho absolute -->
<p> Capítulo 1 </p>
<p> Capítulo 2 </p>
<p> Capítulo 3 </p>
<p id="c4"> Capítulo 4 </p>
```


<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../5.images/images.md)