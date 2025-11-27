# Create following table 

table name `EMP`

<center>

| column | type | No |
|---|---|---|
| emo_id | number | user |
| name | varchar2 | user |
| city | varchar2 | user |
| job | varchar 2 |user |
| salary | number | user |
| join_date | date |  -|
| commission | number | user |
| dept_no | number | user |

</center>

table name `dept`

<center>

| column | type | No | key |
|---|---|---|---|
|dept_no | number | 3 | primer |
|dname | varchar2 | 20 |  |
| location | varchar2 | 15 | |

</center>


# Command
1
Create dept table add its column 
```
create table dept(dept_no number(3) primary key , dname varchar2(20) , location varchar2(15));
```
Create emp table add columns
```
create table emp(emp_id number(3) , name varchar2(10) , city varchar2(15) , job varchar2(15) , salary number(5) , join_date date , commission number(5) , dept_no number(3)  references dept(dept_no));
```
2 insert values in the table <br>
emp
```
insert into emp values(&emp_id,'&name','&city','&job','&salary','&join_date',&commission,&dept_no);
```
dept
```
insert into dept values(&dept_no,'&dname','&location');

```
# 3 `display both table at time`
```
 select * from emp e join dept d ON e.dept_no = d.dept_no;
```
4 display info of employee join the mark `march`
```
select * from emp where join_date like '% mar';
```
5 display detail of employee whose city is not `botad & jayput`
```
select * from emp where not city='botad' and city='jaypur';
```
6 display detail of employee joined after `01-jun-2020`
```
select * from emp where join_date > '01/jun/2020';
```
7

