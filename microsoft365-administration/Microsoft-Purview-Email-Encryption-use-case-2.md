## **Setting Up Email Encryption for Sensitive Communication**
A law firm needs to ensure that emails containing sensitive legal documents are encrypted when sent externally.

## **Step 1: Is Understanding Microsoft Purview Message Encryption**

Microsoft Purview Message Encryption is an online service that's built on Azure Rights Management (Azure RMS) which is part of Microsoft Purview Information Protection. This service includes encryption, identity, and authorization policies to help secure your email.

## **Here are the Key Features of Microsoft Purview Message Encryption**
- Enforces encryption based on predefined rules
- Works seamlessly with Microsoft Outlook and Outlook Web Access
- Protects sensitive information by encrypting email content
- Allows external recipients to securely read encrypted emails


## **Step 2: Is to Configure Mail Flow Rules to Automatically Encrypt Emails for the law firm**
To ensure emails containing sensitive legal documents are encrypted, the law firm will create mail flow rules in Exchange Online. These rules will detect specific keywords or attachments and apply encryption automatically

**To Configure Mail Flow Rules Here are the Steps to Take**

1. Access the Exchange Admin Center (EAC)

- Sign in to the Microsoft 365 Admin Center → Open the Exchange Admin Center.
  <img width="705" alt="img1" src="https://github.com/user-attachments/assets/3e19380b-ac16-4832-ad97-c535218c0891" />

2. Create a New Mail Flow Rule

- Navigate to Mail Flow → Rules → Click + Add a Rule → Select Create a New Rule.
![image](https://github.com/user-attachments/assets/b7436432-4fc2-4ae7-869d-14b9de9d3d4a)

![image](https://github.com/user-attachments/assets/25113b1e-4b6d-4116-82c6-10b5c454d359)

![image](https://github.com/user-attachments/assets/239b288f-b22e-44aa-81e6-ec4f461a33f9)

3. Define the Conditions for Encryption
- Name the rule: I named it Encrypt Emails with Sensitive Legal Documents
Then, I apply the rule if:

![image](https://github.com/user-attachments/assets/20064c99-5921-44de-be5e-45ba5884fd6d)

The subject or body contains specific words: I used the keywords like "Confidential"

![image](https://github.com/user-attachments/assets/d0e5263c-7fd1-4bb8-be57-01887c44b300)

To Apply the Encryption Action
Under Do the following, I choose:
- Modify the message security
- Apply Office 365 Message Encryption and Rights Protection
- And then select Encrypt.

![image](https://github.com/user-attachments/assets/485b1222-8cca-4fa7-8585-554b9c704535)

![image](https://github.com/user-attachments/assets/ec789fe1-a85b-4a11-89b8-c3f9d54f6f59)

- Set the rule settings
![image](https://github.com/user-attachments/assets/6ee8c7e1-311c-40bd-a7b3-fc2ae39289d3)

- Review and Finish

![image](https://github.com/user-attachments/assets/9d813714-2ab2-43b8-bb7f-a85770c159f0)

![image](https://github.com/user-attachments/assets/78a52461-f7ac-4fd1-bc60-b0485f794323)

After Reviewing, click on Done to effect the policy.

**Step 3: Is to send and verify an Encrypted Email**
- I send an Encrypted email from Outlook to Gmail to verify
![image](https://github.com/user-attachments/assets/25325e3d-24fd-4258-985e-a47ab876aa32)

Here's the Encrypted message in my Gmail
![image](https://github.com/user-attachments/assets/c415b2f4-c4a2-4177-a7fc-7e2edd479b7f)

Here you're requested to either sign in with your Gmail account or an OTP
![image](https://github.com/user-attachments/assets/6c66dcb8-9890-4f36-8d40-29a4454a0e21)

Here I opted for an OTP to open the email
![image](https://github.com/user-attachments/assets/7b6e084a-9090-41e6-a045-2abf7d59c82a)

Finally, I open the Encrypted message using the OPT

![image](https://github.com/user-attachments/assets/ca69bf80-b5bb-4c96-a42b-245a12579267)

## **Conclusion**

With this solution in place, the law firm can confidently send sensitive legal communications without worrying about security risks. By using Microsoft Purview Message Encryption and setting up Exchange Online Mail Flow rules, every external email is automatically protected. This not only ensures confidentiality but also helps the firm stay compliant with data protection regulations while keeping sensitive legal information safe from unauthorized access.
