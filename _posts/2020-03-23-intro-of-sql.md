---
layouts: archive
title: "Introduction to SQL I"
---
## Introduction to SQL I
> SQL is a  domain-specific programming language designed for managing data in a relational database management system(RDBMS), and is used by a huge number of apps and organizations. For more information, please click the following link: [SQL_wiki](https://en.wikipedia.org/wiki/SQL "Title")

Nowadays, people who work as data scienctist and analyst, software developer and even web designer require to use SQL as a tool for sharing and managing data in RDBMS. This post aims to record my self-learning experience and share with people who would like to learnig some basic technics in SQL. So, Let's get started.

* About SQL <br>

&emsp;&emsp;SQL are compoesd of three parts 
> Data Definition Language(DDL) <br>
  Data Manipulation Language(DML) <br>
  Data Control Language (DCL)

Today, I will introduce the first part, DDL.

 ---

* About Tables

> Before we go through the Syntax of SQL, we whould have fundemantal understading about the `Tables`.

| Data direction | name | also known as |
| :------------- | :--- | :------------ |
| horizontal     | Rows | Observations  |
| vertical       | Columns | Variables  |

 ---

### Important Syntax in DDL
* remark: the syntax and function of SQL need to be all capitals. e.g. SELECT, FROM and DROP.
* remark2: put the semicolon (`;`) in the end of statement.

1. Create Statement 
  * The create command is used to establish a new database, table, index, or stored procedure.

> Syntax: CREATE DATABASE `database-name` <br>
  Example: CREATE DATABASE `exerciseDB`;

> Syntax: CREATE TABLE `table-name` 
  Example: CREATE TABLE `exercise_table`;
  
2. Delete Statement <br>
  * The DROP statement destroys an existing database, table, index, or view.

> Syntax: DROP DATABASE `database-name` <br>
  Example: DROP DATABASE `exerciseDB`;
  
> Syntax: DROP TABLE `table-name` <br>
  Example: DROP TABLE `exercise_table`;

3. Alter Statement 
  * The ALTER statement modifies an existing database object.

> Syntax: ALTER DATABASE `database-name` <br>
           &emsp;&emsp;&emsp;&ensp;MODIFY NAME = `new_db`; <br>
   Example: ALTER DATABASE `exerciseDB`  <br>
            &emsp;&emsp;&emsp;&emsp;MODIFY NAME = `exerciseDB_new`; 

> Syntax: ALTER TABLE `table-name` <br>
           &emsp;&emsp;&emsp;&ensp;ADD COLUMN `col_type`; <br>
   Example: ALTER TABLE `exercise_table`  <br>
            &emsp;&emsp;&emsp;&emsp;ADD COLUMN `Age`;

> Syntax: ALTER TABLE `table-name` <br>
           &emsp;&emsp;&emsp;&ensp;ADD PRIMARY KEY `col_name`; <br>
   Example: ALTER TABLE `exercise_table`  <br>
           &emsp;&emsp;&emsp;&emsp;ADD PRIMARY KEY `Age`;
