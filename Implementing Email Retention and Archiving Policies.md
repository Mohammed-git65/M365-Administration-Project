## **Introduction**

Organizations in the financial services industry must comply with strict regulatory requirements for data retention and security. One key requirement is the long-term retention of emails to ensure compliance with industry regulations.

This project focuses on configuring email retention and archiving policies in Microsoft 365 to help a financial services company meet its 7-year email retention requirement. The implementation will ensure that emails are securely retained, archived for long-term storage, and available for compliance investigations when necessary.

This solution will provide a structured approach to email governance by leveraging Microsoft Purview Compliance Center, Exchange Online Archiving, and Litigation Hold. It will ensure that the organization remains compliant while optimizing mailbox storage.


**Solution Overview**

1. Is to Configure Retention Policies and Labels in Microsoft Purview
2. Implement Mailbox Archiving for Long-Term Storage
3. Set up Litigation Hold for Compliance Investigations
## **Implementing Email Retention and Archiving Policies**

**Step 1: Access the Microsoft Purview Compliance Portal**
- I signed in to my Microsoft 365 account with administrator credentials.
- Then, I navigated to the Microsoft Purview Compliance Portal or https://compliance.microsoft.com/
![image](https://github.com/user-attachments/assets/9b502a1a-4dd3-4cbb-8d31-f5a18babbbd2)

- I clicked on **Solutions** > **Data Lifecycle Management** > **Exchange (Legacy)** > I clicked on the **Exchange (Legacy) drop-down and selected Retention tags** > Then, I clicked on the **+ sign to create a New Retention tag**
<img width="807" alt="image" src="https://github.com/user-attachments/assets/65ea404c-fbf9-4570-ac92-ac3100cd7cd5" />

In the screenshot below, I'm in the process of creating a retention tag

This means emails will be kept for seven years before any retention action (such as deletion or archiving) is applied.
<img width="807" alt="image" src="https://github.com/user-attachments/assets/b5e6cff3-3479-475f-949d-b0861bc84a6f" />

Here, I defined how the tag would be applied
<img width="807" alt="image" src="https://github.com/user-attachments/assets/9f0de53d-61c7-43bd-8d69-877f3fb116c5" />

Then, I defined the retention settings
<img width="807" alt="image" src="https://github.com/user-attachments/assets/d7b1acf3-5744-4ec9-b6ab-cb30a3d0d81a" />

- Finally, I reviewed the tag and submitted

<img width="807" alt="image" src="https://github.com/user-attachments/assets/7141d05a-6c39-422d-801b-cd2fa8ef57ce" />

- Here, the tag was successfully created
<img width="953" alt="image" src="https://github.com/user-attachments/assets/c2c1527c-1980-4daa-955c-616c3355ea47" />

**Step 2: I Created a Retention Policy**

To do that:
- I signed in to my Microsoft 365 account with administrator credentials.
- Then, I navigated to the Microsoft Purview Compliance Portal or https://compliance.microsoft.com/
![image](https://github.com/user-attachments/assets/9b502a1a-4dd3-4cbb-8d31-f5a18babbbd2)

- Then, I clicked on **Solution** > **Data LifeCycle Management
![image](https://github.com/user-attachments/assets/14ab7628-11e0-4398-9479-fe75dc6e854d)

- Expand the Data Lifecycle Management > MRM Retention Policies > I clicked on New Policy to start a new policy
![image](https://github.com/user-attachments/assets/5495ff06-1ad7-47f9-92d3-27330b560ff8)

- Here I provided a name for the policy and then added the tag as shown on the screenshot below:

<img width="960" alt="image" src="https://github.com/user-attachments/assets/c6a126c7-6c56-4561-a312-4206f2efc0c7" />

<img width="960" alt="image" src="https://github.com/user-attachments/assets/e196c6e3-1aba-4c4d-bb05-819afc42460f" />


- Finally, I reviewed and submitted the policy
<img width="960" alt="image" src="https://github.com/user-attachments/assets/80293564-f59d-4514-8472-65b8c3bef59a" />

<img width="960" alt="image" src="https://github.com/user-attachments/assets/d1344198-1990-4a36-a7d2-359e25558f14" />

**The next step is to go the Exchange Online and apply it to all mailboxes**

<img width="960" alt="image" src="https://github.com/user-attachments/assets/0455ebe8-2442-46a4-bf1e-fc44c716b4af" />

<img width="960" alt="image" src="https://github.com/user-attachments/assets/23c5e863-b111-483c-9bf7-c8b8f1f9c06a" />

**Step 3: I created a Retention Label**
To do that:
As shown in the screenshot below, I clicked on Solution > Data Lifecycle > Retention Label > I clicked on the + to create a new label
<img width="960" alt="image" src="https://github.com/user-attachments/assets/4fcca605-d351-4883-ab64-dfd9bee40fd2" />

<img width="960" alt="image" src="https://github.com/user-attachments/assets/2ed0354a-0960-414a-bb16-fc497b6823c6" />

Below, I defined the label settings
<img width="960" alt="image" src="https://github.com/user-attachments/assets/17b77950-13a0-4b64-bf7a-1baf4f21ab76" />

This is the definition of the period
<img width="960" alt="image" src="https://github.com/user-attachments/assets/c86381c9-976a-4df2-baed-6e8422fb5f26" />
Here, I choose what happens next to the label
<img width="960" alt="image" src="https://github.com/user-attachments/assets/3cd9ad6c-aea8-47a8-8dad-3f83930a96fd" />

Finally, I reviewed and created the label
<img width="960" alt="image" src="https://github.com/user-attachments/assets/f2059161-caf7-4e12-924f-1eeb8a9e7770" />

<img width="957" alt="image" src="https://github.com/user-attachments/assets/cead6e3c-31ca-422f-9afd-0716c1485dd4" />





