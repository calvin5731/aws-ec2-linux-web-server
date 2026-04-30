# 🚀 AWS EC2 Linux Web Server Deployment

## 📸 Final Result

![Live Website](screenshots/screenshots:19-live-website-browser.png)

> Deployed a Linux-based web server on AWS EC2 and made it accessible through a public IP address.

---

## 💡 Project Overview

This project demonstrates how I deployed a cloud-hosted Linux server using AWS EC2, configured secure access, installed Apache, and hosted a live webpage.

---

## 🛠️ Technologies Used

- AWS EC2
- Amazon Linux 2023
- t3.micro
- SSH
- Key Pair Authentication
- Security Groups
- Apache HTTP Server
- Linux CLI

---

## ⚙️ Deployment Walkthrough

### Step 1: EC2 Dashboard
![EC2 Dashboard](screenshots/screenshots:01-ec2-dashboard.png)

### Step 2: Launch Instance
![Launch Instance](screenshots/screenshots:02-launch-instance-name.png)

### Step 3: Key Pair Section
![Key Pair Section](screenshots/screenshots:03-key-pair-section-main-screen.png)

### Step 4: Create Key Pair
![Key Pair Creation](screenshots/screenshots:04-key-pair-creation-popup.png)

### Step 5: Select Amazon Linux
![Amazon Linux](screenshots/screenshots:05-amazon-linux-selected.png)

### Step 6: Choose Instance Type
![Instance Type](screenshots/screenshots:06-instance-type-selected.png)

### Step 7: Select Key Pair
![Key Pair Selected](screenshots/screenshots:07-key-pair-section.png)

### Step 8: Configure Security Group
![Security Group](screenshots/screenshots:08-network-security-settings.png)

### Step 9: Launch Instance
![Launch Success](screenshots/screenshots:09-instance-launch-success.png)

### Step 10: Instances List
![Instances List](screenshots/screenshots:10-instances-list.png)

### Step 11: Public IP
![Public IP](screenshots/screenshots:11-instance-running-public-ip.png)

### Step 12: EC2 Connect
![EC2 Connect](screenshots/screenshots:12-ec2-connect-page.png)

### Step 13: Terminal Access
![Terminal](screenshots/screenshots:13-terminal-connected.png)

---

## 🐧 Linux Setup

### Step 14: Update System
![System Update](screenshots/screenshots:14-linux-system-update.png)

```bash
sudo yum update -y
