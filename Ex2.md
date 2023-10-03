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
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/a6ec7ac3-f8f4-4f6c-90fe-c5b2d68caaa8)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/516d97e9-2f72-42b2-974a-960481b2f018)

### Q2) Delete the records from manager table where the salary less than 2750.
## QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/c1c4f798-c143-494e-92dc-9ecde835b44d)

## OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/34ac8772-5137-4229-9ec8-f51620f94e3f)

### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/2f4e38ae-006d-4525-8ea9-e891f82cc035)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/31da2dbe-d87e-4219-98da-32c3cdaae6aa)

### Q5)	List the names of Clerks from emp table.
## QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/8b04d452-ad17-4afe-9547-a93816344664)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/84b17fb4-fffb-48f0-877d-e80e6c7e88e1)

### Q6)	List the names of employee who are not Managers.
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/0d21ecea-0f50-4b74-941a-ef83dd9cdb01)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/1ffd29e6-a1f8-4192-b182-9799f1428fca)

### Q7)	List the names of employees not eligible for commission.
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/b6b47a91-cfb0-41ee-aaf4-34c4de41550e)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/1dec71e1-6e2c-4c05-a186-707fd5c94e99)


### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/93b459b1-01d4-4c8d-a505-1b0593ecd249)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/b2c9b5ce-6d43-4648-aa22-15aefa59e6d0)


### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/dab72ba1-05ac-43fb-b943-6f1016409207)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/27fcb2f0-98a6-410e-a04e-2b8063293092)


### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/05120525-827c-4e3f-87c8-db7c89605a26)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/1ca1f106-b154-419d-b123-b6678245d692)


### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/f824cf33-8ff5-4727-b870-00260ef82031)

### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/1c064453-0a43-4ec2-91b1-870875768d99)


### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/bd595671-67fb-4940-9c5d-2dda66481e02)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/ad250683-45b1-4667-b399-5109524d28f9)

### Q13) Find number of rows in the table EMP

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/a1271bbf-ebc7-4fc7-9866-6859b1697e00)

### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/7810b26e-547d-4a15-be4f-0b3313bdcbc5)


### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/7a34515b-a60c-45d6-9d69-4dbdd8e6d74c)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/856afb8b-d873-440f-be9b-cdc77c4ee7f6)


### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/2f8ccb53-1871-40db-bc7a-cb8df51f0a29)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/120552008/3b9b8313-7368-4384-a8c4-1fb8868b6419)
### RESULT:
Thus the Data Manipulation Language (DML) Commands and built in functions in SQL
