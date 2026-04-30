# 🚀 AWS EC2 Linux Web Server Deployment

## 📸 Final Result

![Live Website](screenshots/screenshots:19-live-website-browser.png)

> Successfully deployed a Linux web server on AWS EC2 and accessed it through a public IP address.

---

## 💡 Project Overview

In this project, I deployed a Linux-based server using AWS EC2. I configured secure access using a key pair, opened required ports using security groups, installed Apache, and hosted a live webpage.

This project demonstrates real-world cloud engineering skills including infrastructure deployment, Linux administration, and web server configuration.

---

## 🛠️ Technologies Used

- AWS EC2  
- Amazon Linux  
- t3.micro instance  
- SSH  
- Key pair authentication  
- Security groups (firewall rules)  
- Apache HTTP Server  
- Linux CLI  

---

## ⚙️ Deployment Walkthrough

### Step 1: EC2 Dashboard
I started in the AWS EC2 dashboard where instances are created and managed.

![EC2 Dashboard](screenshots/screenshots:01-ec2-dashboard.png)

---

### Step 2: Launch Instance
I began creating a new EC2 instance and assigned it a name.

![Launch Instance](screenshots/screenshots:02-launch-instance-name.png)

---

### Step 3: Key Pair Section
I reviewed the key pair section which is used for secure access.

![Key Pair Section](screenshots/screenshots:03-key-pair-section-main-screen.png)

---

### Step 4: Create Key Pair
I created a new key pair to securely connect to the server using SSH instead of a password.

![Key Pair Creation](screenshots/screenshots:04-key-pair-creation-popup.png)

---

### Step 5: Select Amazon Linux
I selected Amazon Linux as the operating system for the instance.

![Amazon Linux](screenshots/screenshots:05-amazon-linux-selected.png)

---

### Step 6: Choose Instance Type
I selected a t3.micro instance because it is free tier eligible and sufficient for this project.

![Instance Type](screenshots/screenshots:06-instance-type-selected.png)

---

### Step 7: Assign Key Pair
I attached the key pair to the instance so I could securely connect later.

![Key Pair Selected](screenshots/screenshots:07-key-pair-section.png)

---

### Step 8: Configure Security Group
I configured firewall rules to allow:
- SSH (port 22) for remote access  
- HTTP (port 80) for web traffic  

![Security Group](screenshots/screenshots:08-network-security-settings.png)

---

### Step 9: Launch Instance
The EC2 instance was successfully launched.

![Launch Success](screenshots/screenshots:09-instance-launch-success.png)

---

### Step 10: Instances List
I navigated to the instances page to confirm the server was running.

![Instances List](screenshots/screenshots:10-instances-list.png)

---

### Step 11: Public IP Address
I copied the public IP address which is used to access the server in a browser.

![Public IP](screenshots/screenshots:11-instance-running-public-ip.png)

---

### Step 12: EC2 Connect
I used EC2 Connect to access the instance through the browser.

![EC2 Connect](screenshots/screenshots:12-ec2-connect-page.png)

---

### Step 13: Terminal Access
I successfully connected to the Linux terminal.

![Terminal](screenshots/screenshots:13-terminal-connected.png)

---

## 🐧 Linux Configuration

### Step 14: Update System
I updated system packages to ensure everything was current.

Command:
sudo yum update -y

![System Update](screenshots/screenshots:14-linux-system-update.png)

---

### Step 15: Install Apache
I installed Apache so the server could host a website.

Command:
sudo yum install httpd -y

![Apache Installed](screenshots/screenshots:15-apache-installed.png)

---

### Step 16: Start Apache
I started Apache and enabled it to run automatically when the system boots.

Commands:
sudo systemctl start httpd  
sudo systemctl enable httpd  

![Apache Started](screenshots/screenshots:16-apache-started-enabled.png)

---

### Step 17: Check Apache Status
I verified Apache was running correctly.

Command:
sudo systemctl status httpd  

![Apache Status](screenshots/screenshots:17-apache-status-running.png)

---

## 🌐 Web Deployment

### Step 18: Create HTML Page
I created a basic HTML file to display a custom webpage.

Example:
<h1>Calvin Trammell - AWS Cloud Project</h1>  
<p>EC2 Linux Web Server Deployment using Apache</p>  

![HTML Page](screenshots/screenshots:18-html-page-created.png)

---

### Step 19: Access Website
I entered the public IP address in a browser and confirmed the web server was working.

![Live Website](screenshots/screenshots:19-live-website-browser.png)

---

## 🧹 Cleanup

### Step 20: Stop Instance
I stopped the instance to avoid unnecessary AWS charges.

![Instance Stopped](screenshots/screenshots:20-instance-stopped.png)

---

## 🧠 What I Learned

- How to deploy a cloud server using AWS EC2  
- How SSH key authentication works  
- How to configure firewall rules using security groups  
- How to install and manage Apache on Linux  
- How to host a live webpage in the cloud  

---

## 📌 Author

Calvin Trammell  
https://github.com/CalvinT57  
https://www.linkedin.com/in/calvin-trammell-56675295  
