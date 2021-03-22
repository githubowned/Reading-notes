# Readings : Object-Oriented Programming, HTML Tables

## What is Domain modeling?
Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

<p>&nbsp;</p>
<p>&nbsp;</p>

## TABLES 

### What's a Table?
A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

<p>&nbsp;</p>


- Grids allow us to understand complex data by referencing information on two axes.

- Each block in the grid is referred to as a table cell. In HTML a table is written out row by row.

<p>&nbsp;</p>
<p>&nbsp;</p>


### Table syntax 

 
```<tr>
<table>
<td>15<td>
<td>30<td>
</tr>

<tr>
<td>20</td>
<td>40</td>
</tr>
</table>
````

### This would render as :

<table>
<td>15</td>
<td>30</td>
</tr>

<tr>
<td>20</td>
<td>40</td>
</tr>
</table>


<p>&nbsp;</p>

### Table headings:
```
<table>
<tr>
<th></th>
<th scope="col">Saturday</th>
<th scope="col">Sunday</th>
</tr>
<tr>
<th scope="row">Tickets sold:</th>
<td>120</td>
<td>135</td>
</tr>
<tr>
<th scope="row">Total sales:</th>
<td>$600</td>
<td>$675</td>
</tr>
</table>
```
<p>&nbsp;</p>
<p>&nbsp;</p>

### This would render as:

<table>
<tr>
<th></th>
<th scope="col">Saturday</th>
<th scope="col">Sunday</th>
</tr>
<tr>
<th scope="row">Tickets sold:</th>
<td>120</td>
<td>135</td>
</tr>
<tr>
<th scope="row">Total sales:</th>
<td>$600</td>
<td>$675</td>
</tr>
</table>



<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>


---

# Refernces
1. From the Duckett HTML book:
      - Chapter 6: “Tables” (pp.126-145),

2. From the Duckett JS Book:
    - Chapter 3: “Functions, Methods, and Objects” (pp.106-144)