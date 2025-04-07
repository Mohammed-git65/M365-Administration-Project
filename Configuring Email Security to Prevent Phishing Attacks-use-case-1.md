# Configuring Email Security to Prevent Phishing Attacks

## Introduction
Phishing attacks significantly threaten organizations, leading to data breaches, credential theft, and financial losses. **Fabrikam Inc.** has experienced an increase in phishing emails. Robust security solutions are essential to safeguard sensitive information and maintain organizational integrity. Microsoft Defender for Office 365 is a cloud-based security platform designed to mitigate risks by offering advanced protection for emails and collaboration tools.

In this project, I outlined the steps I took to configure Microsoft Defender for Office 365 to enhance an organization's security posture, protecting against email-based threats, phishing attempts, and other malicious attacks.

## Solution Overview
To mitigate phishing risks,  I implemented the following security measures:

**Anti-Phishing & Anti-Spam Policies** – Configured policies in **Microsoft Defender for Office 365** to detect and block phishing attempts.

**Safe Links & Attachments** – Enabled real-time protection against malicious links and attachments.

**SPF, DKIM, and DMARC** – Implemented email authentication protocols to prevent domain spoofing.

**Zero-Hour Auto Purge (ZAP)** – Automatically removed phishing emails post-delivery.

**Threat Explorer** analyzes phishing attempts and improves detection mechanisms.

### Step 1: Configure Anti-Phishing Policies in Defender for Office 365
To do that:
- I went to Microsoft Defender Portal: https://security.microsoft.com
- Sign in as a security administrator or a Global administrator
- I Navigated to **Email & Collaboration** > **Policies & Rules** > **Threat Policies** > **Anti-Phishing**.
- Then, I set up a policy for high-level employees and defined the policy name. In this case, I used **Fabrikam Anti-Phishing Policy**
- I added **protected users, domains, and mailbox intelligence**.
- Then, I enabled **impersonation protection**.
- I finally reviewed the policy and then clicked on Done to apply the policy

