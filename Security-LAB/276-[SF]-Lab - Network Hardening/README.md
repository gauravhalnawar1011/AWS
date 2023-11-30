# Network Hardening Using Amazon Inspector and AWS Systems Manager

## Lab Summary

Welcome to the "Network Hardening Using Amazon Inspector and AWS Systems Manager" lab! In this lab, you play the role of a new security engineer for AnyCompany. Your task is to identify weak areas in the company's network security and update AnyCompany's environment for better efficiency and optimization. You will utilize Amazon Inspector to perform an agentless network audit on your EC2 instances, analyze the findings, and update security groups. Additionally, you will replace the BastionServer with Systems Manager to enhance security.

**Duration:** Approximately 45 minutes

## Lab Environment

The lab environment includes two EC2 instances: a bastion server named BastionServer in a public subnet and an application server named AppServer in a private subnet.

### Accessing the AWS Management Console

1. Click on "Start Lab" at the upper-right corner of these instructions.
2. Wait for the lab to be ready (indicated by a green circle).
3. Click on the green circle next to AWS at the top to open the AWS Management Console.

### Important Note

- **Do not change the lab Region unless specifically instructed to do so.**

## Lab Tasks

### **Task 1: View EC2 instances and add tags**

- Tag the BastionServer instance with the key-value pair: `SecurityScan: true`.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a63f8346-9561-46ff-9c80-d6ad984234e5)

### **Task 2: Configure and run Amazon Inspector**

- Configure an assessment target for Amazon Inspector to assess using network reachability.
- Create an assessment template and run an agentless network audit.
- Analyze the findings generated by the network audit.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b45866d9-5471-4c9f-a4ed-0e43d0ba171d)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/2996b199-2e48-4b9a-ad53-e8684a53c024)

### **Task 3: Analyze Amazon Inspector findings**

- Review high and medium-severity findings generated by Amazon Inspector.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/17990fc0-523e-48d5-8ffe-5ad063df6359)

### **Task 4: Update security groups**

- Update the security group associated with the BastionServer to restrict access.
- Re-scan the environment to verify the changes.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a34144bb-e1c0-4a3b-a93f-b70a07e52776)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/0913a9af-cfc8-472e-aa04-ccc7d397798e)

### **Task 5: Replace BastionServer with Systems Manager**

- Remove the SSH inbound rule for BastionServer.
- Stop the BastionServer instance.
- Connect directly to AppServer using AWS Systems Manager Session Manager.
- Final scan of the environment to verify security improvements.

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/4b0f1687-2847-4562-8701-a6581491cff4)

![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/57b6bee1-c427-41ab-a9f3-f923a8c70b68)

## Lab Completion

Congratulations! You have successfully:

- Configured Amazon Inspector.
- Run an agentless network audit.
- Investigated the scan results.
- Updated security groups.
- Logged in to an application server using Session Manager.

### Ending the Lab

- Click on "End Lab" at the top of this page.
- Confirm that you want to end the lab by selecting "Yes."

An "Ended AWS Lab Successfully" message will be briefly displayed.

### Additional Resources

- For more information about AWS Training and Certification, see [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is welcome and appreciated. If you have any suggestions or corrections, please provide the details in the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.