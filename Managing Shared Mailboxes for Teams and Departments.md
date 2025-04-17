**Introduction**

Managing Shared Mailboxes for Teams and Departments

**To Create and Configure Shared Mailboxes**

**Step 1: Access The Microsoft 365 Admin Center**

- Log in to the Microsoft 365 Admin Center using your admin credentials.
<img width="949" alt="image" src="https://github.com/user-attachments/assets/ac725ea9-41aa-4273-bef9-f940afa3cd5b" />

**Step 2: Create a Shared Mailbox**
- Go to your Exchange Admin Center
- Click on **Mailboxes** and then, click on **Add a shared mailbox** to create a new Mailbox
<img width="949" alt="image" src="https://github.com/user-attachments/assets/86f76858-dc68-45df-abad-d8b55ebbadce" />

- Here, fill in the **name and email address** of the shared mailbox.

<img width="949" alt="image" src="https://github.com/user-attachments/assets/ecda5d85-d13d-47b6-961e-c88631128ea3" />

- Here, the shared mailbox is created successfully

<img width="949" alt="image" src="https://github.com/user-attachments/assets/f69bfcc9-838a-48f2-a018-b350014a8d7a" />

**Using Windows PowerShell to Create the Shared Mailbox**

<img width="967" alt="image" src="https://github.com/user-attachments/assets/6f5366aa-2f99-45e9-9f56-cd13e3a64b90" />

- Now, add delegation permission

<img width="959" alt="image" src="https://github.com/user-attachments/assets/be086857-f299-4e43-85cd-28d8d55bd49c" />

- Assign members and delegate them to **Send As**
<img width="949" alt="image" src="https://github.com/user-attachments/assets/01bb33a4-a026-408f-9209-894e00fab234" />

- Here, the two added members are confirmed to have **full access** to the **Mailbox**
<img width="949" alt="image" src="https://github.com/user-attachments/assets/0c5ad1ac-4dba-4bf3-99f3-bcded72a430f" />



**Step 3: Test Sending and Receiving Emails from the Shared Mailbox**

1. To test for **Send As**

- Log in to Outlook OWA and click on Options, and tick the Show From to enable the Send As

- Click “New Email”

- Select **Options** and then, select **Show From**

- Click From > Click “Other email address”

- Choose the shared mailbox email or type it in manually

- Compose and send an email
  
<img width="964" alt="image" src="https://github.com/user-attachments/assets/69c41b4a-4df8-4793-bbe8-97ea0e5cdea4" />

- This is the delivered email

<img width="942" alt="image" src="https://github.com/user-attachments/assets/197780ef-5446-46b5-a1c1-f5650fbabdde" />


2. To test for **Send on behalf**

- Go to the **Shared Mailbox**, click on it to open it up, and then select **Send on behalf** to delegate members that would **Send on behalf** of the **Mailbox** 

<img width="967" alt="image" src="https://github.com/user-attachments/assets/2915ecde-9aef-4c64-89f5-12946ed2ac42" />

- Here are the selected members who have the permissions to **Send on behalf**

<img width="441" alt="image" src="https://github.com/user-attachments/assets/56650980-6561-42a6-8ea1-0c4822e7d3de" />

- Mailbox permissions added to the Mailboxes

<img width="939" alt="image" src="https://github.com/user-attachments/assets/b4dba7b4-3ef8-44dc-b83c-88f340e07120" />

- To send an email on behalf of

- Click “New message”

- Select **Options** and select **Show From**
  
- Click From > Click “Other email address…”

- Choose customerservice@yourdomain.com or type it in manually 

- Compose and send an email

3. Receive Email:

- Here's the test email sent to the shared mailbox

<img width="969" alt="image" src="https://github.com/user-attachments/assets/301ecce2-1378-4250-a973-63b0d1b35c3b" />

