# Data Protection Using Encryption

## Lab Summary

Welcome to the "Data Protection Using Encryption" lab! In this hands-on experience, you will explore cryptography and encryption techniques in the context of AWS. Specifically, you will connect to a file server hosted on an Amazon EC2 instance and configure the AWS Encryption Command Line Interface (CLI) to encrypt and decrypt data. The lab focuses on using the AWS Key Management Service (KMS) for key management and encryption.

**Duration:** Approximately 45 minutes

## Lab Environment

The lab environment includes one preconfigured EC2 instance named "File Server." An AWS Identity and Access Management (IAM) role is attached to enable connection to the instance using the AWS Systems Manager Session Manager.

### Accessing the AWS Management Console

1. Click on "Start Lab" at the upper-right corner of these instructions.
2. Wait for the lab to be ready (indicated by a green circle).
3. Click on the green circle next to AWS at the top to open the AWS Management Console.

### Important Note

- **Do not change the lab Region unless specifically instructed to do so.**

## Lab Tasks

### **Task 1: Create an AWS KMS Key**

- Create a symmetric AWS KMS key.
- Configure key labels and permissions.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/e7edb56f-8695-4220-8352-d66fc0f8bee8)

### **Task 2: Configure the File Server Instance**

- Configure AWS credentials on the File Server EC2 instance.
- Install the AWS Encryption CLI.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/512ec120-faff-4a77-8889-add9610131e0)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/314a4771-257d-4827-85de-83800e8404f0)

### **Task 3: Encrypt and Decrypt Data**

- Create a text file with mock sensitive data.
- Encrypt the file using AWS KMS key.
- Decrypt the encrypted file and view its contents.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/9f3e266d-7979-49b3-bc08-9bec098f681b)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/db6c6c77-388a-4d74-9dad-34d3d9a0b7be)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/628510c9-5e27-4aa7-8cfe-6a61aea22515)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c10a3776-e68d-474a-9be0-b7e8262e2c3a)

## Lab Completion

Congratulations! You have successfully:

- Created an AWS KMS encryption key.
- Installed the AWS Encryption CLI.
- Encrypted plaintext data.
- Decrypted ciphertext.

### Ending the Lab

- Click on "End Lab" at the top of this page.
- Confirm that you want to end the lab by selecting "Yes."

An "Ended AWS Lab Successfully" message will be briefly displayed.

### Additional Resources

- For more information about AWS Training and Certification, see [AWS Training and Certification](https://aws.amazon.com/training/).

Your feedback is welcome and appreciated. If you have any suggestions or corrections, please provide the details in the [AWS Training and Certification Contact Form](https://www.aws.training/ContactUs).

© 2022 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.
