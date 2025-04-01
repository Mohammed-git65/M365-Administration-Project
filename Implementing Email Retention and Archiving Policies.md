## **Introduction**

In the financial services industry, organizations must comply with strict regulatory requirements for data retention and security. One key requirement is the long-term retention of emails to ensure compliance with industry regulations.

This project focuses on configuring email retention and archiving policies in Microsoft 365 to help a financial services company meet its 7-year email retention requirement. The implementation will ensure that emails are securely retained, archived for long-term storage, and available for compliance investigations when necessary.

By leveraging Microsoft Purview Compliance Center, Exchange Online Archiving, and Litigation Hold, this solution will provide a structured approach to email governance, ensuring that the organization remains compliant while optimizing mailbox storage.


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

Finally, I reviewed the tag and submitted

<img width="807" alt="image" src="https://github.com/user-attachments/assets/7141d05a-6c39-422d-801b-cd2fa8ef57ce" />

<img width="953" alt="image" src="https://github.com/user-attachments/assets/c2c1527c-1980-4daa-955c-616c3355ea47" />

**Step 2: I Created a Retention Policy**

To do that:
- I signed in to my Microsoft 365 account with administrator credentials.
- Then, I navigated to the Microsoft Purview Compliance Portal or https://compliance.microsoft.com/
![image](https://github.com/user-attachments/assets/9b502a1a-4dd3-4cbb-8d31-f5a18babbbd2)
![image](https://github.com/user-attachments/assets/14ab7628-11e0-4398-9479-fe75dc6e854d)

- Expand the Data Lifecycle Management > MRM Retention Policies > I clicked on New Policy to start a new policy
![image](https://github.com/user-attachments/assets/5495ff06-1ad7-47f9-92d3-27330b560ff8)

- Here I provided a name for the policy and then added the tag as shown on the screenshot below:

<img width="808" alt="image" src="https://github.com/user-attachments/assets/c6a126c7-6c56-4561-a312-4206f2efc0c7" />



- Finally is to review and submit the policy
![image](https://github.com/user-attachments/assets/3527ef33-70b1-4553-a474-e01bbe6d9372)


![image](https://github.com/user-attachments/assets/a9540632-2ff7-4618-8c38-33e51306f9de)

**Create a Retention Tag**

![image](https://github.com/user-attachments/assets/7fb074b0-3aa0-46db-b912-fd19d3e76df3)

![image](https://github.com/user-attachments/assets/972cbf62-1d08-4933-9e55-9e32fa9a0da3)

![image](https://github.com/user-attachments/assets/b4dc0ddf-3a5c-4991-915f-65f101291112)

![image](https://github.com/user-attachments/assets/3a7ee9be-af7e-4896-aee3-c7b60888186b)





