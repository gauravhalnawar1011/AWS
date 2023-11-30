# AWS Identity and Access Management (IAM) Lab

## Overview

Cryptography is the conversion of communicated information into secret code that keeps the information confidential and private. In this lab, you will explore users, user groups, and policies in the AWS Identity and Access Management (IAM) service.

### Objectives

After completing this lab, you should be able to:

- Create and apply an IAM password policy
- Explore pre-created IAM users and user groups
- Inspect IAM policies as applied to the pre-created user groups
- Add users to user groups with specific capabilities active
- Locate and use the IAM sign-in URL
- Experiment with the effects of policies on service access

### Duration

This lab requires approximately 60 minutes to complete.

## Accessing the AWS Management Console

1. Click on the "Start Lab" button to access the AWS Management Console.
2. Wait for the lab to be ready before proceeding.

...

### Task 1: Create an account password policy

In this task, you create a custom password policy for your AWS account.

1. Open the IAM service in the AWS Management Console.
2. In the left navigation pane, choose **Account settings**.
3. Choose **Change password policy**.
4. Under **Select your account password policy requirements**, configure the desired options.
5. Choose **Save changes**.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c4560124-3afd-4c4f-9df3-055881e858b1)

...

### Task 2: Explore users and user groups

In this task, you explore the pre-created IAM users and user groups.

1. Open the IAM service in the AWS Management Console.
2. Explore IAM users, user groups, and policies.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/4ff071ca-6a33-4575-b4f5-f0fe5b939927)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/2b1e238f-d05f-4e5c-8f52-a2cd2235fa26)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/2e555cdd-878a-48d5-ba93-fd23b1b943c4)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/61c19a26-c506-4ce0-94cf-5c290aed1c47)

...

### Business scenario

For the remainder of this lab, you work with these users and user groups to activate permissions supporting the following business scenario:

| User  | In Group     | Permissions                       |
|-------|--------------|-----------------------------------|
| user-1| S3-Support   | Read-only access to Amazon S3      |
| user-2| EC2-Support  | Read-only access to Amazon EC2     |
| user-3| EC2-Admin     | View, start, and stop EC2 instances|

### Task 3: Add users to user groups

You have recently hired users into different roles. In this task, you add them to the corresponding IAM user groups.

1. Add user-1 to the S3-Support group.
2. Add user-2 to the EC2-Support group.
3. Add user-3 to the EC2-Admin group.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/3270368e-6896-458b-ae8d-3eb25408e7aa)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/dd778791-8b3b-4003-aa90-882cc4e171fd)

...

### Task 4: Sign in and test user permissions

In this task, you test the permissions of each IAM user.

1. Copy the IAM sign-in URL.
2. Open a private window and sign in as each user to test their permissions.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/bec0beba-6d16-479c-931a-f2b9eccd61ab)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/d321d805-7a37-474e-a3b7-0b4479d2b898)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/714ce950-d78e-4c13-ab33-117bcb568d05)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/f35ed4b9-58f7-4116-9375-d7d457779ead)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/2ee8d858-7042-42c7-baa5-3771794fb539)

...

## Conclusion

Congratulations! You have successfully completed the lab, including creating and applying an IAM password policy, exploring IAM users and user groups, inspecting IAM policies, adding users to groups, and testing user permissions.

## Lab Complete

Choose **End Lab** at the top of this page to conclude the lab.

---
*For more information about AWS Training and Certification, see [AWS Training and Certification](https://aws.amazon.com/training/).*

*Your feedback is welcome and appreciated. If you would like to share any suggestions or corrections, please provide the details in our [AWS Training and Certification Contact Form](https://www.aws.training/Support).*
