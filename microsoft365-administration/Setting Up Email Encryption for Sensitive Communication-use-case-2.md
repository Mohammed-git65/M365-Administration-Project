## **Setting Up Email Encryption for Sensitive Communication**
A law firm needs to ensure that emails containing sensitive legal documents are encrypted when sent externally.

**Introduction**

In the legal industry, safeguarding client confidentiality and maintaining the integrity of sensitive information is paramount. Law firms frequently exchange confidential legal documents with clients, external partners, and other stakeholders via email. With the growing risk of cyberattacks and data breaches, it is essential to implement secure methods for transmitting sensitive information to prevent unauthorized access and ensure compliance with regulatory requirements.

**Objective**

The objective of this project is to implement an email encryption solution that automatically detects and encrypts outbound emails containing sensitive legal documents. This solution should ensure that all external communications involving confidential information are securely transmitted, thereby protecting client data, maintaining compliance with legal and industry standards, and upholding the firm’s reputation for confidentiality and professionalism.


## **Here are the Key Features of Microsoft Purview Message Encryption**
- Enforces encryption based on predefined rules
- Works seamlessly with Microsoft Outlook and Outlook Web Access
- Protects sensitive information by encrypting email content
- Allows external recipients to read encrypted emails securely


## **Step 1: Is to Configure Mail Flow Rules to Automatically Encrypt Emails for the law firm**
The law firm will create mail flow rules in Exchange Online to ensure emails containing sensitive legal documents are encrypted. These rules will detect specific keywords or attachments and apply encryption automatically

**To Configure Mail Flow Rules, Here are the Steps to Take**

1. Access the Exchange Admin Center (EAC)

- Sign in to the Microsoft 365 Admin Center → Open the Exchange Admin Center.
  <img width="705" alt="img1" src="https://github.com/user-attachments/assets/3e19380b-ac16-4832-ad97-c535218c0891" />

2. Create a New Mail Flow Rule

- Navigate to Mail Flow → Rules → Click + Add a Rule → Select Create a New Rule to create a new rule
![image](https://github.com/user-attachments/assets/b7436432-4fc2-4ae7-869d-14b9de9d3d4a)

- Click the **+ Add a Rule to Add a new Rule**

![image](https://github.com/user-attachments/assets/239b288f-b22e-44aa-81e6-ec4f461a33f9)

3. Here, I defined the Conditions for Encryption to **set the rule Conditions**
- To name the rule: I named it Encrypt Emails with Sensitive Legal Documents.
Then, I apply the rule if the **Conditions** are met

![image](https://github.com/user-attachments/assets/20064c99-5921-44de-be5e-45ba5884fd6d)

Here, the subject or body contains specific word(s): So, I used the keyword **"Confidential"**

![image](https://github.com/user-attachments/assets/d0e5263c-7fd1-4bb8-be57-01887c44b300)

To Apply the Encryption Action
Under Do the following, I choose:
- Modify the message security
- Apply Office 365 Message Encryption and Rights Protection
- And then select Encrypt.

![image](https://github.com/user-attachments/assets/485b1222-8cca-4fa7-8585-554b9c704535)

- Here, is to **set the rule settings** and **clicked Next**
![image](https://github.com/user-attachments/assets/6ee8c7e1-311c-40bd-a7b3-fc2ae39289d3)

- Finally, it's to review the **rules**

![image](https://github.com/user-attachments/assets/9d813714-2ab2-43b8-bb7f-a85770c159f0)

- After reviewing, I clicked on Done to create the **Rule**, and it was successfully created
![image](https://github.com/user-attachments/assets/78a52461-f7ac-4fd1-bc60-b0485f794323)

**Step 3: Is to test and verify an Encrypted Email**
- So, I sent an Encrypted email from my Outlook to Gmail to verify the **rule**
<img width="960" alt="image" src="https://github.com/user-attachments/assets/18d5fd9c-a3c0-4e4c-ac04-7fcdc94f41fd" />


- Here's the Encrypted message delivered in my Gmail
<img width="960" alt="image" src="https://github.com/user-attachments/assets/fb6e2459-e770-4f87-8b4f-a7d36d900ad5" />


- Here you're requested to either sign in with your **Gmail account** or an **OTP**

<img width="960" alt="image" src="https://github.com/user-attachments/assets/390244c6-b72a-4646-b8c1-9f0750ee47a7" />


- So, I opted for an OTP to open the email
<img width="960" alt="image" src="https://github.com/user-attachments/assets/9f0cb503-21bd-4d8b-a608-3d8bebb6c5f7" />


Finally, I open the **Encrypted message using the OPT**

<img width="960" alt="image" src="https://github.com/user-attachments/assets/e497cc57-f1cb-4328-9b74-07c1933c9443" />


## **Conclusion**

With this solution in place, the law firm can confidently send sensitive legal communications without worrying about security risks. By using Microsoft Purview Message Encryption and setting up Exchange Online Mail Flow rules, every external email is automatically protected. This not only ensures confidentiality but also helps the firm stay compliant with data protection regulations while keeping sensitive legal information safe from unauthorized access.
