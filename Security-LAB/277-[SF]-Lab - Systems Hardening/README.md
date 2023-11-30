# Systems Hardening with Patch Manager via AWS Systems Manager

## Lab Summary

Welcome to the "Systems Hardening with Patch Manager via AWS Systems Manager" lab! In this lab, you will utilize AWS Systems Manager's Patch Manager to enhance the security of your EC2 instances. The primary focus is on creating and modifying patch baselines, configuring patch groups, and ensuring patch compliance for both Linux and Windows instances.

**Duration:** Approximately 60 minutes

## Lab Environment

The lab environment includes six EC2 instances: three instances with the Linux OS and three with the Windows OS.

### Accessing the AWS Management Console

1. Click on "Start Lab" at the upper-right corner of these instructions.
2. Wait for the lab to be ready (indicated by a green circle).
3. Click on the green circle next to AWS at the top to open the AWS Management Console.

### Important Note

- **Do not change the lab Region unless specifically instructed to do so.**

## Lab Tasks

### **Task 1: Select Patch Baselines**

- Select a patch baseline for Linux instances.
- Create a custom patch baseline for Windows instances.
- Modify patch groups associated with Linux and Windows instances.

### **Task 1.1: Tag Instances**

- Tag Windows instances with "Patch Group: WindowsProd."
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/dd13dad7-7f30-47ea-b286-5912e6243a48)

### **Task 1.2: Create a Custom Patch Baseline**

- Create a custom patch baseline for Windows instances.
- Modify the patch group for the Windows patch baseline.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a5cefe35-ff72-4d4c-babb-4830cdce346f)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8249a9f6-a20e-4214-9e68-f09dc89ee36e)

### **Task 2: Configure Patching**
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/ee110d93-5fc4-4b09-a4a9-6c1ccd3aedd5)

#### **Task 2.1: Patch the Linux Instances**

- Use Patch Now to scan and install patches for Linux instances.
- Monitor the progress of the patching operation.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/78983484-16c9-481e-b41e-212ed2def6f8)

#### **Task 2.2: Patch the Windows Instances**

- Use Patch Now to scan and install patches for Windows instances.
- Verify the details using the Systems Manager document.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8528aa19-266b-47b4-9f55-8468fdc036c1)


#### **Task 2.3: Verify Compliance**

- Verify compliance for both Linux and Windows instances.
- Explore the Compliance Reporting tab for an overview of all instances.
- Check the patch details for a Windows instance.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/17cde654-09cf-492b-8b69-e280e6ae6f52)
## Lab Completion

Congratulations! You have successfully:

- Created a custom patch baseline.
- Modified patch groups for Linux and Windows instances.
- Configured patching and patched instances.
- Verified patch compliance for all EC2 instances.

### Ending the Lab

- Click on "End Lab" at the top of this page.
- Confirm that you want to end the lab by selecting "Yes."

An "Ended AWS Lab Successfully" message will be briefly displayed.

### Additional Resources

- For more information about AWS Training and Certification, see [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is welcome and appreciated. If you have any suggestions or corrections, please provide the details in the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2023 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.
