Create an S3 Bucket:

Log in to your AWS account or create one if you don't have an AWS account.
Open the Amazon S3 console.
Click "Create bucket."
Choose a globally unique bucket name and select the region for your bucket.
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/ae9d2bd1-5dce-49c1-98dc-0876b85d28be)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b9db9979-8123-4b1a-8d09-e1f4f5e960e1)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c0f4a7da-e310-41d7-945e-d8aa41ae4dd4)
enable the static website hosting
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/c72da279-632b-480e-8591-facd86430ba1)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/cc6790ca-4943-4ff4-8733-30e430f24468)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/ca326d8c-15c0-4f05-b6fc-43c8922fa766)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/3a92c74a-a2c3-440d-99a0-174602ec6bab)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/fa7b11b7-68f4-4213-b771-d2e5af485521)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/0229de1e-b612-452e-8946-34c59aa3e62d)
make sure you Add te /* in the policy genereter resoucre at the end
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/579baa4c-0f7c-4291-916b-21c72800b64c)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/7fc1920a-7cb7-4479-9d26-9a5873f2b141)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/19b8945e-d58d-40a3-a34f-c78d1f1ce6a9)

Upload Your Website Files:

In your S3 bucket, navigate to the "Properties" tab.
Enable "Static website hosting."
Set the index document and error document (e.g., index.html and error.html).
Upload your static website files to the S3 bucket. You can do this manually through the AWS Management Console or use the AWS CLI.

Configure Permissions:

In your S3 bucket, go to the "Permissions" tab.
Set the bucket policy to allow public read access. You can use the following policy as an example

Make sure to replace "your-bucket-name" with your actual bucket name.
