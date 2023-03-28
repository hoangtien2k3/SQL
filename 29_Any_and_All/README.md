
## Any and All

- Các toán tử ANY và ALL cho phép bạn thực hiện so sánh giữa một giá trị cột đơn và một dải giá trị khác.



Syntax Any:
```roomsql
SELECT column_name(s)
FROM table_name
WHERE column_name operator ANY
  (SELECT column_name
  FROM table_name
  WHERE condition);
```


Ex:
```roomsql
SELECT * FROM customers WHERE sales_price > ANY(500, 1000);
```

Ex:
```roomsql
SELECT ProductName
FROM Products
WHERE ProductID = ANY
  (SELECT ProductID
  FROM OrderDetails
  WHERE Quantity = 10);
```


///////////////////////////////////////////////////////////////////////////////////////////////////

Syntax All:
```roomsql
SELECT column_name(s)
FROM table_name
WHERE column_name operator ALL
  (SELECT column_name
  FROM table_name
  WHERE condition);
```

Ex:
```roomsql
SELECT ProductName
FROM Products
WHERE ProductID = ALL
  (SELECT ProductID
  FROM OrderDetails
  WHERE Quantity = 10);
```

Ex:
```roomsql
SELECT ALL ProductName
FROM Products
WHERE TRUE;
```