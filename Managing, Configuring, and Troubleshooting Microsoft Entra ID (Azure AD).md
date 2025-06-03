# Managing, Configuring, and Troubleshooting Microsoft Entra ID (Azure AD)

This project demonstrates how to manage, configure, and troubleshoot Microsoft Entra ID (formerly Azure Active Directory) using a Microsoft 365 tenant. It includes real-world scenarios, PowerShell scripts, and screenshots from a live environment

## Project Objectives

- Understand the core components of Entra ID
- Perform user and group management
- Configure security features like MFA and Conditional Access
- Troubleshoot common identity and access issues
- Document and automate tasks using PowerShell

## Step-by-Step Guide

### Step 1: **User and Group Management**

- Create users manually and via bulk import
  1.  Navigate to Identity
![image](https://github.com/user-attachments/assets/9ecbd725-1283-4aac-ab6b-2ca5bf98650b)


2.  Users

![image](https://github.com/user-attachments/assets/4c52d667-833d-4a3e-aaab-4a28e1dce8bc)

 
Bulk Operations > Bulk Create

![image](https://github.com/user-attachments/assets/d78813e8-84f7-4341-8115-7794b1c35633)

![image](https://github.com/user-attachments/assets/49db70cc-86d4-4a6a-b880-ca80a2a9e5d0)


- Create security and Microsoft 365 groups


![image](https://github.com/user-attachments/assets/73c02dc3-ac3c-4006-956b-0615427c4e6c)

- Security Group

![image](https://github.com/user-attachments/assets/c1d715b2-0144-4d59-8117-b341bbdd102b)

- Microsoft 365 Group

![image](https://github.com/user-attachments/assets/5e2686c6-6870-4dd4-bff1-f025a9900a71)

- M365 Group created successfully

![image](https://github.com/user-attachments/assets/b87dee88-cabd-467a-9234-4e42accb81ae)


- Assign group-based licensing

- Delegate admin roles


### Step 2. **Custom Domain Configuration**
- Add a custom domain to Entra ID
- Verify domain via DNS
- Set as a primary domain


### Step 3. **Multi-Factor Authentication (MFA)**
- Enable MFA per user
- Configure Conditional Access to enforce MFA
- Test login scenarios with and without MFA

### Step 4. **Conditional Access Policies**
- Create policies based on location, device, or risk
- Block legacy authentication
- Require compliant devices for access

### 5. **Enterprise App Integration**
- Add and configure an app (e.g., Salesforce, Dropbox)
- Enable Single Sign-On (SSO)
- Assign users/groups to the app

### 6. **Monitoring and Troubleshooting**
- Use Sign-in logs and Audit logs
- Troubleshoot login failures
- Resolve sync issues (if using Azure AD Connect)
- Use Entra ID recommendations and Identity Protection

### 7. **Automation with PowerShell**
- Install and connect to MS Graph
- Script user creation and license assignment
- Export user and group reports


## 🙌 Acknowledgments

- Microsoft Learn
- Microsoft 365 Developer Program
- Azure AD / Entra ID Documentation

