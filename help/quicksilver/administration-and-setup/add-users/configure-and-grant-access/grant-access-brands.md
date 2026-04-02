---
title: Grant Access to Brand Permissions
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: As an Adobe Workfront administrator, you can configure brand permissions by creating a user group in the Admin Console and assigning the GenStudio system manager product profile.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
---
# Grant access to brand permissions

{{highlighted-preview-article-level}}

Users are granted the brand create, edit, and publish permissions of Adobe GenStudio system managers when added to a user group. 

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

## Requirements

* Your Workfront instance must have Unified Approvals enabled. 

* Your organization must have GenStudio Foundation. 
    * Content Reviewer in Workfront provides the functionality available in GenStudio Foundation for asset review and approval workflows. You do not need to access GenStudio Foundation directly to complete your work. Your access to GenStudio Foundation functionality through Content Reviewer falls under the terms of your Workfront contract.
* Adobe must have a signed Adobe Gen AI agreement on file.
    For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

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

You must complete all steps in the previous section before granting access to individual users to Brands in Workfront access levels.

>[!IMPORTANT]
>
>* Only users assigned to the user group with the GenStudio system manager product profile in the Admin Console can create, edit, and publish brands in Workfront, even if other users have access to Brands enabled in their access level settings.
>* Users added to the access level with Brands access enabled but not added to the user group in the Admin Console can only view brands. 


To grant access to Brands in Workfront access levels:

{{step-1-to-setup}}

1. Click **Access Levels** in the left panel.
1. Find the access level you want to edit, then click the edit icon ![edit icon](assets/edit-icon.png) to edit it.

   Or

   Click **New Access Level** to create a new access level. For more information about creating access levels, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Scroll down to **Set additional restrictions**, then select **Allow users to access Brands**.
    ![allow access to brands setting](assets/access-for-brands.png)
1. Click **Save**.

Once you have configured Brands, you can create a Content Reviewer to review assets against brand guidelines in the review and approval workflow. For more information, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).
