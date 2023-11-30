# Working with Amazon EBS

## Overview

Amazon Elastic Block Store (Amazon EBS) is a scalable, high-performance block-storage service designed for Amazon Elastic Compute Cloud (Amazon EC2). In this lab, you will learn how to create an EBS volume and perform various operations such as attaching it to an instance, creating a file system, and taking a snapshot backup.

![EBS Lab Overview](link-to-image)

## Objectives

By the end of this lab, you will be able to:

- Create an EBS volume.
- Attach and mount an EBS volume to an EC2 instance.
- Create a snapshot of an EBS volume.
- Create an EBS volume from a snapshot.

## Duration

This lab requires approximately 45 minutes to complete.

## Accessing the AWS Management Console

1. Click on [Start Lab](#) to launch your lab.
2. Follow the on-screen instructions to access the AWS Management Console.

Ensure that AWS lab resources are ready before proceeding.

## Lab Tasks

### Task 1: Creating a new EBS volume

1. Open the EC2 Management Console.
2. In the left navigation pane, choose "Instances."
3. Note the Availability Zone for the Lab instance.
4. In the left navigation pane, under Elastic Block Store, choose "Volumes."
5. Choose "Create volume" and configure the options.
6. Refresh the page to see your new volume.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8e595d4d-86e7-4bf2-848c-47a0401c6941)

### Task 2: Attaching the volume to an EC2 instance

1. Select the created volume.
2. From the "Actions" menu, choose "Attach volume."
3. Choose the Lab instance from the dropdown list.
4. The Volume state of your new volume should change to In-use.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/6c969d16-0b56-47bc-bb1e-821091a3a42c)

### Task 3: Connecting to the Lab EC2 instance

1. Open the EC2 Management Console.
2. Choose "Instances" from the navigation pane.
3. Select the Lab instance.
4. Choose "Connect" and open the EC2 Instance Connect tab.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/546baf80-464d-4d97-a701-cd0a17afcca9)

### Task 4: Creating and configuring the file system

Use commands in the EC2 Instance Connect terminal:

```bash
df -h
sudo mkfs -t ext3 /dev/sdf
sudo mkdir /mnt/data-store
sudo mount /dev/sdf /mnt/data-store
echo "/dev/sdf   /mnt/data-store ext3 defaults,noatime 1 2" | sudo tee -a /etc/fstab
cat /etc/fstab
df -h
sudo sh -c "echo some text has been written > /mnt/data-store/file.txt"
cat /mnt/data-store/file.txt
```
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/d2b9070f-cda2-4424-9b77-98ff4c5d638d)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a6b18d64-1a60-4e2b-a221-b032d84c5b5c)

### Task 5: Creating an Amazon EBS snapshot

1. In the EC2 Management Console, choose "Volumes" and select My Volume.
2. From the "Actions" menu, choose "Create snapshot."
3. In the Tags section, add a tag.
4. Choose "Create snapshot."
5. In the left navigation pane, choose "Snapshots."
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/7f5ba91b-32ef-4d25-87fe-512f7fc4217e)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8cbbc8b5-9b3e-4f02-8e74-b872c3a31e89)

### Task 6: Restoring the Amazon EBS snapshot

#### Task 6.1: Creating a volume by using the snapshot

1. In the EC2 Management Console, select My Snapshot.
2. From the "Actions" menu, choose "Create volume from snapshot."
3. Configure the options and choose "Create volume."
4. In the left navigation, choose "Volumes."
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/2a505dd8-da4c-4b91-8fee-679d498e01d4)

#### Task 6.2: Attaching the restored volume to the EC2 instance

1. Select the Restored Volume.
2. From the "Actions" menu, choose "Attach volume."
3. Choose the Lab instance from the dropdown list.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8dec7e33-f07f-4fe0-9102-77b3f55242fd)

#### Task 6.3: Mounting the restored volume

Use commands in the EC2 Instance Connect terminal:

```bash
sudo mkdir /mnt/data-store2
sudo mount /dev/sdg /mnt/data-store2
ls /mnt/data-store2/file.txt
```
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/7a947c1b-61b5-408e-880e-78a5e145996c)

## Conclusion

Congratulations! You have successfully:

- Created an EBS volume.
- Attached and mounted an EBS volume to an EC2 instance.
- Created a snapshot of an EBS volume.
- Created an EBS volume from a snapshot.

## Lab Complete

Congratulations! You have completed the lab.

Click "End Lab" at the top of this page, then choose "Yes" to confirm the end of the lab.

---

**Additional Resources:**
- [Amazon Elastic Block Store (Amazon EBS)](link-to-ebs-docs)
- [Connect to Your Linux Instance](link-to-connect-docs)
- For more information about AWS Training and Certification, see [AWS Training and Certification](link-to-training-certification).
- Your feedback is welcome and appreciated. If you have suggestions or corrections, provide details in the [AWS Training and Certification Contact Form](link-to-contact-form).

© 2023, Amazon Web Services, Inc. or its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.
