# aws-security-monitoring
Multi-region AWS security monitoring architecture using CloudTrail, CloudWatch Logs, metric filters, and SNS-based alerting.

---

## 📌 Architecture Overview

This project implements a security monitoring baseline in AWS to detect and alert on critical account activities.

### Core Components

- **Amazon EC2** (inside custom VPC)
- **Security Groups**
- **Public & Private Subnets**
- **AWS CloudTrail (Multi-Region)**
- **Amazon S3 (centralized log storage)**
- **CloudWatch Logs**
- **Metric Filters**
- **CloudWatch Alarms**
- **SNS Email Notifications**

---

## 🏗 Architecture Diagram

<img width="1492" height="982" alt="AWS Security Monitoring Architecture (CloudTrail + CloudWatch + SNS) drawio" src="https://github.com/user-attachments/assets/f3d6151c-8ae8-419d-98e5-0610e037b223" />


## 🔎 Security Controls Implemented

### 1️⃣ Root Account Login Detection
- CloudWatch Metric Filter: `RootLogin`
- Alarm triggers when root login occurs
- SNS notification sent immediately

### 2️⃣ IAM Changes Monitoring
- Detects IAM policy modifications
- Alerts on user/role/permission changes

### 3️⃣ Multi-Region Logging
- CloudTrail enabled across all regions
- Log file validation enabled
- Encrypted S3 log storage (SSE-S3)

---

## 🔐 Security Best Practices Applied

- Block Public Access on S3 bucket
- Server-side encryption enabled
- Multi-region CloudTrail
- Log validation enabled
- Least-privilege IAM role for EC2
- CloudWatch log retention configured

---

## 🚀 Future Improvements

- GuardDuty integration
- AWS Config compliance rules
- VPC Flow Logs monitoring
- Security Hub integration
- KMS CMK encryption instead of SSE-S3
- Terraform IaC version

---

## 🧠 Skills Demonstrated

- AWS Security Architecture
- Incident Detection Design
- CloudTrail & Log Analysis
- CloudWatch Monitoring
- Metric Filter Creation
- Alarm & Notification Design
- IAM Security Hardening
- Multi-Region Security Strategy

---

## 📎 Repository Structure
[AWS Security Monitoring Architecture (CloudTrail + CloudWatch + SNS).drawio](https://github.com/user-attachments/files/25316151/AWS.Security.Monitoring.Architecture.CloudTrail.%2B.CloudWatch.%2B.SNS.drawio) # Editable diagram file


<img width="1492" height="982" alt="AWS Security Monitoring Architecture (CloudTrail + CloudWatch + SNS) drawio" src="https://github.com/user-attachments/assets/ed68a257-58df-40ef-a9f2-40274a9e2b47" /> # Exported diagram image


## 📬 About

This project is part of my transition into Cloud & Security Engineering, 
focused on practical AWS security architecture implementation.




