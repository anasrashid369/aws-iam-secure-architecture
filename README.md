# 🔐 AWS IAM Secure Architecture Project

## 📌 Overview

This project demonstrates a secure IAM (Identity and Access Management) setup for a startup-like environment using AWS best practices.

The goal was to implement **least privilege access**, secure authentication, and proper role-based access control.

---

## 🏗️ Architecture Components

* IAM Users (Admin & Developer)
* IAM Groups (Admin-Team, Backend-Team)
* IAM Role (EC2 Role for S3 access)
* S3 Bucket (Secure storage)
* Custom IAM Policies
* Permissions Boundary
* IAM Policy Simulator & Access Analyzer

---

## 👥 IAM Setup

### 🔹 Admin User

* Full access using AWS managed policy

### 🔹 Developer User (anas-dev)

* Restricted access using custom policy
* Cannot delete S3 objects (explicit deny)
* Limited via permissions boundary

---

## 🎭 IAM Role (EC2)

* Role attached to EC2
* Allows secure access to S3 without hardcoded credentials

---

## 🔐 Security Features Implemented

* Least Privilege Principle
* Explicit Deny for critical actions
* Permissions Boundary for additional restriction
* MFA enabled for users
* No hardcoded credentials

---

## 🧪 Testing & Validation

* IAM Policy Simulator used to verify permissions
* Access Analyzer used to detect security risks

---

## 💡 Key Learnings

* Explicit Deny overrides Allow
* Roles are essential for secure AWS service access
* Managed policies are broad; custom policies are precise
* Permissions boundaries add an extra layer of control

---

## 🚀 Future Improvements

* Add CloudTrail-based policy generation
* Integrate with CI/CD pipelines
* Expand to EC2 + S3 full architecture

---

## 📸 Screenshots

<img width="1683" height="796" alt="image" src="https://github.com/user-attachments/assets/5c9368bd-781a-43a6-8fe1-afaff4293ee5" />
<img width="1133" height="691" alt="image" src="https://github.com/user-attachments/assets/c1d59536-614b-44e9-922e-5b34092d2468" />

<img width="1504" height="697" alt="image" src="https://github.com/user-attachments/assets/e1b53c6a-ffe8-4a7d-a221-36d53e86823c" />


---

## 🏷️ Tags

#AWS #IAM #CloudSecurity #DevOps #LearningInPublic
