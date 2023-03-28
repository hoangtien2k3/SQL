
## Insert Into Select

- INSERT INTO SELECT sao chép dữ liệu từ một bảng và chèn nó vào một bảng khác.
- INSERT INTO SELECT yêu cầu kiểu dữ liệu trong bảng nguồn và bảng đích phải khớp nhau.


Syntax:
```roomsql
INSERT INTO table2
SELECT * FROM table1
WHERE condition;
```

or
```roomsql
INSERT INTO table2 (column1, column2, column3, ...)
SELECT column1, column2, column3, ...
FROM table1
WHERE condition;
```



Ex:
```roomsql
INSERT INTO Customers (CustomerName, City, Country)
SELECT SupplierName, City, Country FROM Suppliers;
```

Ex:
```roomsql
INSERT INTO Customers (CustomerName, City, Country)
SELECT SupplierName, City, Country FROM Suppliers
WHERE Country='Germany';
```
