
# Create Table Stud_Result

<center>

| Column |  type | No |
|--- |   ---  |:---:|
|RNO | Number | 5 |   
|SNAME| varchar2 | 20|
|BDATE| date | - |
|: --- :|: --- :|: --- :|

***
</center>

## Commands 

 Create Table using `create` command

```
create table Stud_Result (Rno number(5) , Sname varchar2(20) , Bdate date);
```
 Add Reconds and rno Start with 101 , Using `Insert` Command

```
insert into Stud_Result values(101,'Raj','10-Jun-2005');
```

 add new 3 Columns uisng `alter` command

<center>

| Column | Type | No |
|---|---|---|
|SUB1 | number | 3 |
|SUB2 | number | 3 |
|SUB3 | number | 3 |

</center>

```
alter table Stud_result add(SUB1 number(3) , SUB2 number(3) , SUB3 number(3));
```

 add recond using `update` command
```
update stud_result set sub1=59 where Rno=101; 
``` 
```
update stud_result set sub2=69 where Rno=101; 
```
```
update stud_result set sub3=89 where Rno=101; 
```
 update all Subject using this way

***

Add new 3 Columns using `alter` command like

<center>

| Column | Type | No |
|  ---  |  ----  |:---:|
| Total | Number | 5 |
| Per   | Number |5.2|
| Grade | varchar2 | 3 |

</center>

```
alter table Stud_Result add(Total number(5) , Per number(5,2) , Grade varchar2(3));
```

total of all Subject using `update command`

```
 update Stud_result set total = sub1 + sub2 + sub3;
```

make percentage of total 

```
 update Stud_result set PER = total / 3;
```

give Grades  

```
 update Stud_result set GRADE='A' where Per>=80
```
```
update Stud_result set GRADE='B' where Per>=60 and Per < 80;
```
```
update Stud_result set GRADE='C' where Per>=45 and Per < 60;
```

# SAVE TABLE

```
commit;
```