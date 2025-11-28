# table name : EMPONE

<center>

| column name | datatype | size | attribute|
|---|---|---|---|
|emp_id|number|6|primary key |
|branch_id|number|6|-|
|Fname | varchar2|15|not NULL|
|Lname | varchar2 | 15 | -|
|dept | varchar2 | 15 | - |
|designation |varchar2|15| - |
|salary | number | 5 | - |
|commission | number | 4 | -|

</center>

1 create table 
```
create table empone(emp_id number(6) primary key , branch_id number(6), Fname varchar2(15)not NULL , Lname varchar2(15)not NULL, dept varchar2(15) , designation varchar2(15),salary number(5), commission number(4));
```
2 insert Records
```
insert into empone values(&emp_id,&branch_id,'&fname','&Lname','&dept','&designation',&salary,&commission);
```
3 show table structuer
```
DESC empone;
```
4 combine Fname and Lname add new column name is fullname
```
select concat (Fname,Lname) as Fullname from empone;
```
5 Rename table empone to  employee_master
```
rename empone to employee_master;
```
6 employee whose salary is greater than 15000
```
select * From employee_master where salary >= 15000;
```
7 list inorder by designation
```
 select * from employee_master order by Designation;
```
