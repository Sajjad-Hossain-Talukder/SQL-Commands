
<br>
<br>

#### Section 08 : [ JOIN - CARTESIAN PRODUCT ] : Row 


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

##### Inner Join or Join : 






| Command    | Description |
| ----------- | ----------- |
|  **INNER JOIN** | <img src="images/inner.gif">  <br> Returns records that have matching values in both tables |
| **RIGHT (OUTER) JOIN** |<img src="images/right.gif">  <br>Returns all records from the left table, and the matched records from the right table|
| **LEFT (OUTER) JOIN** |<img src="images/left.gif">  <br>RIGHT (OUTER) JOIN: Returns all records from the right table, and the matched records from the left table|
| **FULL (OUTER) JOIN** |<img src="images/full.gif">  <br>FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table|
