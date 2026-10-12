# AWS Custom VPC & Cloud Networking Architecture

## 📌 Project Overview
This project demonstrates the design and deployment of a custom Amazon Virtual Private Cloud (VPC) architecture built from scratch. It establishes a secure network foundation following AWS best practices, featuring network segmentation using public and private subnets, internet connectivity via Internet Gateway, and secure outbound connectivity for private resources via a NAT Gateway.
---

## 🏗️ Architecture Architecture & Network Specifications

- **VPC CIDR Block:** `10.0.0.0/16`
- **Public Subnet:** `10.0.1.0/24` (Auto-assign public IP enabled)
- **Private Subnet:** `10.0.2.0/24`
- **Internet Gateway (IGW):** Attached to the VPC for direct internet access.
- **NAT Gateway:** Deployed in the Public Subnet with an Elastic IP (EIP) for secure outbound connectivity.
- **Route Tables:** 
  * `public-route-table`: Routes `0.0.0.0/0` traffic to Internet Gateway.
  * `private-route-table`: Routes `0.0.0.0/0` traffic to NAT Gateway.

---

## 📸 Implementation Screenshots

### 1. Subnets Configuration
![Subnets Configuration]<img width="1907" height="973" alt="vpc ss" src="https://github.com/user-attachments/assets/a279bf66-08ea-4e90-a09e-d3acc032004a" />


### 2. Route Table Configuration
![Route Table Configuration] <img width="1902" height="917" alt="route table ss" src="https://github.com/user-attachments/assets/9edb4eaf-51d7-4262-b244-8ce7068e91ec" />


### 3. NAT Gateway Setup
![NAT Gateway Setup]<img width="1918" height="923" alt="nat gateway" src="https://github.com/user-attachments/assets/6b77b31b-07a2-45d2-9881-ce3d4f963553" />
---
## 🎯 Key Takeaways
- Mastered hands-on configuration of core AWS Cloud Networking components.
- Implemented secure network isolation using public/private subnets and route table configurations.
- Configured one-way outbound internet access for private network resources using NAT Gateway.
