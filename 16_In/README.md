## IN
- The IN operator allows you to specify multiple values in a WHERE clause.
- The IN operator is a shorthand for multiple OR conditions.


IN Syntax:
```roomsql
SELECT column_name(s)
FROM table_name
WHERE column_name IN (value1, value2, ...);
```

or
```roomsql
SELECT column_name(s)
FROM table_name
WHERE column_name IN (SELECT STATEMENT);
```


Ex:
// nghiĩa là IN nằng trong điều kiện Where để chứa các điều kiện ràng buộc
```roomsql
SELECT * FROM Customers
WHERE Country IN ('Germany', 'France', 'UK');
```
