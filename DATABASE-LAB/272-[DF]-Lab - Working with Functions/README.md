# Working with Functions Lab

## Introduction

Welcome to the "Working with Functions" Lab! In this session, you will interact with a relational database named "world" that comprises three tables: city, country, and countrylanguage. Your goal is to write SQL queries using the SELECT statement and WHERE clause, incorporating various common database functions.

## Lab Overview and Objectives

This lab aims to familiarize you with the usage of common database functions in conjunction with the SELECT statement and WHERE clause. By the end of this lab, you should be able to:

- Utilize aggregate functions such as SUM(), MIN(), MAX(), AVG() to summarize data
- Apply the SUBSTRING_INDEX() function to split strings
- Use LENGTH() and TRIM() functions to determine the length of a string
- Employ the DISTINCT() function to filter duplicate records
- Incorporate functions in both the SELECT statement and WHERE clause

- ![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/4820b732-0b6a-4703-9e25-1d0bb3082fe0)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/4600ef78-3b6e-4ea5-9de1-1976a398b271)


**Duration:** Approximately 45 minutes

## AWS Service Restrictions

Be aware that access to AWS services and specific actions might be restricted within this lab environment. Follow the provided instructions to avoid errors.

## Accessing the AWS Management Console

1. Click "Start Lab" at the upper-right corner to initiate your lab.
2. Wait until the lab status shows as "ready" before proceeding.

## Task 1: Connect to the Command Host

In this task, you'll connect to an instance (Command Host) containing a database client, facilitating your connection to a database. Follow the steps in the AWS Management Console to connect to the instance and open a terminal window.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c87ebd39-e5c1-4cbc-909d-7ade85645bc4)

## Task 2: Query the world database

In this task, you will query the "world" database using various SELECT statements and database functions. Functions are employed to process and manipulate data in your queries. You'll explore aggregate functions like SUM(), MIN(), MAX(), AVG(), and others.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/46d86805-3f76-4aa5-98dd-ac357395ef53)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/3ecbf6d6-0cd6-4995-858b-e05b50fccce7)

**Challenge:** Write a query to return rows with "Micronesian/Caribbean" as the name in the region column. The output should split the region into two separate columns: "Region Name 1" and "Region Name 2."

## Conclusion

Congratulations! You've successfully:

- Used aggregate functions to summarize data
- Applied functions like SUBSTRING_INDEX() to split strings
- Utilized LENGTH() and TRIM() functions to analyze string length
- Employed DISTINCT() function to filter duplicate records
- Integrated functions in both the SELECT statement and WHERE clause

## Lab Complete

Click "End Lab" at the top of this page and select "Yes" to confirm the end of the lab.

## Additional Resources

- Country, city, and language data: [Statistics Finland](https://www.stat.fi/index_en.html)
- For more information about SQL functions and operators, refer to:
  - [SELECT statements](https://dev.mysql.com/doc/refman/8.0/en/select.html)
  - [Count function](https://dev.mysql.com/doc/refman/8.0/en/counting-rows.html)
  - [SUM function](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html#function_sum)
  - [AVG function](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html#function_avg)
  - [MIN function](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html#function_min)
  - [MAX function](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html#function_max)
  - [SUBSTRING_INDEX function](https://dev.mysql.com/doc/refman/8.0/en/string-functions.html#function_substring-index)
  - [LENGTH function](https://dev.mysql.com/doc/refman/8.0/en/string-functions.html#function_length)
  - [TRIM function](https://dev.mysql.com/doc/refman/8.0/en/string-functions.html#function_trim)
  - [DISTINCT function](https://dev.mysql.com/doc/refman/8.0/en/distinct-optimization.html)

For more information about AWS Training and Certification, visit [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is valuable; share suggestions or corrections through the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. Unauthorized reproduction, redistribution, or commercial use is prohibited.
