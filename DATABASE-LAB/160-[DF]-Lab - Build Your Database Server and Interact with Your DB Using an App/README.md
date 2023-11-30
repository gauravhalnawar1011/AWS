# Build Your DB Server and Interact With Your DB Using an App Lab

## Introduction

Welcome to the "Build Your DB Server and Interact With Your DB Using an App" Lab! In this session, you'll work with Amazon Relational Database Service (Amazon RDS) to create a relational database instance. The lab focuses on launching an RDS DB instance with high availability, configuring the instance to permit connections from your web server, and interacting with the database through a web application.

## Lab Overview and Objectives

This lab aims to reinforce the concept of leveraging an AWS-managed database instance for relational database needs. After completing this lab, you should be able to:

- Launch an Amazon RDS DB instance with high availability.
- Configure the DB instance to permit connections from your web server.
- Open a web application and interact with your database.

**Duration:** Approximately 45 minutes
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b2bda025-e5ec-4be7-bc2a-455ee9897fb6)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/9e12ac78-5913-469a-acec-d59f9407aab8)


## AWS Service Restrictions

Please note that in this lab environment, access to AWS services and certain actions may be restricted. Follow the provided instructions to avoid encountering errors.

## Accessing the AWS Management Console

1. Click "Start Lab" at the upper-right corner to initiate your lab.
2. Wait until the lab status shows as "ready" before proceeding.

## Task 1: Create a Security Group for the RDS DB Instance

In this task, you'll create a security group to allow your web server to access your RDS DB instance. Follow the provided steps in the AWS Management Console to create and configure the security group.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a318c5fe-47c3-4e01-ae1e-1316b0ec9084)

## Task 2: Create a DB Subnet Group

Create a DB subnet group that specifies which subnets can be used for the database. This group requires subnets in at least two Availability Zones. Follow the provided steps in the AWS Management Console to create the DB subnet group.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/02e6b4ae-14cd-4bf4-ba6c-02185ea91388)

## Task 3: Create an Amazon RDS DB Instance

Configure and launch a Multi-AZ Amazon RDS for MySQL database instance. Follow the provided steps to create the RDS DB instance. Wait for the database to be available.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c81edebf-c31d-4f07-80d9-a288c320426d)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b5e3609a-ea1b-4f79-b005-96adf7cf9078)

## Task 4: Interact with Your Database

Open a web application running on your web server and configure it to use the database. Follow the provided steps to interact with the database through the web application.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/5c02666e-df1f-4f62-af2e-80d0647fa542)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/ce2a2347-5c80-4591-9993-2a0dc43f2a0c)

## Conclusion

Congratulations! You've successfully:

- Launched an Amazon RDS DB instance with high availability.
- Configured the DB instance to permit connections from your web server.
- Interacted with the database through a web application.

## Lab Complete

Click "End Lab" at the top of this page and select "Yes" to confirm the end of the lab.

## Additional Resources

- [Amazon RDS FAQs](https://aws.amazon.com/rds/faqs/)
- For more information about AWS Training and Certification, visit [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is valuable; share suggestions or corrections through the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. Unauthorized reproduction, redistribution, or commercial use is prohibited.
