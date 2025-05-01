# 🚀 AWS Capstone Project: Secure, Scalable, Highly Available Web Application

## 📌 Project Overview

This project demonstrates how to build a **highly available, fault-tolerant, and secure web application** on AWS, using managed services and best practices. It utilizes Amazon EC2, RDS, Load Balancer, Auto Scaling, and IAM roles for secure, cost-effective, and scalable architecture.

## 🧱 Architecture Summary

![Architecture Diagram]attached

### 🗂️ Key Components:

- **Amazon EC2 (Auto Scaling)**: Hosts the web application in public subnets across multiple availability zones.
- **Amazon RDS**: Managed relational database hosted in private subnets for enhanced security.
- **Application Load Balancer (ALB)**: Distributes traffic evenly to EC2 instances.
- **NAT Gateway**: Allows private subnet resources to access the internet securely.
- **Internet Gateway**: Enables internet access for public subnet resources.
- **AWS Secrets Manager**: Stores database credentials securely.
- **IAM Roles & Parameter Store**: Manages access control and configuration data.
- **Bastion Host (recommended)**: Provides secure SSH access to private subnet resources.

---

## 🛠️ Features & Best Practices

- ✅ **Highly Available**: EC2 instances are spread across two public subnets in separate availability zones.
- 🔐 **Secure**:
  - RDS instance resides in a private subnet.
  - Application Load Balancer allows only necessary inbound traffic (e.g., port 80).
  - Secrets are securely stored in AWS Secrets Manager.
  - IAM Roles minimize the use of hardcoded credentials.
- ⚙️ **Scalable**: Auto Scaling Group dynamically adjusts capacity based on load.
- 🔄 **Efficient Networking**: Internet Gateway for public traffic, NAT Gateway for private outbound access.

---

## 📊 AWS Cost Estimation

- Use the [AWS Pricing Calculator Estimate](https://calculator.aws/#/estimate?id=3bce2ddb1ee49c4697a5173b8253613f0be7712c) for cost details related to compute, database, and networking resources.

---

## 📝 Recommendations

- Introduce a **Bastion Host** to access private subnets securely via SSH.
- Continue monitoring usage with **CloudWatch** for performance and cost optimization.
- Integrate with **AWS WAF** and **Shield** for additional protection against common web attacks.

---

## 📂 Project Files

- `AWS CAPSTONE PROJECT.pdf` – Summary and architectural justification
- `AWS PROJECT.docx` – Implementation notes and AWS pricing calculator link
- `AWS PROJ.PNG` – Architecture diagram

---

## 📬 Contact

For any queries or feedback, reach out to  
📧 keerthiyalamanchili6@gmail.com

