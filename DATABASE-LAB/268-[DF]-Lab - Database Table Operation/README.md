# Database Table Operations Lab

## Introduction

Welcome to the Database Table Operations Lab! This hands-on session is designed to help you practice creating and dropping (deleting) databases and tables. The database operations team for an organization has configured a relational database instance, and you'll perform various tasks to enhance your skills in database management.

## Lab Overview and Objectives

This lab focuses on common database and table operations. By the end of this session, you should be able to:

- Use the `CREATE` statement to create databases and tables.
- Use the `SHOW` statement to view available databases and tables.
- Use the `ALTER` statement to alter the structure of a table.
- Use the `DROP` statement to delete databases and tables.

**Duration:** Approximately 45 minutes

## AWS Service Restrictions

Be aware that access to AWS services and certain actions might be restricted within this lab environment. Stick to the provided instructions to avoid errors.

## Accessing the AWS Management Console

1. Click "Start Lab" at the upper-right corner to launch your lab.
2. Wait until the lab status shows as "ready" before proceeding.

## Task 1: Connect to the Command Host

In this task, you'll connect to an EC2 instance configured with a database client (Command Host). Follow the AWS Management Console steps to connect to the instance and use the terminal to run MySQL commands.

## Task 2: Create a Database and a Table

In this task, you'll perform the following operations:

- Show existing databases.
- Create a new database named "world."
- Verify the creation of the "world" database.
- Create a table named "country" with specified columns.
- Verify the creation of the "country" table.
- Use the `ALTER` statement to correct a column name in the table.

**Challenge 1:** Create a table named "city" and add two columns named "Name" and "Region." Both columns should use the `CHAR` data type.

## Task 3: Delete a Database and Tables

In this task, you'll delete the "city" table and the "world" database. Use the `DROP TABLE` and `DROP DATABASE` commands.

**Challenge 2:** Write a query to drop the "country" table.

## Conclusion

Congratulations! You've successfully:

- Used the `CREATE` statement to create databases and tables.
- Used the `SHOW` statement to view available databases and tables.
- Used the `ALTER` statement to alter the structure of a table.
- Used the `DROP` statement to delete databases and tables.

## Lab Complete

Click "End Lab" at the top of this page and select "Yes" to confirm the end of the lab.

## Additional Resources

- Country, city, and language data: [Statistics Finland](https://www.stat.fi/index_en.html)
- For more information about SQL table operation commands, refer to:
  - [CREATE DATABASE](https://dev.mysql.com/doc/refman/8.0/en/create-database.html)
  - [CREATE TABLE](https://dev.mysql.com/doc/refman/8.0/en/create-table.html)
  - [SHOW Commands](https://dev.mysql.com/doc/refman/8.0/en/show.html)
  - [ALTER TABLE](https://dev.mysql.com/doc/refman/8.0/en/alter-table.html)
  - [DROP DATABASE](https://dev.mysql.com/doc/refman/8.0/en/drop-database.html)
  - [DROP TABLE](https://dev.mysql.com/doc/refman/8.0/en/drop-table.html)

For more information about AWS Training and Certification, visit [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is valuable; share suggestions or corrections through the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. Unauthorized reproduction, redistribution, or commercial use is prohibited.
