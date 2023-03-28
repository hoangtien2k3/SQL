
## Between: (phạm vi của giá trị cần lấy ra)

- The BETWEEN operator selects values within a given range. The values can be numbers, text, or dates.
- The BETWEEN operator is inclusive: begin and end values are included. 


Between syntax:
```roomsql
SELECT column_name(s)
FROM table_name
WHERE column_name BETWEEN value1 AND value2;
```

Ex:
```roomsql
SELECT * FROM Products
WHERE Price BETWEEN 10 AND 20;
```