---
layouts: archive
title: "Introduction to SQL"
---
## Introduction to SQL
> SQL is a  domain-specific programming language designed for managing data in a relational database management system(RDBMS), and is used by a huge number of apps and organizations. For more information, please click the following link: [SQL_wiki](https://en.wikipedia.org/wiki/SQL "Title")

Nowadays, people who work as data scienctist and analyst, software developer and even web designer require to use SQL as a tool for sharing and managing data in RDBMS. This post aims to record my self-learning experience and share with people who would like to learnig some basic technics in SQL. So, Let's get started.

* About SQL
SQL are compoesd of three parts 
> Data Definition Language(DDL) <br>
  Data Manipulation Language(DML) <br>
  Data Control Language

Today, I will introduce the first two parts, DDL and DML.

 ---

* About Tables

> Before we go through the Syntax of SQL, we whould have fundemantal understading about the `Tables`.

| Data direction | name | also known as |
| :------------- | :--- | :------------ |
| horizontal     | Rows | Observations  |
| vertical       | Columns | Variables  |

 ---

### Important Sntax in DDL
* remark: the syntax and function of SQL need to be all capitals. e.g. SELECT, FROM and DROP.
* remark2: put the semicolon (`;`) in the end of statement.

1. Create a new database or table
> Syntax: CREATE DATABASE `database-name` <br>
  Example: CREATE DATABASE `exerciseDB`;

> Syntax: CREATE DATABASE `table-name` <br>
  Example: CREATE DATABASE `exercise_table`;
  
2. Delete a database or table
> Syntax: DROP DATABASE `database-name` <br>
  Example: DROP DATABASE `exerciseDB`;
  
> Syntax: DROP DATABASE `table-name` <br>
  Example: DROP DATABASE `exercise_table`;

3. Alter a database
> Syntax: ALTER DATABASE `database-name` <br>
           &emsp;&emsp;&emsp;&ensp;MODIFY NAME = `new_db`; <br>
   Example: ALTER DATABASE `exerciseDB`  <br>
            &emsp;&emsp;&emsp;&emsp;MODIFY NAME = `exerciseDB_new`; 

> Syntax: ALTER DATABASE `database-name` <br>
           &emsp;&emsp;&emsp;&ensp;ADD COLUMN `col_type`; <br>
   Example: ALTER DATABASE `exerciseDB`  <br>
            &emsp;&emsp;&emsp;&emsp;ADD COLUMN `Age`;

> Syntax: ALTER DATABASE `database-name` <br>
           &emsp;&emsp;&emsp;&ensp;ADD PRIMARY KEY `col_name`; <br>
   Example: ALTER DATABASE `exerciseDB`  <br>
           &emsp;&emsp;&emsp;&emsp;ADD PRIMARY KEY `Age`;
