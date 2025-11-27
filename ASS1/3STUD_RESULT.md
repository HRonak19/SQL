# Create Stud1_Result table

<center>

| Column | Datatype | values |
|---|---|---|
|Stud_RollNo|number|3|
|Stud_Name|varchar2|15|
|City|varchar2|20|
|Oracle|number|3|
|Asp|number|3|
|Network|number|3|
|Se|number|3|

</center>

# Commands

1 Create Table `STUD1_RESULT`
```
Create table Stud1_Result (Stud_Rollno number(3),Stud_name varchar2(15),City varchar2(20),Oracle number(3), Asp number(3) , Network number(3),Se number(3));
```
2 insert 10 Records 
```
insert into Stud1_Result values(&Stud_Rollno,'&Stud_name','&City',&Oracle,&Asp,&Network,&Se);
```
using this ->  ` / `

3 Display all info
```
select * from Stud1_Result;
```
4 Display table structure
```
desc Stud1_Result;
```
5 add more columns like

<center>

|Column | Datatype | Values|
|---|---|---|
|Total|Number|3|
|Per |Number|6,2|

</center>

```
alter table Stud1_Result add(total number(3),Per number(6,2));
```
6 update column total & Per
```
update Stud1_Result set total = Oracle + Asp + Network + Se;
```
```
update Stud1_Result set Per = Total / 4;
```
h
