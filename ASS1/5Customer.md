# CUSTOMERS

| column | Datatype | size | attribute |
| --- | --- | ---- | --- |
| cust_no | number | 3 | primary key |
| Fname | varchar2 | 15 | - |
| Lname | varchar2 | 15 | - |
| Birth_Date | date | - | - |
| city | varchar2 | 10 | - |
| Mob_no | number | 10 | - |
| dept_name | varchar2 | 20 | - |
| Salary | number | 15 | - |

# Commands 
1 create table 
```
create table customer (cust_no number(3) primary key , fname varchar2(15),Lname varchar2(15) , birth_date date, city varchar2(10),mob_no number(10),dept_name varchar2(20),salary number(15));
```
2 insert data
```
 insert into customer values(&cust_no,'&fname','&lname','&birth_date','&city',&mob_no,'&dept_name',&salary);
```
