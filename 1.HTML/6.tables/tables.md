<!-- title -->
<h1 align="center">
    <span>Tables</span>
    <img src="https://cdn-icons-png.flaticon.com/512/2824/2824181.png" alt="html icon" width="90px" align="center" >
</h1>

Para criar uma table no html é bem simples. Primeiro informamos que vamos criar uma table, e depois saimos setando linha por linha.

- `<table>` --> Container da table
- `<tr>` --> table rows
- `<th>` --> table headers
- `<td>` --> table data

```html
<!-- Criamos uma table -->
<table>
    <!-- Cabeçalho da table -->
    <tr>
        <th> Name </th>
        <th> Age </th>
        <th> Phone </th>
    </tr>
    <!-- Dados da table -->
    <tr>
        <td> Paulo </td>
        <td> 33 </td>
        <td> 55555 </td>
    </tr>
    <tr>
        <td> Amanda </td>
        <td> 27 </td>
        <td> 4444 </td>
    </tr>
    <tr>
        <td> Roberto </td>
        <td> 44 </td>
        <td> 99999 </td>
    </tr>
</table>
```

```css
/* CSS */ 
table,th,td{
    border: 1px solid black;
    border-collapse: collapse;
}

th{padding: 3px 16px;}

td{padding: 6px 4px;}
```
💡 Para juntar as bordas, use o  `border-collapse: collapse;`


<br>
<br>


<!-- Next page button-->
[<img src="https://cdn-icons-png.flaticon.com/512/5553/5553581.png" alt="next button icon" width="60px" align="right">](../7.lists/lists.md)