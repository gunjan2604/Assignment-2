# Assignment-2
 
## Create database and perform all basic queries.

- **To Create Database** (CREATE & USE Query)

  `CREATE DATABASE University;`

   `USE University;`

   `CREATE TABLE Student(`

     `Name varchar(50),`

     `Roll_no int primary key,`
                 
     `Enrollment_no VARCHAR(20),`  
               
     `Cgpa Decimal`  
         
     `Subject varchar(30)`
                   
     `Phone_no VARCHAR(15),`  
             
     `Address VARCHAR(100),` 
              
     `Date_Of_Birth DATE,`  
              
     `Gender char (1)); ` 

 
  
  *Output:*

  <img src="op1.png">
  
---

- **DROP Query**

  `DROP TABLE Student;`
  
  *Output:*
  
  <img src="op2.png">

---
 - **SELECT Query**

  `select * from Student;`
  
  *Output:*
  
  <img src="OP3.png">

---
 
- **INSERT Query**

`INSERT INTO Student (Name, Roll_no, Enrollment_no, Cgpa, Subject, Phone_no, Address, Date_Of_Birth, Gender)`
`VALUES`
    `('Alice', 101, 'E2023101', 8.2, 'Computer Science', '1234567890', '123 Main St', '2000-01-01', 'F'),`
    `('Bob', 102, 'E2023102', 7.9, 'Mathematics', '0987654321', '456 Oak St', '2001-02-02', 'M'),`
   `('Charlie', 103, 'E2023103', 8.5, 'Physics', '1122334455', '789 Pine St', '2000-03-03', 'M');`
    
  *Output:*
  
  <img src="OP3.png">

---


- **UPDATE & WHERE Query**

  `UPDATE Student`
  
  `SET cgpa = 8.1, subject = 'Data Science'`
  
  `WHERE roll_no = 102;`
  
  *Output:*
  
  <img src="op4.png">

---

- **ALTER Query**

  `ALTER TABLE Student`
  
  `RENAME COLUMN date_of_birth TO DOB;`
  
  *Output:*
  
  <img src="OP5.png">

---

- **ORDER BY Query**

  `SELECT * FROM Student ORDER BY cgpa DESC;`
  
  *Output:*
  
  <img src="OP6.png">

---

- **Inner Join Query**

  `SELECT Student.name, Student.roll_no, Student.cgpa, Department.head`
  
  `FROM Student`
  
  `INNER JOIN Department ON Student.subject = Department.subject;`
  
  *Output:*
  
  <img src="OP7.png">
---

- **Left Join Query**

  `SELECT Student.name, Student.roll_no, Student.cgpa, Department.head`
  
  `FROM Student`
 
  `LEFT JOIN Department ON Student.subject = Department.subject;`

  
  *Output:*
  
  <img src="OP8.png">

---

- **Right Join Query**

 `SELECT Student.name, Department.subject, Department.head`

 `FROM Student`

 `RIGHT JOIN Department ON Student.subject = Department.subject;`


  *Output:*
  
  <img src="OP9.png">

---

- **Full Outer-Join Query**

`SELECT Student.name, Student.roll_no, Student.subject, Department.head`

`FROM Student`

`LEFT JOIN Department ON Student.subject = Department.subject`

`UNION`

`SELECT Student.name, Student.roll_no, Student.subject, Department.head`

`FROM Student`

`RIGHT JOIN Department ON Student.subject = Department.subject;`

 
  
  *Output:*
  
  <img src="OP10.png">

---

