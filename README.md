# 🛒 E-Commerce Website - Hosted on AWS

## 📌 Project Overview

This project involves hosting a **dynamic e-commerce website** on **AWS** using a **highly available, scalable, and fault-tolerant architecture**. The infrastructure follows a **multi-tier design**, leveraging **AWS cloud services** for enhanced security, availability, and performance.

## 🎯 Problem Statement

### **Challenges in Hosting an E-commerce Website**
- **Scalability**: Ensuring the website can handle fluctuating traffic.
- **High Availability**: Preventing downtime and maintaining reliability.
- **Security**: Protecting user data and application infrastructure.
- **Performance Optimization**: Efficiently balancing load and optimizing response times.
- **Automated Deployment & Management**: Reducing manual intervention for resource scaling.

✅ **Solution Implemented:**  
This architecture was designed to **enhance security, scalability, and resilience** using AWS cloud solutions like **VPC, Auto Scaling, Load Balancer, NAT Gateway, RDS, EC2, Route 53, and IAM**.

---

## 🏗️ Architecture Overview

### **🔹 Key AWS Services Used**
- **VPC** - Custom network with private and public subnets.
- **Internet Gateway & NAT Gateway** - Secure internet access for public and private instances.
- **EC2 Instances** - Hosting the web application.
- **Auto Scaling Group** - Automatic scaling based on traffic demands.
- **Application Load Balancer** - Distributing requests to EC2 instances.
- **IAM** - Managing access control and permissions.
- **Amazon RDS** - Managed database service for persistent storage.
- **Amazon S3** - Storing static assets and backups.
- **Amazon Route 53** - Managing DNS records for domain resolution.
- **AWS Certificate Manager** - Enabling HTTPS for secure communication.
- **Amazon SNS** - Sending notifications for scaling events.

📌 **Reference Architecture:**  
![Architecture](3._Host_a_Dynamic_Web_App_on_AWS.png)

---

## 🚀 Deployment Steps

### **1️⃣ Setup Networking**
- Create a **VPC** with **public** and **private subnets** in multiple **Availability Zones**.
- Configure **Internet Gateway** for public access.
- Deploy **NAT Gateway** for private instances to access the internet securely.
- Set up **Security Groups** to manage access.

### **2️⃣ Configure Compute Resources**
- Launch **EC2 instances** in the **private subnets**.
- Set up an **Application Load Balancer** to distribute traffic.
- Create an **Auto Scaling Group** for high availability.

### **3️⃣ Database & Storage**
- Deploy **Amazon RDS** in private subnets.
- Configure **S3** for application storage and backups.

### **4️⃣ Security & Access Management**
- Use **IAM roles and policies** for secure access.
- Enable **SSL/TLS** via **AWS Certificate Manager**.
- Implement **EC2 Instance Connect Endpoint** for secure instance access.

### **5️⃣ Domain & DNS**
- Register a domain using **Amazon Route 53**.
- Configure DNS settings to route traffic efficiently.

### **6️⃣ Monitoring & Alerts**
- Set up **Amazon SNS** to receive alerts for scaling and failures.

---

## 🔧 How to Set Up Locally
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ecommerce-aws.git
   cd ecommerce-aws
2. Deploy infrastructure using Terraform or AWS CloudFormation.
3. Configure the backend and database connection.
4. Deploy the application on EC2 instances.
5. Configure Route 53 for domain resolution.

📊 Key Benefits

✅ High Availability - Uses Multi-AZ deployment and Auto Scaling.
✅ Scalability - Automatically adjusts resources based on demand.
✅ Security - Private subnets, IAM policies, SSL encryption.
✅ Performance Optimization - Load Balancing and NAT Gateway.
✅ Cost Efficiency - Auto Scaling optimizes resource utilization.
