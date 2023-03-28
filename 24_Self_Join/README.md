
## Self Join:

- SELF-JOIN trong SQL có nghĩa là tự kết nối một bảng với chính nó.
- SELF JOIN – được sử dụng để tham gia một bảng với chính nó như thể bảng đó là hai bảng, tạm thời đổi tên ít nhất một bảng trong câu lệnh SQL. 

Self Join Syntax:
```roomsql
SELECT column_name(s)
FROM table1 T1, table1 T2
WHERE condition;
```


Ex:
```roomsql
SELECT A.CustomerName AS CustomerName1, B.CustomerName AS CustomerName2, A.City
FROM Customers A, Customers B
WHERE A.CustomerID <> B.CustomerID
AND A.City = B.City
ORDER BY A.City;
```


