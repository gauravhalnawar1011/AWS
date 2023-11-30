# AWS Lab: Scaling and Load Balancing Your Architecture

## Overview

In this lab, you will use Elastic Load Balancing (ELB) and Amazon EC2 Auto Scaling to load balance and automatically scale your infrastructure.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/aa2830b6-319c-4d1a-8764-4071b221bab5)

ELB automatically distributes incoming application traffic across multiple Amazon EC2 instances, providing fault tolerance in your applications.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/03e81a4a-11ac-4d5c-aea0-823e671f61b7)

Auto Scaling helps maintain application availability by automatically scaling your Amazon EC2 capacity based on conditions you define.

## Objectives

After completing this lab, you should be able to:

- Create an Amazon Machine Image (AMI) from an EC2 instance.
- Create a load balancer using Elastic Load Balancing.
- Create a launch template and an Auto Scaling group.
- Configure an Auto Scaling group to scale new instances within private subnets.
- Use Amazon CloudWatch alarms to monitor the performance of your infrastructure.

## Duration

This lab requires approximately 45 minutes to complete.

## Accessing the AWS Management Console

1. Click on [Start Lab](#) to launch your lab.
2. Follow the on-screen instructions to access the AWS Management Console.

## Lab Tasks

### Task 1: Creating an AMI for Auto Scaling

1. Navigate to the EC2 Dashboard.
2. In the left navigation pane, locate and choose "Instances."
3. Select the "Web Server 1" instance.
4. From the "Actions" dropdown list, choose "Image and templates" > "Create image."
5. Configure options for the new AMI and click "Create image."
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/3aa108a2-86cf-4132-8070-a3849677f294)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/97b569bd-4b8c-45db-aae6-6598d21e4c4a)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/e2bacf11-f6c7-4d98-ab51-b496a0cb4eeb)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8a5d8f0c-8b5d-4dcf-a17e-7b6459553c6f)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/29e4f285-dd0a-4ce2-9542-f27ac90b9c74)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/dbbc30f0-7794-45cb-a988-97f5fb502a8a)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8e0cdc1a-4b14-41b7-96f3-f927c2ab2901)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/bfdc8b70-97f5-4005-ad49-bc9259e006ab)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c89b5466-b83f-4214-a538-94de61165bd5)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/fb2d2f47-c012-4e63-9a59-390f41f97409)


## Conclusion

Congratulations! You have successfully completed the lab, achieving the following:

- Created an AMI from an EC2 instance.
- Created a load balancer.
- Created a launch template and an Auto Scaling group.
- Configured an Auto Scaling group to scale new instances within private subnets.
- Used CloudWatch alarms to monitor the performance of your infrastructure.

## Additional Resources

- [Amazon EC2 Auto Scaling Getting Started](#)
- [Getting Started with Elastic Load Balancing](#)

---

© 2023, Amazon Web Services, Inc. or its affiliates. All rights reserved.
