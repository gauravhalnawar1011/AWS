You can host a static website using Amazon EC2 by configuring a web server like Apache or Nginx on your EC2 instance and then uploading your website files to the server. Here are the steps to host a static website on EC2:

1. **Launch an EC2 Instance**:

   - Log in to your AWS account.
   - Navigate to the EC2 dashboard.
   - Click "Launch Instance" to create a new EC2 instance.
   - Choose an Amazon Machine Image (AMI). A Linux-based AMI, such as Amazon Linux or Ubuntu, is a good choice.
   - Select an instance type based on your website's traffic and resource requirements.
   - Configure the instance details, including the network settings, instance type, and storage options.
   - Add tags and configure security groups and key pairs as needed.
   - Review your settings and launch the instance.

2. **Connect to Your EC2 Instance**:

   - Once your EC2 instance is running, you'll need to connect to it using SSH. Use the private key associated with the key pair you selected during instance setup.
   - You can connect using a terminal with a command like:

     ```bash
     ssh -i "your-key-pair.pem" ec2-user@your-instance-public-ip
     ```

3. **Install a Web Server**:

   - Update the package repository on your EC2 instance:

     ```bash
     sudo yum update (for Amazon Linux)
     # or
     sudo apt update (for Ubuntu)
     ```

   - Install a web server, such as Apache or Nginx:

     For Apache:

     ```bash
     sudo yum install httpd (for Amazon Linux)
     # or
     sudo apt install apache2 (for Ubuntu)
     ```

     For Nginx:

     ```bash
     sudo yum install nginx (for Amazon Linux)
     # or
     sudo apt install nginx (for Ubuntu)
     ```

   - Start the web server and set it to run at startup:

     ```bash
     sudo systemctl start httpd (for Apache)
     # or
     sudo systemctl start nginx (for Nginx)
     sudo systemctl enable httpd (for Apache)
     # or
     sudo systemctl enable nginx (for Nginx)
     ```

4. **Upload Your Website Files**:

   - Use SCP or SFTP to upload your static website files to your EC2 instance. You can use a tool like `scp` or a graphical SFTP client like FileZilla.

     Example using `scp`:

     ```bash
     scp -i "your-key-pair.pem" -r /path/to/your/local/files/ ec2-user@your-instance-public-ip:/var/www/html/
     ```

5. **Configure Domain or IP**:

   - Point your domain's DNS to your EC2 instance's public IP address if you have a custom domain.

6. **Access Your Website**:

   - Open a web browser and enter your EC2 instance's public IP or your domain name to access your static website.

Your static website should now be hosted on your Amazon EC2 instance. Be sure to manage security, backup, and other configurations as needed for your specific use case.
