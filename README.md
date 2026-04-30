# AWS EC2 Linux Web Server Deployment

## Project Overview

This project demonstrates how I deployed a Linux web server on Amazon Web Services using an EC2 instance. I launched a t3.micro Linux instance, configured key pair access, adjusted the security group, connected to the instance, installed Apache, and verified the web server from a browser using the public IP address.

This project helped me practice basic cloud engineering skills such as EC2 deployment, SSH access, Linux commands, web server installation, and cloud security group configuration.

## Tools and Services Used

- Amazon Web Services
- EC2
- Amazon Linux
- t3.micro instance
- SSH
- Key pair authentication
- Security Groups
- Apache HTTP Server
- GitHub

## Skills Demonstrated

- Creating and launching an EC2 instance
- Selecting an Amazon Linux image
- Choosing a t3.micro instance type
- Creating or using an existing key pair
- Configuring inbound security group rules
- Connecting to Linux through SSH
- Installing and starting Apache
- Testing a web server through a browser
- Documenting a cloud project for a technical portfolio

## Project Steps

### 1. Launched an EC2 Instance

I started by creating a new EC2 instance in AWS. I selected a Linux image and used the t3.micro instance type because it is a lightweight option that works well for basic cloud practice.

![EC2 Launch](screenshots/screenshots:02-launch-instance-name.png)

### 2. Selected or Created a Key Pair

I used a key pair to securely connect to the EC2 instance through SSH. This is important because AWS uses key based authentication instead of a regular username and password.

![Key Pair](screenshots/screenshots:03-key-pair-section-main-screen.png)

### 3. Configured Security Group Rules

I configured the security group so the instance could allow SSH traffic for remote access and HTTP traffic so the web page could be viewed in a browser.

![Security Group](screenshots/screenshots:08-network-security-settings.png)

### 4. Launched the Instance

After reviewing the instance settings, I launched the EC2 instance successfully.

![Launch Success](screenshots/screenshots:09-instance-launch-success.png)

### 5. Connected to the Linux Instance

Once the instance was running, I connected to it using SSH. This allowed me to manage the Linux server from the command line.

![SSH Connection](screenshots/screenshots:13-terminal-connected.png)

### 6. Installed Apache Web Server

After connecting to the instance, I installed Apache so the EC2 instance could serve a basic webpage.

```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
