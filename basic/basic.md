# Introduction to SQL commands

* DDL `Data Definition Language`
* DML `Data Manipulation Language`
* DCL `Data Control Language`
* TCL `Transaction Control Language`

# 1 DDL COMMANDS

## Create Command
```
create table Student(NO number(2), name varchar2(10),B_Date DATE);
```

## Alter Command

### 1 to add a new column 
```
alter table Student ADD(address varchar2(20));
```
### 2 To Modify exiting column
```
alter table Student MODIFY(address varchar2(15));
```
> You can modify datatype and its size
### 3 To drop existing column
```
alter table student Drop column mok;
```
Drop command
```
DROP TABLE student;
```
 Rename command
```
RENAME student TO STU;
```
# 2 DML Commands

## INSERT Commnds

### 1 First Way
```
INSERT INTO stu values(1,'Qon','17/MAY/2003','botad');
```
### 2 Second Way
```
INSERT INTO STU(no,name,B_date,address) values (2,'Won','18-jun'2003','jayput');
```
### 3 third Way
```
INSERT INTO stu values(&no,'&name','&B_date','&address');
```
## UPDATE COMMAND
```
update stu SET NO=3 WHERE name='Won';
```
## DELETE COMMAND
```
DELETE FROM stu WHERE no=2;
```

# delete This type of table 
```
PURGE TABLE "BIN$hudh46ZSQI+9DolBWAaQTg==$0";
```