## Specifying Foreign key and primary key

### Primary key
For specifying primary key , make the particular col as primary key while defining the table
```bash
create table {table_name} (emp_name char(15) primary key , .........);
```

### Foreign key
For specifying foreign key , make the particular col as references {table_name}
```bash
create table {table_name1} (dept_name char(15) primary key , emp_name char(15) references {table_name} , .....);
```

## group by function SQL

### GROUP BY is used when we want to apply aggregate functions (like MIN(), MAX(), AVG(), SUM(), COUNT()) on each group of rows that share the same value(s) in one or more columns.

Example:
```bash
select deptno , max(salary) from employee1 group by deptno;
```
Point: If you dont group it , so it will not know max for which deptno , so if you are using group it will go deptno wise and provide max value of each dept

### select from two different tables
```bash
select ename , dept_name from employee , department where employee.deptno = department.deptno and city='madurai';
```
Here deptno is the foreign key and adding a constraint where city is "madurai".

Checking by adding if login works or not.



