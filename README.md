# AWS Custom VPC & Cloud Networking Architecture

## 📌 Project Overview
This project demonstrates the design and deployment of a custom Amazon Virtual Private Cloud (VPC) architecture built from scratch. It establishes a secure network foundation following AWS best practices, featuring network segmentation using public and private subnets, internet connectivity via Internet Gateway, and secure outbound connectivity for private resources via a NAT Gateway.

---

## 🏗️ Architecture & Network Specifications

- **VPC CIDR Block:** `10.0.0.0/16`
- **Public Subnet (`public-vpc`):** `10.0.0.0/24` (Auto-assign public IP enabled)
- **Private Subnet (`private-vpc`):** `10.0.2.0/24`
- **Internet Gateway (IGW):** Attached to the VPC for direct internet access.
- **NAT Gateway:** Deployed in the Public Subnet with an Elastic IP (EIP) for secure outbound connectivity.
- **Route Tables:** 
  * `public-route-table`: Routes `0.0.0.0/0` traffic to Internet Gateway.
  * `private-route-table`: Routes `0.0.0.0/0` traffic to NAT Gateway.

---

## 📸 Implementation Screenshots

### 1. Subnets Configuration
<img width="1907" height="973" alt="vpc ss" src="https://github.com/user-attachments/assets/4fecc71a-6dd5-443f-a900-0845428c7811" />

### 2. Route Table Configuration
<img width="1902" height="917" alt="route table ss" src="https://github.com/user-attachments/assets/1ebca302-475f-4987-a096-5f789455ea28" />

### 3. NAT Gateway Setup
<img width="1918" height="923" alt="nat gateway" src="https://github.com/user-attachments/assets/d395441a-7e61-4ebe-9708-187475124c08" />

---

## 🎯 Key Takeaways
- Mastered hands-on configuration of core AWS Cloud Networking components.
- Implemented secure network isolation using public/private subnets and route table configurations.
- Configured one-way outbound internet access for private network resources using NAT Gateway.
