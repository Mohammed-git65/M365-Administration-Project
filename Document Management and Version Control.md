**Introduction**


Managing and tracking contract changes efficiently is crucial for maintaining accuracy and compliance in today's fast-paced legal environment. A robust document management system with version control capabilities is essential for legal teams to ensure that all contract modifications are properly documented and approved. This project aims to implement a comprehensive document repository that facilitates version control, approval workflows, and collaborative editing.

**Statement Overview**

The legal team requires a document repository that stores contracts, tracks changes and maintains version history. This system will enable seamless collaboration among team members, ensuring that all edits and updates are accurately recorded. By implementing document libraries with metadata, co-authoring features, and file check-in/check-out functionalities, the team can enhance their document management processes and improve overall efficiency.

**Objectives**

Enable Document Versioning and Approval Workflows: Implement version control to track changes and maintain a history of contract modifications. Configure approval workflows to ensure that all changes are reviewed and authorized before finalizing.

Set Up Document Libraries with Metadata: Create document libraries that include metadata to categorize and organize contracts effectively. This will facilitate easy retrieval and management of documents.

Configure Co-Authoring and File Check-In/Check-Out: Enable co-authoring features to allow multiple team members to work on documents simultaneously. Implement file check-in/check-out functionalities to prevent conflicts and ensure that edits are properly managed.


**Step 1: Create a SharePoint for the Legal Team**

- Select Create to create a new site

<img width="957" alt="image" src="https://github.com/user-attachments/assets/1e1ae618-99e7-4ece-91d4-f4aaa05fcd39" />

- Select a site type

<img width="957" alt="image" src="https://github.com/user-attachments/assets/06fc1503-7228-42f2-b786-5995d8d38e8b" />

- Select a Template

<img width="957" alt="image" src="https://github.com/user-attachments/assets/808edab5-7752-49ef-897b-f8e44720cff1" />

- Select Use Template to use the Selected Template

<img width="957" alt="image" src="https://github.com/user-attachments/assets/8a68beb4-9830-42ae-834d-e458d3c542d9" />

- Give your site a name

<img width="957" alt="image" src="https://github.com/user-attachments/assets/99a03164-4a2f-47cd-8018-1e4cc261cf2c" />


- Set language and other options

<img width="957" alt="image" src="https://github.com/user-attachments/assets/5705528c-8d13-4046-b2f5-3ad647b0f0ab" />

- Add site owners and members

<img width="957" alt="image" src="https://github.com/user-attachments/assets/c1f13e3c-8967-4a7c-9fb5-1e5feaa48c2f" />

- Add news

<img width="957" alt="image" src="https://github.com/user-attachments/assets/8d09bb3d-bfc1-46d3-9488-d8f3b5805c3e" />

**Step 2: Set up document libraries with metadata**

- Click Settings 

<img width="957" alt="image" src="https://github.com/user-attachments/assets/0358e756-c6b6-49bc-80fb-ed9080c22e43" />


- Select site contents

<img width="957" alt="image" src="https://github.com/user-attachments/assets/3f274315-5c4b-4e97-bf5f-a55b5d4022f1" />

- Click + New 

<img width="957" alt="image" src="https://github.com/user-attachments/assets/529ac71a-e9fd-4f58-bb54-5c28d9462c92" />

- Select Document Library

<img width="957" alt="image" src="https://github.com/user-attachments/assets/f4e399ad-fa07-4e0b-901d-2e5a80dfbcf0" />


- Enter a name 

- Add a description (Optional)

- Click Create

<img width="957" alt="image" src="https://github.com/user-attachments/assets/802a8453-3091-454c-aef0-ff124dfb2e44" />

**Step 3: Add Metadata (Columns) to the Library**

- Go to the newly created library

<img width="957" alt="image" src="https://github.com/user-attachments/assets/4f148898-df50-42ef-9477-21dd08706b8c" />


- Click + Add column (from the header row)

