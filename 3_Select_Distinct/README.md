
## 2_Select Distinct

- The SELECT DISTINCT statement is used to return only distinct (different) values.
- Inside a table, a column often contains many duplicate values; and sometimes you only want to list the different (distinct) values.

```roomsql
SELECT DISTINCT column1, column2, ...
FROM table_name;
```

Ex:
> SELECT DISTINCT Country FROM Customers;

