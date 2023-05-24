<h1 align="center">
    CSS variables
    <img src="https://cdn-icons-png.flaticon.com/512/4215/4215538.png" alt="html icon" width="90px" align="center" >
</h1>

Para facilitar a manutenção do nosso código, é melhor usarmos variables para setar as cores do nosso CSS.


1. Criamos as variables dentro do seletor `:root`
   ```css
    :root {
        --corPrincipal: #1e90ff;
        --corSecundaria: #ffffff;
    }
   ```

2. Agora, é só chamar a propriedade que queremos setar a cor, e chamar a variable.

    ```css
    .container{
        color:var(--corPrincipal);
        background-color: var(--corSecundaria);
    }
    ```

:bulb: Criando variables ficam muito mais fácil dar manutenção no código. Ao invés de alterar a cor em cada selector, basta alterar o valor da variable no selector `:root`.


:bulb: É legal sempre definir as cores das sua page primeiro, criando as variables. Aí, é só atribuir essas varibles nas properties de cores(color,background-color,etc...).
<br>

:pencil2: Crie um `<p>` e altere a cor do texto e do background com variables.

```html
<body>
    <p class="destaque">Salve gurizada!</p>
</body>
```

```css
/* variables de cores */
:root{
    --textoPadrao: #2D4262;
    --backgroundPadrao: #D09683;
}

p.destaque{
    color: var(--textoPadrao);
    background-color: var(--backgroundPadrao);
}
```


<br>
<br>

<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../6.media_query_responsividade/media_query_responsividade.md)
