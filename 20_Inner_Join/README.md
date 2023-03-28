
## INNER JOIN 

Syntax:
```roomsql
SELECT column_name(s)
FROM table1
INNER JOIN table2
ON table1.column_name = table2.column_name;
```


![](https://www.w3schools.com/sql/img_innerjoin.gif)


Ex:

```roomsql
SELECT Orders.OrderID, Customers.CustomerName
FROM Orders
INNER JOIN Customers ON Orders.CustomerID = Customers.CustomerID;
```

