# Create The Customer Table as Follow

<center>

| Column | Type | No |
|---|---|---|
| Cust_id | varchar2 | 5 |
| Cust_Name | varchar2 | 15 |
| Cust_City | varchar2 | 15 |
|:---:|:---:|:---:|

</center>

# Commands
> Create Table using `Create` command

```
create table Customer (Cust_id varchar2(5) , Cust_Name varchar2(15) , Cust_City varchar2(15));
```
> add 10 Record in the table 

```
insert into Customer values('&Cust_id','&Cust_Name','&Cust_City');
```
>  use ` / ` to repait first command

# Display Section

1 Display all Information of Customer
```
select * from Customer;
```
2 Display Name and City of All Customer
```
select Cust_NAME , Cust_City From Customer;
```
3 Display Structure of Customer table
```
DESC Customer;
```
4 Display informaction of Customer `C107` 
```
select * from Customer where Cust_id='C107';
```
5 Display all Customer from Bhavanager
```
select * from Customer where Cust_City='Bhavnagar;
```
6 Display Customer From `Amreli` and `Rajkot`
```
select * from Customer where Cust_City='Amreli' or Cust_City='Rajkot';
```
7 Display all Customer except Form `BOTAD`
```
select * from Customer where Cust_City='Botad';
```
8 Display Customer Information in Deseending order
```
 select * from  Customer order by Cust_id DESC;
```
9 Display Informaction of Cust_Name = "Neelam"
```
select * from Customer where Cust_Name ='Neelam Patel';
```
