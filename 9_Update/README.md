
## Update:

- The UPDATE statement is used to modify the existing records in a table.

UPDATE Syntax:
```roomsql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

Ex:
```roomsql
UPDATE Customers
SET ContactName = 'Alfred Schmidt', City= 'Frankfurt'
WHERE CustomerID = 1;
```
