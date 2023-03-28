
## Union

- The UNION operator is used to combine the result-set of two or more SELECT statements.
- UNION được sử dụng để kết hợp tập hợp kết quả của hai hoặc nhiều câu lệnh SELECT. Mỗi câu lệnh SELECT với UNION phải có cùng số lượng cột, các cột phải có cùng kiểu dữ liệu, các cột trong mỗi câu lệnh SELECT phải có cùng trật tự.


UNION ALL Syntax
```roomsql
SELECT column_name(s) FROM table1
UNION ALL
SELECT column_name(s) FROM table2;
```


Ex:
```roomsql
SELECT City FROM Customers
UNION
SELECT City FROM Suppliers
ORDER BY City;
```



