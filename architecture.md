# 🏗️ Architecture Explanation

## 🔐 Flow Overview

1. Admin user manages AWS resources
2. Developer user (anas-dev) has restricted access
3. EC2 instance assumes IAM Role
4. EC2 accesses S3 securely via role

---

## 🔁 Access Flow

* anas-dev → S3 (limited access, no delete)
* EC2 Role → S3 (read access only)
* Admin → Full access

---

## 🧠 Security Layers

* IAM Policies (Allow/Deny)
* Permissions Boundary
* Role-based access
* No direct credential exposure

---

## 📊 Diagram 



<img width="1746" height="1236" alt="image" src="https://github.com/user-attachments/assets/f836d15e-4f28-4bba-818c-ca0338d5acf2" />


## 🎯 Key Design Principles

* Least privilege
* Separation of roles
* Secure service-to-service communication
* Defense in depth
