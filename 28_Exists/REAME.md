
## Exists (giống như kiểu điều kiện lồng)

- Toán tử EXISTS được sử dụng để kiểm tra sự tồn tại của bất kỳ bản ghi nào trong một truy vấn con. 
- Toán tử EXISTS trả về giá trị TRUE nếu truy vấn con trả về một hoặc nhiều bản ghi.


Syntax:
```roomsql
SELECT column_name(s)
FROM table_name
WHERE EXISTS
(SELECT column_name FROM table_name WHERE condition);
```


Ex:
```roomsql
SELECT SupplierName
FROM Suppliers
WHERE EXISTS (SELECT ProductName FROM Products WHERE Products.SupplierID = Suppliers.supplierID AND Price < 20);
```






