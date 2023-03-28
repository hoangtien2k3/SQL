
## Min and Max:

- The MIN() function returns the smallest value of the selected column.
- The MAX() function returns the largest value of the selected column.


Min: 
```roomsql
SELECT MIN(column_name)
FROM table_name
WHERE condition;
```


Max:
```roomsql
SELECT MAX(column_name)
FROM table_name
WHERE condition;
```


Ex:
```roomsql
SELECT MIN(Price) AS SmallestPrice
FROM Products;
```



