# Create HTML Table

The HTML table tag allows you to arrange data like text, images, links in rows and columns of cells. Tables begin with a `<table>` tag and end with a `</table>` tag. Each row is between `<tr> ... </tr>`. Each cell or data point is between `<td> ... </td>` tags. If you want a table header for the first row then use `<th> ... </th>` instead of `<td> ... </td>`.

**Note:**  It is not considered appropriate to use tables to create rows and columns to render content layout. This is because screen readers assume tables contain data and read them row by row. Did you use tables for format your fabulous three column newsletter about wine? It will sound like you had to much of it to the person viewing your site with a screen reader.

Example table:

```markup
<table border="1" style="width:100%"  cellpadding="1" cellspacing="1">
  <thead>
  <tr><th>Year</th><th>Make</th><th>Model</th><th>Color</th></tr>
  </thead>
  <tbody>
  <tr><td>1999</td><td>Chevy</td><td>Corvette (small)</td><td>Red</td></tr> 
  <tr><td>1981</td><td>Renault</td><td>Barchetta</td><td>Red</td></tr> 
  <tr><td>1981</td><td>GM</td><td>Cadillac</td><td>Pink</td></tr> 
</tbody>
</table>
```

## Your Assignment

Create an HTML Table to display the following data:

| First Name | Last Name | Phone |
| :--- | :--- | :--- |
| Maryam | Henry | 347-694-8645 |
| Amelia | Cannon | 748-534-6259 |
| Hilel | Watts | 736-712-0782 |
| Portia | Hampton | 728-690-5531 |
| Cameran | Kline | 775-470-2885 |
| Ashton | Dickerson | 417-859-1589 |
| Sopoline | Flowers | 445-198-8160 |
| Reese | Huffman | 491-627-6062 |
| Hanna | Wheeler | 975-850-0929 |

