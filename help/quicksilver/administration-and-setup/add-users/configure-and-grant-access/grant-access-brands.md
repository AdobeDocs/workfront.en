---
title: Grant Access to Brand Permissions
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: As an Adobe Workfront administrator, you can configure brand permissions by creating a user group in the Admin Console and assigning the GenStudio system manager product profile.
author: Courtney
feature: System Setup and Administration
role: Admin
---
# Grant access to brand permissions

Users are granted the brand create, edit, and publish permissions of Adobe GenStudio system managers when added to a user group. Users also receive an automated email invitation to edit the Adobe GenStudio for Performance Marketing Brands project.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console permissions</td> 
   <td> <p>You must be a system administrator in the Adobe Admin Console.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 1. Configure brand permissions in the Admin Console

### Step 1: Create a user group

Create a new user group in the Admin Console to manage permissions for brand creation and editing.

### Step 2: Assign a product profile to the user group

The entitlement associated with the assigned profile gives all users in this group GenStudio Brands permissions (create, update, and delete brands).

To assign a profile:

1. Navigate to the newly created user group.
1. Click the **Assigned product profiles** tab.
1. Click **Assign profile**.
1. In the popup, select **Adobe GenStudio** from the products list, then click **Apply**.
1. Select the **Adobe GenStudio system manager** profile.
1. Click **Apply**.
1. Click **Save**.

### Step 3: Add users to the user group

To assign users permissions to create, edit, and publish brands, add them to the user group.

>[!NOTE]
>
>You must add at least one user before adding the group to a project as described in step 4.

To add users:

1. Go to **Admin Console** > **Users** > **User Groups**.
1. Select your user group.
1. Add users by username or email address.
1. Select from suggested matches for existing users.

### Step 4: Create a Brands project

A project provides a storage location where users can save brand assets.

To create a project:

1. Navigate to the **Storage** tab in Admin Console.
1. Click **Projects**.
1. Click **Create Project**.
1. In the popup, enter the project name: **Adobe GenStudio Brands**.

   >[!IMPORTANT]
   >
   >Enter the project name exactly as shown. Do not add extra spaces or change the case.

1. Click **Create**.

### Step 5: Invite the user group to the project

Add the user group to the Brands project so they can access and manage assets.

1. In the **Invite to project** popup, add the user group you created.
1. Select **Can edit** permissions.
1. Click **Invite**.

### Result

Users in the group now have permissions to create, edit, and publish brand assets within Workfront.
## 2. Grant access to Brands in Workfront access levels