
## Case:

CASE có 2 định dạng:
- Hàm CASE đơn giản hay còn gọi là Simple CASE.
- Hàm CASE tìm kiếm hay còn gọi là Searched CASE.


CASE Syntax:
```roomsql
CASE
   WHEN condition1 THEN result1
   WHEN condition2 THEN result2
   WHEN condition3 THEN result3
   ...
   ELSE default_result
END
```

Trong đó, các phần tử của câu lệnh là:

- "condition1", "condition2", "condition3", ...: Các điều kiện cần được kiểm tra.
- "result1", "result2", "result3", ...: Kết quả trả về nếu điều kiện tương ứng được đáp ứng.
- "default_result": Giá trị mặc định trả về nếu không có điều kiện nào được đáp ứng.




Ex:
```roomsql
SELECT employee_name, salary,
CASE
   WHEN salary >= 50000 THEN 'high'
   WHEN salary >= 30000 THEN 'medium'
   ELSE 'low'
END AS salary_group
FROM employees;
```

Kết quả:

|employee_name | salary   | salary_group |
|--------------|----------|--------------|
|John          | 40000    | medium       |
|Mary          | 55000    | high         |
|Bob           | 25000    | low          |   

Như vậy, câu lệnh "CASE" trong SQL rất hữu ích để thực hiện các phép tính logic phức tạp trong câu truy vấn và trả về các giá trị được xử lý một cách dễ dàng.