![image](https://github.com/user-attachments/assets/cc149fce-f485-4ddb-9451-c5057d0c6d05)

![image](https://github.com/user-attachments/assets/918bc062-6e62-415f-bb51-6841199d2f16)

![image](https://github.com/user-attachments/assets/f94f647f-be2f-4506-96b0-8031b5a4a6c8)

![image](https://github.com/user-attachments/assets/7c24988a-3bd8-4ccb-b018-9ffe160ba747)

![image](https://github.com/user-attachments/assets/58f95173-ed7d-4d24-b955-e4b72685d003)


- Here I added the domain
<img width="805" alt="image" src="https://github.com/user-attachments/assets/94b2c4d8-f0af-4297-bf8d-53803fc1ff38" />

![image](https://github.com/user-attachments/assets/c501a290-1a4a-4fe3-a298-182a3cc64da7)

![image](https://github.com/user-attachments/assets/5ee96b79-3a9e-4643-8dad-322c7ee10d7d)

- Here I review the Anti-Phishing policy before submitting
![image](https://github.com/user-attachments/assets/7c9f36af-7901-4012-83d8-7fbd6a0f03c7)


### Step 2: I created an Anti-Spam policy

- I went to Microsoft Defender Portal: https://security.microsoft.com
- Sign in as a security administrator or a Global administrator
- I navigate to **Email & Collaboration** > **Policies & Rules** > **Threat Policies** > **Anti-Spam**.
- Then click on **+ Create** to create new policies

![image](https://github.com/user-attachments/assets/5a7f06bc-04d6-4263-93d3-2bc91cbb0015)

<img width="805" alt="image" src="https://github.com/user-attachments/assets/e1d71fd4-f34b-4c38-aeba-55b5a9f384a2" />


- Here are the Actions to be taken
![image](https://github.com/user-attachments/assets/39276b9c-ccd4-4331-8a3e-3c3c6e7015b2)

- After reviewing the Anti-Spam Policy, I click on Create to create the policy
![image](https://github.com/user-attachments/assets/cc9325fa-8c86-4d36-bd97-1784f71a53ac)


## **Step 3: Implementing Safe Links and Safe Attachments**  
1. **To enable Safe Attachments**:
- I navigated to **Threat Policies** > **Safe Attachments**.
- Created a new policy to **scan attachments for malware** and define the policy
- I configured options to **block or quarantine** suspicious files.
- Then I reviewed and applied the policy.

![image](https://github.com/user-attachments/assets/ad1133b5-fbed-42d3-bf0c-677c24d54dfe)

<img width="806" alt="image" src="https://github.com/user-attachments/assets/22d29c10-e9e9-4f69-aeac-c98c40ea0fa9" />

- As shown above, I selected the domain name for the Safe Attachments policy in Microsoft 365 Defender, and the protection was automatically applied to all email addresses within that domain.

This ensures that any email address using the domain benefits from the Safe Attachments policy, which enhances security by scanning email attachments in real-time to detect and block malicious content
![image](https://github.com/user-attachments/assets/d0a58b73-47ec-4c57-91dd-557266bb422c)

![image](https://github.com/user-attachments/assets/01081a2e-e027-47d0-a975-49581ca5ef29)

2. **Enable Safe Links**:
To do that:
- I navigated to **Threat Policies** > **Safe Links**.
- I click **Create policy** and define the policy.
- I Enabled real-time scanning of **URL links in emails**.
- Then I reviewed and applied the policy.

![image](https://github.com/user-attachments/assets/0d5eae24-54bb-4903-88f6-df2b2590e686)

![image](https://github.com/user-attachments/assets/b76f7d48-9492-444f-95e8-6533c2d7e1bb)

![image](https://github.com/user-attachments/assets/a9a52ebd-6339-4a0a-ba78-673a806791ff)

![image](https://github.com/user-attachments/assets/3d183124-696f-49b4-bb25-df4e8f6fce7f)

## **Setting up SPF, DKIM, and DMARC for Email Authentication**  
1. **SPF**: The SPF record has already been done
2. Before I enabled the **DKIM**, I sent an email from my domain to Gmail to see if it would pass **SPF** and **DKIM** using Mxtoolbox to verify and see if it passes **SPF** and **DKIM**.

**The Screenshots below only show that it passes only SPF**
<img width="939" alt="img11" src="https://github.com/user-attachments/assets/fd34363e-6587-4f36-ab90-5f5531c37a69" />
![image](https://github.com/user-attachments/assets/09556709-d7b5-4ba7-8123-208c3553ccf6)
<img width="960" alt="image" src="https://github.com/user-attachments/assets/e10086d8-dce1-4e6f-81d6-6f95694ea06e" />


So after I published the **Cname** in my domain provider and then enabled **DKIM**, it passed both **SPF** and **DKIM**

<img width="960" alt="image" src="https://github.com/user-attachments/assets/5fbdea7e-669c-4e35-9ae2-50d1649b8e56" />

![image](https://github.com/user-attachments/assets/7e8c1b11-f7ce-4bdc-89ab-9a4c31d91356)


## **DMARC**

![image](https://github.com/user-attachments/assets/4dd0460d-f48d-4820-b6d5-ef6a429f4d76)

## **Step 3: To Enable Zero-Hour Auto Purge (ZAP) in Microsoft 365 Defender**
- Sign in to the **Microsoft 365 Defender portal**. 
- Navigate to **Threat Policies**:
- Under **Email & collaboration,** I select **Policies & rules**.
- Then, I selected **Threat policies**. 
- Then to configure the Anti-malware Policies:
- Under **Policies**, I selected **Anti-malware**, Selected the **Default (Default)** policy, and Clicked **Edit protection settings**. 
- Then, I checked the box labeled **Enable zero-hour auto purge for malware (Recommended)**.
- And Click **Save**. 
![image](https://github.com/user-attachments/assets/5f375ed0-459a-49ad-a8b4-a2b8e3e0026d)


## **After all the configurations, I test for Phishing emails using Threat Explorer**

To do that:
- I Access **Threat Explorer**
- I went to the Microsoft Defender portal: https://security.microsoft.com
- Navigate to **Email & collaboration** > **Explorer**
- I selected the **Phish View** in **Threat Explorer** to filter the email 
![image](https://github.com/user-attachments/assets/c779315e-460d-43e4-86f8-053ef7e12b09)

![image](https://github.com/user-attachments/assets/99eabef8-7581-4ee5-8d05-84facf8bfb72)

**Conclusion**
Implementing these security measures significantly strengthened Fabrikam Inc.'s defenses against phishing attacks. By configuring Anti-Phishing and Anti-Spam policies, enabling Safe Links and Safe Attachments, and setting up SPF, DKIM, and DMARC, I created multiple layers of protection to prevent domain spoofing and malicious email threats. Additionally, activating Zero-Hour Auto Purge (ZAP) ensured that phishing emails were swiftly removed, even after delivery, reducing potential risks.
To validate these implementations, I used Threat Explorer to analyze phishing attempts.
