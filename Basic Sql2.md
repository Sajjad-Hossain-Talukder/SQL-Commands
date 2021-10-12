#### Section 08: [ AS ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
| AS  | Used to <b> rename a column or table </b> with an  <b> alias (উপনাম) </b> . <br> An alias only exists for the duration of the query.|
| SELECT <b> CustomerName AS Customer</b>,<b> ContactName AS 'Contact Person'</b> <br> FROM Customers;| Renaming Column with single word or Multiple Words|
|SELECT o.OrderID, o.OrderDate, c.CustomerName<br>FROM <b>Customers AS c, Orders AS o</b><br>WHERE ....... ;|Renaming Table|
|SELECT S_Id as 'Student ID' , S_Name as 'Student Name' , <br> <b> CONCAT_WS(' ',S_Address,S_Email,S_Mobile) as 'Contact Details' </b> <br> from student  ;| Combining Column   |

