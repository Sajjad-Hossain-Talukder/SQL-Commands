
<br>
<br>

### Section 08 : [ JOIN - CARTESIAN PRODUCT ] : Row 


In different cases , we need to join two or more tables.To join two or more tables , we apply Cartesian Product formula here.But Cartesian Product returns all possible result .So also need to apply condition basis of Primary Key/Others Key of those table.

**Syntex :** 
```
SELECT * FROM tablename_1 , tablename_2 , ..... where condition/s.
```
Given Command Shows all column from those table . To get specific colum use ```tablename_1.column_name``` instead of * . We can re-write the command using **JOIN-ON** keyword.

**Syntex :** 

```
SELECT * FROM tablename_1 JOIN tablename_2 JOIN ..... ON condition/s.
```

**Classification of Join :** 

Here we are using two table given below to understand join in MySQL . 
<br>
#### INNER JOIN or JOIN : 

<img src="images/inner.gif">

<img src="images/inner.png">

**Syntex :**
```
SELECT column_name(s)
FROM table1
INNER JOIN table2
ON table1.column_name = table2.column_name;

```
<br>
#### LEFT OUTER JOIN : 

<img src="images/left.gif">

<img src="images/left.png">

**Syntex :**
```
SELECT column_name(s)
FROM table1
LEFT JOIN table2
ON table1.column_name = table2.column_name;

```
<br>
#### RIGHT OUTER JOIN : 

<img src="images/right.gif">

<img src="images/right.png">

**Syntex :**
```
SELECT column_name(s)
FROM table1
RIGHT JOIN table2
ON table1.column_name = table2.column_name;

```
<br>
#### FULL OUTER JOIN : 

<img src="images/full.gif">

<img src="images/full.png">

**Syntex :**
```
SELECT column_name(s) FROM table1 LEFT JOIN table2  ON table1.column_name = table2.column_name;
UNION
SELECT column_name(s) FROM table1 RIGHT JOIN table2  ON table1.column_name = table2.column_name;

```






| Command    | Description |
| ----------- | ----------- |
|  **INNER JOIN**<br> SELECT column_name(s)<br>FROM table1<br>INNER JOIN table2<br>ON table1.column_name = table2.column_name;|Returns records that have matching values in both tables |
| **LEFT (OUTER) JOIN** <br> SELECT column_name(s)<br>FROM table1<br>LEFT JOIN table2<br>ON table1.column_name = table2.column_name;|Returns all records from the left table, and the matched records from the right table|
| **RIGHT (OUTER) JOIN** <br>SELECT column_name(s)<br>FROM table1<br>RIGHT JOIN table2<br>ON table1.column_name = table2.column_name;| Returns all records from the right table, and the matched records from the left table|
| **FULL (OUTER) JOIN** <br> SELECT column_name(s) FROM table1 <br> LEFT JOIN table2  ON table1.column_name = table2.column_name;<br>UNION<br>SELECT column_name(s) FROM table1<br> RIGHT JOIN table2  ON table1.column_name = table2.column_name;
|FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table|


