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
- Then, I navigated to the Microsoft Purview Compliance Portal or click on the link directly https://compliance.microsoft.com/
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
- Then, I navigated to the Microsoft Purview Compliance Portal or click on the link directly https://compliance.microsoft.com/
![image](https://github.com/user-attachments/assets/9b502a1a-4dd3-4cbb-8d31-f5a18babbbd2)

- Then, I clicked on **Solution** > **Data LifeCycle Management**
![image](https://github.com/user-attachments/assets/14ab7628-11e0-4398-9479-fe75dc6e854d)

- Expand the Data Lifecycle Management > MRM Retention Policies > I clicked on New Policy to start a new policy
![image](https://github.com/user-attachments/assets/5495ff06-1ad7-47f9-92d3-27330b560ff8)

- Here I provided a name for the policy and then added the tag as shown on the screenshot below:

<img width="960" alt="image" src="https://github.com/user-attachments/assets/c6a126c7-6c56-4561-a312-4206f2efc0c7" />

<img width="960" alt="image" src="https://github.com/user-attachments/assets/e196c6e3-1aba-4c4d-bb05-819afc42460f" />


- Finally, I reviewed and submitted the policy
<img width="960" alt="image" src="https://github.com/user-attachments/assets/80293564-f59d-4514-8472-65b8c3bef59a" />

- And the policy is successfully created
<img width="960" alt="image" src="https://github.com/user-attachments/assets/d1344198-1990-4a36-a7d2-359e25558f14" />

**The next step is to go the Exchange Online and apply it to all mailboxes**

<img width="960" alt="image" src="https://github.com/user-attachments/assets/0455ebe8-2442-46a4-bf1e-fc44c716b4af" />

<img width="960" alt="image" src="https://github.com/user-attachments/assets/23c5e863-b111-483c-9bf7-c8b8f1f9c06a" />


**Conclusion**

In conclusion, the implementation of email retention and archiving policies in Microsoft 365 for the financial services company has been successfully completed. By configuring retention policies and labels in Microsoft Purview, implementing mailbox archiving for long-term storage, and setting up litigation hold for compliance investigations, the organization is now well-equipped to meet its 7-year email retention requirement.

This structured approach to email governance ensures that emails are securely retained and archived, optimizing mailbox storage while maintaining compliance with industry regulations. The use of Microsoft Purview Compliance Center, Exchange Online Archiving, and Litigation Hold provides a robust solution that supports the organization's commitment to data security and regulatory compliance.

With these measures in place, the company can confidently manage its email data, ensuring that it is available for compliance investigations when necessary, thereby upholding the highest standards of data retention and security.
