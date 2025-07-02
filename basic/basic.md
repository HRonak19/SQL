# Basic of SQL

## Create table  

```
Create Table Student;
```
> `Create Table` is command to make `MT` table \
> **Student** is a Name of Table

## add column in Table

```
Alter Table Student ADD(RollNO number(3) , Name varchar(20));
```
> `Alte Table` is command to add new column \
> **ADD** is Keyword  \
> `RollNO` is name of column  \
> **number** is data type of column \
> `3` is range of  number like you add max 3 digit Ex **212**

## add data into table

```
Insert into Student values(&RollNo,'&Name');
```
> `Insert into` is command to add values \
> **values** is Keyword \
> **`&`** must be use befor column name \
> you to use String or charecter must be use `'` 
