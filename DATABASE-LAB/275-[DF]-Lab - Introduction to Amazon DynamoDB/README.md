# Introduction to Amazon DynamoDB Lab

## Overview

Welcome to the "Introduction to Amazon DynamoDB" Lab! Amazon DynamoDB is a fast and flexible NoSQL database service that provides consistent, single-digit millisecond latency at any scale. In this lab, you will create a DynamoDB table to store information about a music library, enter data into the table, query the table, and finally, delete the DynamoDB table.

## Topics Covered

In this lab, you will:

1. Create an Amazon DynamoDB table.
2. Enter data into an Amazon DynamoDB table.
3. Query an Amazon DynamoDB table.
4. Modify an existing item.
5. Delete an Amazon DynamoDB table.

**Duration:** Approximately 35 minutes

## Accessing the AWS Management Console

1. Click "Start Lab" at the upper-right corner to initiate your lab.
2. Wait until the lab status shows as "ready" before proceeding.

## Task 1: Create a New Table

In this task, you'll create a new DynamoDB table named "Music" with specified partition and sort keys.

1. Navigate to the AWS Management Console.
2. Under **Services > Database**, choose **DynamoDB**.
3. Click on **Create table**.
4. Enter the following details:
   - **Table name:** Music
   - **Partition key:**
     - **Attribute name:** Artist
     - **Type:** String
   - **Sort key - optional:**
     - **Attribute name:** Song
     - **Type:** String
5. Scroll down and choose **Create table**.
6. Wait for the table to become Active before proceeding.

## Task 2: Add Data

In this task, you'll add data to the Music table.

1. Choose the **Music table**.
2. Click on **Actions > Create item**.
3. Enter details for the first item:
   - **Artist:** Pink Floyd
   - **Song:** Money
   - Add new attributes:
     - **Album:** The Dark Side of the Moon
     - **Year:** 1973
4. Click **Create item**.
5. Repeat the process to add two more items with attributes for John Lennon and Psy.

## Task 3: Modify an Existing Item

In this task, you'll modify an existing item in the DynamoDB table.

1. Navigate to the DynamoDB dashboard.
2. Under **Tables**, choose **Explore Items**.
3. Choose the **Music table**.
4. Locate and choose the item for Psy.
5. Change the **Year** attribute from 2011 to 2012.
6. Click **Save changes**.

## Task 4: Query the Table

In this task, you'll perform a query operation on the DynamoDB table.

1. Choose the **Music table**.
2. Expand **Scan/Query items** and choose **Query**.
3. Enter the following details:
   - **Artist (Partition key):** Psy
   - **Song (Sort key):** Gangnam Style
4. Click **Run** to see the result.
5. Alternatively, try a scan operation by scrolling up and choosing **Scan** with a filter for the year 1971.

## Task 5: Delete the Table

In this task, you'll delete the DynamoDB table along with all its data.

1. In the DynamoDB dashboard, under **Tables**, choose **Update settings**.
2. Choose the **Music table**.
3. Click on **Actions > Delete table**.
4. Enter "delete" for confirmation and choose **Delete table**.

## Conclusion

Congratulations! You have successfully:

- Created an Amazon DynamoDB table.
- Entered data into an Amazon DynamoDB table.
- Queried an Amazon DynamoDB table.
- Modified an existing item.
- Deleted an Amazon DynamoDB table.

## Lab Complete

Click **End Lab** at the top of this page, and then select **Yes** to confirm the end of the lab.

## Additional Resources

For more information about DynamoDB, refer to the [DynamoDB documentation](https://docs.aws.amazon.com/dynamodb/).

## Your Feedback

Your feedback is welcome and appreciated. If you have any suggestions or corrections, please provide details through the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. Unauthorized reproduction, redistribution, or commercial use is prohibited.
