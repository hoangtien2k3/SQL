
## Select Into:

- The SELECT INTO statement copies data from one table into a new table.
  - (Câu lệnh SELECT INTO sao chép dữ liệu từ một bảng sang một bảng mới.)


Syntax:
```roomsql
SELECT *
INTO newtable [IN externaldb]
FROM oldtable
WHERE condition;
```


Chỉ sao chép một số cột vào một bảng mới:
```roomsql
SELECT column1, column2, column3, ...
INTO newtable [IN externaldb]
FROM oldtable
WHERE condition;
```


Ex:
```roomsql
SELECT * INTO CustomersBackup2017 IN 'Backup.mdb'
FROM Customers;
```

Ex:
```roomsql
SELECT Customers.CustomerName, Orders.OrderID
INTO CustomersOrderBackup2017
FROM Customers
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID;
```



