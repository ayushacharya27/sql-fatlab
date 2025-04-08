## Manipulating Coloumns

### Select a col or all col(select *) where there is some conditions
```bash
select [(col_name) OR *] from (table_name) where col_name=200/'Ayush';
```
Example:
```bash
 select * from ayush where price = 500;
```

### For a Range
```bash
select [(col_name) OR *] from (table_name) where col_name between 175 and 250;
```
Example:
```bash
select title from ayush where price between 400 and 700;
```

### Selecting name starting from using LIKE operator , it selects the row where the name starts with any_char;
```bash
select [(col_name) OR *] from (table_name) where col_name like '(any_char)%';
```
Example:
```bash
select * from ayush where author like 'a%';
```

### if u want to select a name which ends with any_char;
```bash
select [(col_name) OR *] from (table_name) where col_name like '%(any_char)';
```

Example:
```bash
select * from ayush where author like '%a';
```

## This Changes the actual Table
### Updating a col of intger;
```bash
update ayush set col_name = col_name + 20;
```
Example:
```bash
update ayush set price = price + 100;
```

## If you dont want to change the table
Returns square root of table;
```bash
select sqrt(col_name) from ayush;
```
Use more math functions like floor and ceil with sqrt to make it proper integer


### Sum, Average, Max and Min
```bash
select [sum(col_name) OR avg(col_name) OR min(col_name) OR max(col_name)] from ayush;
```




 



