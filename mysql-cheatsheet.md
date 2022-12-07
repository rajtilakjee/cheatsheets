# MySQL Cheatsheet

MySQL is an open-source relational database management system. This cheatsheet contains the most commonly used commands and statements that helps you work with MySQL more effectively.

## Starting with MySQL

### Connect to MySQL Server

`mysql -u [username] -p;`

### Connect to MySQL Server with a database using a username and password

`mysql -u [username] -p [database];`

### Exit MySQL Command-Line client

`exit;`

### Export data using mysqldump tool

`mysql -u [username] -p [database] > data_backup.sql;`

## Working with Databases

### Create a database with a specific name only if it does not exists

`CREATE DATABASE [IF NOT EXISTS] database_name;`

### Change currect database to another one

`USE database_name;`

### Delete a database with a specific name

`DROP DATABASE [IF EXISTS] database_name;`

### Show all available databases in the current server

`SHOW DATABASES;`

## Working with tables

### Show all tables in current database

`SHOW TABLES;`

### Create a new table

`CREATE TABLE [IF NOT EXISTS] table_name(field1 type1, field2 type2);`

### Add a new column into a table

`ALTER TABLE table_name ADD [COLUMN] column_name column_definition [FIRST|AFTER existing_column];`

### Delete a column from a table

`ALTER TABLE table_name DROP [COLUMN] column_name;`


