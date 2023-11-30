# Organizing Data Lab

## Introduction

Welcome to the "Organizing Data" Lab! In this session, you'll be working with a relational database named "world" that consists of three tables: city, country, and countrylanguage. The focus of this lab is to create SQL queries using both the GROUP BY and OVER clauses, along with common database functions.

## Lab Overview and Objectives

This lab is designed to help you understand and use the GROUP BY and OVER clauses with some common database functions. By the end of this lab, you should be able to:

- Utilize the GROUP BY clause with the aggregate function SUM()
- Apply the OVER clause with the RANK() window function
- Use the OVER clause with both the aggregate function SUM() and the RANK() window function

**Duration:** Approximately 45 minutes

## AWS Service Restrictions

Please note that in this lab environment, access to AWS services and certain actions may be restricted. Stick to the provided instructions to avoid encountering errors.

## Accessing the AWS Management Console

1. Click "Start Lab" at the upper-right corner to initiate your lab.
2. Wait until the lab status shows as "ready" before proceeding.

## Task 1: Connect to the Command Host

In this task, you'll connect to an instance containing a database client, referred to as the Command Host. Follow the provided steps in the AWS Management Console to connect to the instance and open a terminal window.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/55c7c6e0-4909-4499-bc7f-ba2b7b44ba79)

## Task 2: Query the world database

In this task, you will query the "world" database using various SELECT statements and database functions.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/bec755eb-8ba5-47ca-8b69-3c687b58a2da)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/e26a350f-2eeb-46b4-9708-e10e1d9aca4f)

**Challenge:** Write a query to rank the countries in each region by their population from largest to smallest. Determine whether to use the GROUP BY or OVER grouping clause and either the SUM() or RANK() function.

## Conclusion

Congratulations! You've successfully:

- Used the GROUP BY clause with the aggregate function SUM()
- Applied the OVER clause with the RANK() window function
- Used the OVER clause with both the aggregate function SUM() and the RANK() window function

## Lab Complete

Click "End Lab" at the top of this page and select "Yes" to confirm the end of the lab.

## Additional Resources

- Country, city, and language data: [Statistics Finland](https://www.stat.fi/index_en.html)
- For more information about SQL clauses and database functions, refer to:
  - [GROUP BY clause](https://dev.mysql.com/doc/refman/8.0/en/group-by.html)
  - [OVER clause](https://dev.mysql.com/doc/refman/8.0/en/window-functions.html)
  - [SUM function](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html#function_sum)
  - [RANK function](https://dev.mysql.com/doc/refman/8.0/en/window-functions-regular-functions.html#function_rank)
  - [SELECT statements](https://dev.mysql.com/doc/refman/8.0/en/select.html)
  - [COUNT function](https://dev.mysql.com/doc/refman/8.0/en/counting-rows.html)

For more information about AWS Training and Certification, visit [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is valuable; share suggestions or corrections through the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. Unauthorized reproduction, redistribution, or commercial use is prohibited.
