
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

![image](https://user-images.githubusercontent.com/63524824/137452852-5c3897e3-ee61-458d-a645-8a21fcba913a.png)