<img width="957" alt="image" src="https://github.com/user-attachments/assets/56071eda-bc6c-455d-9e32-3823798de0a8" />

- Choose a column type

<img width="957" alt="image" src="https://github.com/user-attachments/assets/f1e69f3e-b0d7-4cba-9dcb-3ff0be90073f" />

- Set the name and options for each column, then click Save

<img width="957" alt="image" src="https://github.com/user-attachments/assets/5775019c-8337-411c-8f38-967b0044edbf" />

- Upload or Create Documents

- Click Upload

<img width="957" alt="image" src="https://github.com/user-attachments/assets/af992b1f-ddc9-4038-9d6f-c541bbcbeb93" />

 - Upload Files to bring in existing contracts

<img width="957" alt="image" src="https://github.com/user-attachments/assets/86bd1612-2969-42d2-ac2e-7305502ed9dc" />


**Step 4: Enable Document Versioning**

- Go to your SharePoint site and open the document library

<img width="957" alt="image" src="https://github.com/user-attachments/assets/da8642fa-a199-49c0-a67b-625f688a9a1b" />


- Click the Settings

<img width="957" alt="image" src="https://github.com/user-attachments/assets/d2430e17-910a-4469-a88d-6228f2454ee6" />


- Library Settings

<img width="957" alt="image" src="https://github.com/user-attachments/assets/69160ff1-58bb-42af-ba10-6241965fffa2" />

- Under General Settings, click Versioning Settings.

<img width="957" alt="image" src="https://github.com/user-attachments/assets/2f0bfb4d-3464-4c07-817f-fbf827b11672" />

**Set the following**:

Document Version History:

- Choose either:

- Create major versions only (recommended for formal documents like contracts).

- Require content approval for submitted items (optional if using workflows).

- Set how many versions to retain (default is 500; adjust based on retention policy).

- Click OK to save.

<img width="957" alt="image" src="https://github.com/user-attachments/assets/1a212c96-93ae-491d-87fa-73382f67200d" />

**Step 5: Enable File Check-In / Check-Out**

- Scroll to the Require Check Out section.

Set Require documents to be checked out before they can be edited. to Yes.

- Click OK.

<img width="957" alt="image" src="https://github.com/user-attachments/assets/31d24753-067d-47f0-be51-114884ba4abb" />

**Step 6: Configure and test document approval workflows**

- Go to your SharePoint document library

<img width="957" alt="image" src="https://github.com/user-attachments/assets/7bb535fb-4c57-4470-b058-85dcf2572431" />

- Click Automate

<img width="957" alt="image" src="https://github.com/user-attachments/assets/c7431808-685a-4890-8599-bad9ce5287a4" />

- Flows

<img width="957" alt="image" src="https://github.com/user-attachments/assets/d0fba96d-d2bd-4497-915e-8ff75ffcc699" />

- Approval Status is still showing pending


<img width="957" alt="image" src="https://github.com/user-attachments/assets/09aaa366-6355-4605-aa6b-5fa4669940b5" />


- Approval workflow

<img width="957" alt="image" src="https://github.com/user-attachments/assets/833712a1-81c3-4636-8a18-980192629c0d" />

<img width="957" alt="image" src="https://github.com/user-attachments/assets/919c625d-1a00-4185-9be2-b2760efbdc88" />


The Approval is still pending here

<img width="957" alt="image" src="https://github.com/user-attachments/assets/ab028796-9e2c-4a06-8713-cf872b540bda" />


- To approve the workflow go to Outlook on the web

<img width="957" alt="image" src="https://github.com/user-attachments/assets/38147fdf-fc11-4d1f-bc28-1086866a98b3" />


- Click on Approve and Comment, then click on Submit to approve the document

<img width="957" alt="image" src="https://github.com/user-attachments/assets/c4bc172c-2890-4260-9cc5-b8f2f9a8ea23" />

- Here's the approved message

<img width="957" alt="image" src="https://github.com/user-attachments/assets/339d7419-28b9-4a10-a6f5-5bed602e1e9d" />



