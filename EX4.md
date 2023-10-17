### Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:

### Program To Create Table:
```
create table employee(empid number(10),name char(40),dept char(30),salary number(30));
```
## Program To Create Procedure:
```
create or replace procedure inserting_data is
begin
insert into employee values(101,'dhivya','ai ds',60000);
insert into employee values(102,'swetha','IT',70000);
insert into employee values(103,'deepesh','IT',80000);
insert into employee values(104,'thilaga','iot',65000);
COMMIT;
END;
/
```
## Program To Call The Procedure:
```
execute inserting_data;
```
## Program To Display The Table:
```
select * from employee;
```

### Output:
![dnms4 1](https://github.com/dhivyapriyar/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/119477552/c00b7906-86b5-47e9-b49c-e19c0769cddd)
![dbms4 2](https://github.com/dhivyapriyar/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/119477552/5d4800f9-10fa-4602-8e3e-ad82c9571639)


### Result:
Hence procedure has been created using PL/SQL.
