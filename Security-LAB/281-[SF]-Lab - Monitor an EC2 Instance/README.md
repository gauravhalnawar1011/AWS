# Monitoring an EC2 Instance Lab

## Lab Overview

Logging and monitoring are crucial for maintaining optimal system performance and security. In this lab, you will create an Amazon CloudWatch alarm to monitor the CPU utilization of an Amazon Elastic Compute Cloud (Amazon EC2) instance. Additionally, you'll set up an Amazon Simple Notification Service (Amazon SNS) notification to receive alerts via email when the CPU utilization exceeds a specific threshold. A stress test will be conducted on the EC2 instance to trigger the CloudWatch alarm, simulating a scenario where CPU usage spikes, possibly due to malicious activity.

### Objectives

After completing this lab, you should be able to:

1. Create an Amazon SNS notification
2. Configure a CloudWatch alarm
3. Stress test an EC2 instance
4. Confirm the receipt of an Amazon SNS email notification
5. Create a CloudWatch dashboard

**Duration:** Approximately 60 minutes

## Lab Environment

- Preconfigured EC2 instance named "Stress Test"
- AWS Systems Manager session manager for connecting to the EC2 instance
- Amazon CloudWatch for monitoring
- Amazon SNS for notifications

**Note:** Backend components, including EC2, IAM roles, and some AWS services, are prebuilt into the lab environment.

## Accessing the AWS Management Console

1. Click **Start Lab** at the upper-right corner.
2. Wait for the lab to be ready (indicated by a green circle).
3. Click the AWS icon at the top to open the AWS Management Console.

**Note:** Do not change the lab Region unless instructed.

## Task 1: Configure Amazon SNS

1. In the AWS Management Console, search for "SNS" and choose **Simple Notification Service**.
2. Click the **Create topic** button.
3. Configure the topic with the following details:
   - **Type:** Standard
   - **Name:** MyCwAlarm
4. Click **Create topic**.
5. On the topic details page, choose the **Subscriptions** tab and then click **Create subscription**.
6. Configure the subscription:
   - **Topic ARN:** Leave default
   - **Protocol:** Email
   - **Endpoint:** Enter a valid email address
7. Click **Create subscription**.
8. Open the confirmation email sent to your provided email address and click **Confirm subscription**.
9. Go back to the AWS Management Console, navigate to **Subscriptions**, and confirm that the status is now **Confirmed**.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c33be02a-c8a0-42f8-b881-a5241db60597)

**Summary of Task 1:**
You created an SNS topic and subscribed to it using an email address, enabling the topic to send alerts to the specified email.

## Task 2: Create a CloudWatch Alarm

1. In the AWS Management Console, search for "CloudWatch" and choose it.
2. In the left navigation pane, choose **Metrics** > **All metrics**.
3. Choose **EC2** > **Per-Instance Metrics**.
4. Select the checkbox next to **CPUUtilization** for the "Stress Test" instance.
5. Choose **Create alarm**.
6. Choose **Select metric**, then **EC2** > **Per-Instance Metrics**, and select the checkbox for **CPUUtilization**.
7. Configure the alarm:
   - **Threshold type:** Static
   - **Threshold value:** 60
8. Choose **Next**.
9. Configure the notification:
   - **Alarm state trigger:** In alarm
   - **Select an SNS topic:** MyCwAlarm
10. Choose **Next** and configure the alarm details:
    - **Alarm name:** LabCPUUtilizationAlarm
    - **Alarm description:** CloudWatch alarm for Stress Test EC2 instance CPUUtilization
11. Choose **Next** and then **Create alarm**.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b534d562-52da-46c7-a008-16eede871ca5)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/9168c0dc-081f-4fe0-9a95-a78bec9cadb2)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/48cdd5ec-6a50-4320-910e-26135bea573f)

**Summary of Task 2:**
You created a CloudWatch alarm that triggers when the CPU utilization of the "Stress Test" instance exceeds 60%, sending a notification to the specified SNS topic.

## Task 3: Test the CloudWatch Alarm

1. Navigate to the Vocareum console and click **AWS Details**.
2. Copy the URL next to **EC2InstanceURL** and open it in a new browser tab.
3. Run the following command in the EC2 instance to increase CPU load:
   ```
   sudo stress --cpu 10 -v --timeout 400s
   ```
4. Return to the AWS console and go to **CloudWatch Alarms**.
5. Monitor the graph and refresh every minute until the alarm status is **In alarm**.
6. Check your email inbox for the Amazon SNS notification confirming the alarm.

**Summary of Task 3:**
You simulated a scenario where the EC2 instance experienced a spike in CPU utilization, triggering the CloudWatch alarm and receiving an email notification.

## Task 4: Create a CloudWatch Dashboard

1. In the AWS Management Console, go to **CloudWatch** > **Dashboards**.
2. Choose **Create dashboard**.
3. Enter the dashboard name as "LabEC2Dashboard" and choose **Create dashboard**.
4. Choose **Line** > **Metrics** > **EC2** > **Per-Instance Metrics**.
5. Select the checkbox for **Stress Test** for the instance name and **CPUUtilization** for the metric name.
6. Choose **Create widget** and then **Save dashboard**.

**Lab Summary:**
In this lab, you created a CloudWatch alarm to monitor CPU utilization on an EC2 instance, configured an SNS notification for alerts, performed a stress test to trigger the alarm, and confirmed the notification. Additionally, you created a CloudWatch dashboard for quick access to relevant metrics.

**Conclusion:**
Congratulations! You have successfully completed the lab, gaining practical experience in monitoring and alerting with AWS services.

**Lab Complete:**
Click **End Lab** at the top of this page and confirm with **Yes** to end the lab.
