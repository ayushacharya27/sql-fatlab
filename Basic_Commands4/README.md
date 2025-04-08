# Row wise Commands in SQL

## Manipulating Rows of the table
### Upper - Makes all characters in that particular col capital and works for all rows
### Lower - Makes all characters in that particular col small
### initcap - Makes the first letter of that particular word capital

Query:
```bash
select upper({col_name}) , initcap({col_name}) , lower({col_name}) from {table_name};
```
Example:
```bash
select upper(name) , initcap(name) , lower(name) from emp_names;
```

## Character Functions CONCAT, LENGTH, SUBSTR, INSTR, LPAD, RPAD, TRIM and REPLACE:
### concat - concatinate sting with ur preffered string.
### lenght - gives the length of the string.
### substr - gives the given substring of the string.
### instr - gives the position of a particual character in row col.
### lpad - adds padding of any character at left where we provide a character.
### rpad - adds padding of any character at right where we provide a character.
### replace - replaces a particular character with character of ur choice.

Example:
```bash
select name, concat(name , 'Kumar')   , length(name) , substr(name , 2 ,3) , lpad(name , 10 , '#') , rpad(name , 10 , '*') , replace(name , 'a' , '@') from emp_names;
```




