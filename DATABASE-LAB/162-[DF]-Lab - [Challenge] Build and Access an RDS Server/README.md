# Challenge Lab: Build Your DB Server and Interact With Your DB

## Challenge Description

Welcome to the Challenge Lab: Build Your DB Server and Interact With Your DB! This lab is designed to reinforce the concept of leveraging an AWS-managed database instance for solving relational database needs using Amazon Relational Database Service (Amazon RDS). After completing this challenge, you should be able to:

1. Launch an Amazon RDS DB instance using either Amazon Aurora Provisioned DB or MySQL database engines.
2. Use the Amazon RDS Query Editor to query data.

**Duration:** Approximately 45 minutes

## Challenge Steps

### Step 1: Launch an Amazon RDS DB Instance

1. Launch an Amazon RDS DB instance using either Amazon Aurora Provisioned DB or MySQL database engines.
   - Choose a supported engine: Amazon Aurora or MySQL.
   - Template: Choose Dev/Test or Free tier.
   - Availability and durability: Avoid creating a standby instance.
   - DB instance size: Choose Burstable classes (db.t2 and db.t3 instances) of type db.t*.micro to db.t*.medium.
   - Storage: Choose General Purpose SSD (gp2) of a size up to 100 GB. Provisioned IOPS access is restricted.
   - Amazon VPC: Use the Lab VPC.
   - Security Group: Include a security group that will allow the LinuxServer to connect to the RDS instance.
   - For MySQL, under Additional configuration - Enable Enhanced monitoring - Disable the option.
   - Purchasing Options: On-Demand instances are allowed. Other purchasing options are disabled.
   - Click the "Details" followed by "Show."
   - Download PEM (for Linux or macOS) or Download PPK (for Windows) depending on your local operating system.
   - Make a note of the LinuxServer address.

### Step 2: Connect to LinuxServer and Install MySQL Client

2. Connect (SSH) to the LinuxServer using the details you made a note of.
3. Install a MySQL client and use it to connect to your database. Refer to [MySQL Client documentation](https://dev.mysql.com/doc/mysql-shell/8.0/en/) for assistance.

### Step 3: Create Table RESTART and Insert Sample Rows

4. Create a table named RESTART with the following columns:
   - Student ID (Number)
   - Student Name
   - Restart City
   - Graduation Date (Date Time)
   - Capture a screenshot for submission.
5. Insert 10 sample rows into the RESTART table.
   - Capture a screenshot for submission.

### Step 4: Select All Rows from Table RESTART

6. Select all rows from the RESTART table.
   - Capture a screenshot for submission.

### Step 5: Create Table CLOUD_PRACTITIONER and Insert Sample Rows

7. Create a table named CLOUD_PRACTITIONER with the following columns:
   - Student ID (Number)
   - Certification Date (Date Time)
   - Capture a screenshot for submission.
8. Insert 5 sample rows into the CLOUD_PRACTITIONER table.
   - Capture a screenshot for submission.

### Step 6: Select All Rows from Table CLOUD_PRACTITIONER

9. Select all rows from the CLOUD_PRACTITIONER table.
    - Capture a screenshot for submission.

### Step 7: Perform Inner Join and Display Results

10. Perform an inner join between the two tables created above (RESTART and CLOUD_PRACTITIONER).
    - Display Student ID, Student Name, Certification Date.
    - Capture a screenshot for submission.

## Lab Complete

Congratulations! You have completed the Challenge Lab. When you are finished:

- Click **End Lab** at the top of this page.
- Click **Yes** to confirm that you want to end the activity.

A panel will appear, indicating that "DELETE has been initiated... You may close this message box now." Click the X in the top right corner to close the panel.

## Additional Resources

For more information about AWS Training and Certification, see [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is welcome and appreciated. If you would like to share any suggestions or corrections, please provide the details in our [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.
