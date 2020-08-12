# SQOOP Export data from HDFS to MySQL
-----------------------


### MapReduce

Sqoop is a command-line interface application for transferring data between relational databases and Hadoop. <br/>


### Pros
* It involves transferring data from a variety of structured sources of data like Oracle, Postgres, etc. <br/>
* The data transfer is in parallel, making it fast and cost-effective. <br/>
* A lot of processes can be automated, bringing in heightened efficiency. <br/>
* It is possible to integrate with Kerberos security authentication. <br/>


### Input Directory
Input directory contains input table that will be uploaded to Sqoop. <br/>

<img src="Screenshots/input_directory.png"> <br/>

In the above screenshot, we can see an input directory (employee_data) contains input file – employee_data. <br/>


### Input_table

<img src="Screenshots/input_table.png"> <br/>

In the above screenshot, we can see that input contains employee_id, Name & Salary data. <br/>


### Create Database employeedb

<img src="Screenshots/create_database.png"> <br/>

In the above screenshot, we can see the employeedb is created. <br/>


### Create Table employee

<img src="Screenshots/create_table.png "> <br/>

In the above screenshot, we can see the schema of the employee table. <br/>


### Command to export data from hdfs to mysql
 
<img src="Screenshots/export.png"> <br/>

**sqoop export -** export to sqoop <br/>
**-m 1 -** number of mapper run 1 <br/>
**Jdbc:mysql://localhost/employeedb –** Connection to the database employeedb <br/>
**--username –** mysql username to verify that user has write access or not <br/>
**--table –** mysql table name <br/>
**--export-dir –** where data have to pick to insert into mysql <br/>


### Verify data in MySQL
 
<img src="Screenshots/verify_data.png"> <br/>

In the above screenshot, we can see that employee table contains all 4 rows. <br/>


### Some Basic Operations:

### 1.	Count records in employee table

<img src="Screenshots/count.png"> <br/>

In the above screenshot, we can see that count is 4. <br/>


### 2.	Select top 2 rows

<img src="Screenshots/top.png"> <br/>
 
In the above screenshot, top 2 records are printed on the screen. <br/>



**Created by:** <br/>
**Name: Krishna Kumar Singh** <br/>
**Email: krishnaai265@gmail.com** <br/>
**Phone: +91-9368754996** 
