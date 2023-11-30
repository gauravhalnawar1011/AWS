# Performing a Conditional Search Lab

## Introduction

Welcome to the "Performing a Conditional Search" Lab! In this session, you will work with a relational database named "world" that contains three tables: city, country, and countrylanguage. Your task is to write SQL queries using the SELECT statement and a WHERE clause to search for specific records in the country table.

## Lab Overview and Objectives

This lab aims to demonstrate your ability to use the SELECT statement and a WHERE clause to filter records with a conditional search. By the end of this lab, you should be able to:

- Write a search condition using the WHERE clause
- Utilize the BETWEEN operator
- Employ the LIKE operator with wildcard characters
- Use the AS operator to create a column alias
- Incorporate functions in both the SELECT statement and the WHERE clause

  ![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/0c93ec85-20ed-433a-81df-953a03564b33)

  ![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/51c4a091-2dd8-4f60-907e-1f8497977b5a)



**Duration:** Approximately 45 minutes

## AWS Service Restrictions

Note that access to AWS services and certain actions might be restricted within this lab environment. Follow the provided instructions to avoid errors.

## Accessing the AWS Management Console

1. Click "Start Lab" at the upper-right corner to launch your lab.
2. Wait until the lab status shows as "ready" before proceeding.

## Task 1: Connect to the Command Host

In this task, you'll connect to an Amazon EC2 instance (Command Host) containing a database client, which you'll use to connect to a database. Follow the provided steps in the AWS Management Console to connect to the instance and open a terminal window.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a91adda9-722b-4133-8e93-f4dad67fe768)



## Task 2: Query the world database

In this task, you will query the "world" database using various SELECT statements and database functions. You'll explore conditions using the WHERE clause, the BETWEEN operator, and the LIKE function. Additionally, you'll use column aliases and functions in both SELECT and WHERE.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/df6a7030-83ed-465f-a61e-4bc9d288a380)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/6507dd14-b0f1-478a-83ee-440acbfd9f44)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/d1bf891a-3f75-4dc9-aacd-4da1d7e1124f)


**Challenge:** Write a query to return the sum of the surface area and population of North America.

## Conclusion

Congratulations! You've successfully:

- Used the SELECT statement and a WHERE clause to filter records conditionally.
- Utilized the BETWEEN operator for range conditions.
- Employed the LIKE function with wildcard characters.
- Used the AS operator to create column aliases.
- Incorporated functions in both the SELECT statement and the WHERE clause.

## Lab Complete

Click "End Lab" at the top of this page and select "Yes" to confirm the end of the lab.

## Additional Resources

- Country, city, and language data: [Statistics Finland](https://www.stat.fi/index_en.html)
- For more information about SQL operations, refer to:
  - [WHERE clause](https://dev.mysql.com/doc/refman/8.0/en/where-optimization.html)
  - [BETWEEN operator](https://dev.mysql.com/doc/refman/8.0/en/comparison-operators.html#operator_between)
  - [LIKE function](https://dev.mysql.com/doc/refman/8.0/en/string-comparison-functions.html#operator_like)
  - [SUM function](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html#function_sum)
  - [LOWER function](https://dev.mysql.com/doc/refman/8.0/en/string-functions.html#function_lower)

For more information about AWS Training and Certification, visit [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is valuable; share suggestions or corrections through the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. Unauthorized reproduction, redistribution, or commercial use is prohibited.
