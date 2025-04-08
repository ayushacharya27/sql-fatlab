# Basic SQL Commands

This is a simple reference for basic Git commands to get you started with version control.

## Table Creation and alteration

### Table Creation:
```bash
create table ayush (name char(15) , roll_number intger , salary intger);
```

### Show latest table
```bash
desc ayush;
```

### Table alteration:
Adding a new coloumn
```bash
alter table ayush add(income integer);
```

Modify an Existing coloumn
Point: You can use both varchar and varchar2 and dont forget to add the length!!
```bash
alter table ayush modify(roll_number varchar2(4));
```

Drop any coloumn
```bash
alter table ayush drop(income);
```

### Inserting Values to table
Point: Always remember the order u put the coloumns!!
For String always use ''!!  
```bash
insert into ayush values('Ayush' , 23BPS1078 , 10000);
insert into ayush values('Sakshee' , 23BPS1079 , 10000);
```

### See the Current Table
```bash
select* from ayush
```

### If you want a particular col to be selected
```bash
select name from ayush;
```

### Delete all rows from table
```bash
delete from ayush;
```

### Drop the table
```bash
drop table ayush;
```











 
