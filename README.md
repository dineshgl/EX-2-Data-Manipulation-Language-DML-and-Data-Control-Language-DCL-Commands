# EX 2 Data Manipulation Language (DML) Commands and built in functions in SQL
## AIM:
To create a manager database and execute DML queries using SQL.


## DML(Data Manipulation Language)
<div align="justify">
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
</div>

## List of DML commands: 
<div align="justify">
INSERT: It is used to insert data into a table.<br>
UPDATE: It is used to update existing data within a table.<br>
DELETE: It is used to delete records from a database table.<br>
</div>

## Create the table as given below:
```sql
create table manager(enumber number(6),ename char(15),salary number(5),commission number(4),annualsalary number(7),Hiredate date,designation char(10),deptno number(2),reporting char(10));
```
## insert the following values into the table
```sql
insert into manager values(7369,'Dharsan',2500,500,30000,'30-June-81','clerk',10,'John');
insert into manager values(7839,'Subu',3000,400,36000,'1-Jul-82','manager',null,'James');
insert into manager values(7934,'Aadhi',3500,300,42000,'1-May-82','manager',30,NULL);
insert into manager values(7788,'Vikash',4000,0,48000,'12-Aug-82','clerk',50,'Bond');
```

### Q1) Update all the records of manager table by increasing 10% of their salary as bonus.

### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/9e9646a2-6bc3-4d25-96b6-09e980a9b38e)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/13bdb417-c0fb-446c-9daa-ecd381c6b6af)

### Q2) Delete the records from manager table where the salary less than 2750.
## QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/bda5d23e-da12-4f04-91cd-61b2d0fb3dee)

## OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/cc718534-b5a8-4f08-867e-65ae166dd8ca)

### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/2b4dd68c-ce1b-4f26-abee-184da220b8cc)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/2fc4d118-3f21-4084-9b5c-328316d2b901)

### Q5)	List the names of Clerks from emp table.
## QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/1af05e93-52d6-4ad1-b1df-9740f98c0786)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/4e093a67-6a5e-4c07-8f3e-682aeaa5be21)

### Q6)	List the names of employee who are not Managers.
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/e430b696-ac1e-4143-82b4-2c9ed1eab62b)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/3e0ca1e6-c5b8-4793-8333-0d4aad910703)

### Q7)	List the names of employees not eligible for commission.
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/485b302e-6256-4486-82a7-41692be45bee)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/8acb421a-f3f3-4b98-b476-349c82db0386)


### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/c3550707-b22c-42a0-a513-eadd091823da)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/c80c281c-5ed2-48ae-8c3d-9777f173eea8)


### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/d5687168-7995-4143-8403-60ef3c001a47)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/616ed1a5-6507-4e87-b7b1-8cf03003d558)


### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/b89fe0da-c3a4-416d-9a7f-46f1162da900)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/d871d976-d92e-413d-bb56-8a52e5f560b4)


### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/3795c30a-d635-44c3-aec8-b25b73280ef1)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/5592b86d-b3e7-405d-a850-12ea45b72a0e)


### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/716ebf6a-397b-47af-b025-bcf7a1545ed1)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/2ed19f49-0113-4e54-bbe0-8333d7f6ad0e)

### Q13) Find number of rows in the table EMP

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/80213feb-1a01-4e49-9ab0-5a9bab3238c2)

### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/a393b618-14d2-4a6a-a3c2-ca42f4f072a2)


### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/c717977d-5466-4f9d-8ac7-54ae3173bf94)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/c8c19ab9-f8d4-4f3f-819d-899b6e44e1fc)


### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/af00cb8d-bf93-4e48-8b7a-4077423c70fb)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/26cc394b-b399-4223-89a7-bae95533000d)
### RESULT:
Thus the Data Manipulation Language (DML) Commands and built in functions in SQL
