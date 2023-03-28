
## Left Join:

- The LEFT JOIN keyword returns all records from the left table (table1), and the matching records from the right table (table2).

LEFT JOIN Syntax:
```roomsql
SELECT column_name(s)
FROM table1
LEFT JOIN table2
ON table1.column_name = table2.column_name;
```

![](https://www.w3schools.com/sql/img_leftjoin.gif)


Ex:
```roomsql
SELECT Customers.CustomerName, Orders.OrderID
FROM Customers
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID
ORDER BY Customers.CustomerName;
```

    