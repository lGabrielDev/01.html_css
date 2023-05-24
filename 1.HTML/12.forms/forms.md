<h1 align="center">
    Formulários - &lt;form&gt;
    <img src="https://cdn-icons-png.flaticon.com/512/3273/3273589.png" alt="html icon" width="90px" align="center" >
</h1>

## Introduction

Um formulário é usado para coletar o input de dados de um usuário. Os elementos de um formulário são:

- `<form>` --> div semântica que representa nosso formulário.

- `<label>` --> Texto explicando o que o usuário deve inputar.

- `<input>` --> Input do usuário. Existem vários tipos de input.


:pencil2: Faça um formulário simples, onde o usuário vai inputar seu "first name".

```html
<form action="arquivo_para_armazenar">
    <label for="firstNameInput">First Name:</label> <br>
    <input type="text" name="firstNameInput" id="firstNameInput"> <br>
    <input type="submit" id="submitButton">
</form>
```

- Perceba que o element `<input>` sempre vêm acompanhado com os attributes `id` and `name`.

- Perceba que o element `<label>` têm sempre um `for` attribute que é vinculado ao `id` attribute do input. Assim, criamos uma conexão do input com a label.

:warning: Obviamente, o valor desse `for` attribute têm que ser igual ao valor do `id` attribute do input.


<br>

Vamos entender os attributes de cada elemento.

<br>
<hr>

## `<form>`
QUando estamos preenchendo um formulário, esses dados vão para algum lugar...

- `action` --> define o local para onde os dados desse input vãos ser armazenados. 
```html
<form action="arquivo1.txt"> 

</form>
```
<br>
<hr>

## `<label>`
Texto explicando o que o usuário deve inputar. O elemento `<label>` sempre vêm acompanhado do attribute `for`. Esse attribute faz conexão com o id do `<input>`.

```html
<label for="firstNameInput">First Name:</label>
<input type="text" name="firstNameInput" id="firstNameInput">
```
Fizemos uma conexão da label com o input.


<br>
<hr>

## `<input>`
Elemento usado para o usuário inputar dados.

- `<type>` --> Tipo de input (radio button, text, submit, etc...)
- `<name>` --> Obrigatório colocar
- `<id>` --> identificador padraozin de cada element.

:warning: O attribute name and id precisam ser iguais. Se não colocar o attribute `<name>` vai dar ruim.

<br>
<hr>

## `<select>`
Ao invés de inputar um dado, o usuário pode selecinar um dado em uma lista.

```html
<form action="caminhoDoArquivoParaSalvarOsDados">
    <label for="personagem">Escolha um personagem:</label>
    <!-- Lista de seleção -->
    <select name="personagem" id="personagem">
        <!-- Opções dentro da lista -->
        <option value="naruto">Naruto</option>
        <option value="sasuke">Sasuke</option>
        <option value="sakura">Sakura</option>
    </select>
    <input type="submit" id="submitButton">
</form>
```

Perceba que usamos o attribute `value`. Se quisermos usar algum method em javascript para retornar o valor desse input, retornamos esse `value`.

<hr>
<br>

## `<fieldset>` and `<legend>`
- `<fieldset>` --> Usado para separar seções do seu formulário.
- `<legend>` --> Título dessa seção.

```html
<form action="caminhoParaSalvarDadosInputados">
    <!-- Primeira seção do formulário -->
    <fieldset>
        <legend>Informações pessoais:</legend>
        <label for="firstNameInput">First Name:</label> <br>
        <input type="text" name="firstNameInput" id="firstNameInput"> <br>
        <label for="lastNameInput">Last Name:</label> <br>
        <input type="text" name="lastNameInput" id="lastNameInput"> <br>
    </fieldset>
    <!-- Segunda seção do formulário -->
    <fieldset>
        <legend> Informações do jogo: </legend>
        <label for="favoriteChampionInput">Favorite Champion:</label><br>
        <input type="text" name="favoriteChampionInput" id="favoriteChampionInput">
    </fieldset>
    <input type="submit" name="submitButton" id="submitButton">
</form>
```


<hr>
<br>

## Tipos de input

Existem vários tipos de input...

### `<input type="password">`
```html
<form action="caminhoParaSalvarDadosInputados">
    <fieldset>
        <legend>Sistema de login</legend>
        <label for="loginInput">Login:</label> <br>
        <input type="text" name="loginInput" id="loginInput"> <br>
        <label for="passwordInput">Password:</label> <br>
        <input type="password" name="passwordInput" id="passwordInput"> <br>
    </fieldset>
    <input type="submit" value="Enviar">
</form>
```

- Todo `input` element sempre vêm acompanhado dos attributes `name` and `id`.

:bulb: Use a ide (vsCode) a seu favor. `Input`...

<br>
<br>

## `<input type="radio">`
```html
<p>Escolha sua linguagem favorita:</p>
<form action="caminhoParaSalvarInput">
    <!-- choose java -->
    <input type="radio" name="favLanguage" id="javaInput" value="java">
    <label for="javaInput"> Java </label> <br>
    <!-- choose php -->
    <input type="radio" name="favLanguage" id="php" value="php">
    <label for="php"> Php </label> <br>
    <!-- choose ruby -->
    <input type="radio" name="favLanguage" id="javaInput" value="ruby">
    <label for="javaInput"> Ruby </label> <br>
    <input type="submit" value="Enviar">
</form>
```
:warning: O valor do attribute `name` de todos os radio inputs precisam ser iguais.

<br>
<br>

## `<input type="checkbox">`
```html
<p>Escolha os produtos que deseja comprar:</p>
<form action="arquivoParaSalvarInput">
    <!-- Produto 1 -->
    <input type="checkbox" name="pizza" id="pizza">
    <label for="pizza">Pizza</label> <br>
    <!-- Produto 2 -->
    <input type="checkbox" name="agua" id="agua">
    <label for="agua">Água</label> <br>
    <!-- Produto 3 -->
    <input type="checkbox" name="salgadinho" id="salgadinho">
    <label for="salgadinho">Salgadinho</label> <br>
    <!-- submit button -->
    <input type="submit" value="Enviar">
</form>
```

<br>
<br>

## placeholder Attribute
Escrevemos um valor no input para ajudar o usuário.

```html
<form action="arquivoTal">
    <label for="fullNameInput">Full name:</label><br>
    <input type="text" name="fullNameInput" id="fullNameInput" placeholder="João da Silva ....">
    <input type="submit" value="Enviar">
</form>
```

Existem vários outros tipos de input. Não precisa aprender todos... Quando precisar de um deles, estude.

<br>

- `<input type="button">`
- `<input type="checkbox">`
- `<input type="color">`
- `<input type="date">`
- `<input type="datetime-local">`
- `<input type="email">`
- `<input type="file">`
- `<input type="hidden">`
- `<input type="image">`
- `<input type="month">`
- `<input type="number">`
- `<input type="password">`
- `<input type="radio">`
- `<input type="range">`
- `<input type="reset">`
- `<input type="search">`
- `<input type="submit">`
- `<input type="tel">`
- `<input type="text">`
- `<input type="time">`
- `<input type="url">`
- `<input type="week">`

<a href="https://www.w3schools.com/html/html_form_attributes.asp" target="_blank">consulta</a>


<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../../2.CSS/0.introduction/introduction.md)