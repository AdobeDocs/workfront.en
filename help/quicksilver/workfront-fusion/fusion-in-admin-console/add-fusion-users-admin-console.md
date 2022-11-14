---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add users to Adobe Workfront Fusion through the Adobe Admin Console
description: You can add a user to the Adobe Admin Console and assign them to Adobe Workfront Fusion, or assign an existing user in the Adobe Admin Console to Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
hidefromtoc: true

---
# Add users to Adobe Workfront Fusion through the Adobe Admin Console

>[!IMPORTANT]
>
>The procedures described on this page apply only to organizations that have been onboarded to the Admin Console.
>
>If your organization has not yet been onboarded to the Adobe Admin Console, see [Add a user to an organization in Adobe Workfront Fusion](../organizations/add-user-to-an-organization.md).
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../fusion-in-admin-console/fusion-adobe-admin-console.md).

You can add a user to the Adobe Admin Console and assign them to Adobe Workfront Fusion, or assign an existing user in the Adobe Admin Console to Workfront Fusion.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> <p>Workfront Fusion for Work Automation </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr>
   <tr> 
   <td role="rowheader">Adobe administrator rights</td> 
   <td>You must be a Product Configuration Administrator of Adobe products for your organization.</td> 
  </tr>
  </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Prerequisites

Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console.

1.  If you are new to Adobe and you have received an email telling you that you now have administer rights to manage Adobe software and services for your organization, click the button in the email to create an Adobe account and open the Admin Console.
    
    Or
    
    If you already have an Adobe account, go to the [Adobe Admin Console page](https://adminconsole.adobe.com/).
    

## Add a new user to the Adobe Admin Console and Workfront Fusion

1.  From the [Adobe Admin Console page](https://adminconsole.adobe.com/), select the **Products** tab in the top navigation bar, and then select the **Workfront Fusion** product tile.
    
    ![Fusion in Admin Console](assets/fusion-product-admin-console.png)
    
1.  In the list that displays, select the organization where you want to add a user.
    
    ![Fusion instance in Admin Console](assets/fusion-instances-admin-console.png)
    
1.  In the list that displays, with the Product Profiles tab selected, click the name of the Workfront Fusion Product Profile link.
    
    ![Workfront Fusion Product Profile](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)
     
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    
1.  With the **Users** tab selected above the list, click **Add User**.
    
1.  In the **Add users to this product profile** box, enter the email address or name of a user you want to add, then select the user in the list that appears.

1. Click **Save**.
    
    The user is created in Workfront Fusion.
    
    <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Optional) Continue to [Change a user's access level in Workfront Fusion](#change-a-users-access-level-in-workfront-fusion)

## Change a user's access level in Workfront Fusion

### Change a user's role to Admin

Giving a user an Admin role must be done in the Adobe Admin Console. 

1. On the Workfront Fusion Product Profile page where you added the user, select the **Admins** tab.

1. Click Add Admin.

1.  In the **Add product profile administrators** box, enter the email address or name of a user you want to add, then select the user in the list that appears.

1. Click **Save**.

   This user is now an Administrator in Workfront Fusion.

### Change a user's role to Member, Accountant, or App Developer.
    
Member, Accountant, and App Developer roles are handled inside Workfront Fusion. 

For instructions, see [View or edit user roles](../organizations/manage-fusion-users.md#view-or-edit-user-roles) in the article [Manage Adobe Workfront Fusion users in your organization](../organizations/manage-fusion-users.md)
    
## Assign an existing user in the Adobe Admin Console to Workfront Fusion

1.  Begin editing the user as described in the "Edit user details" section of the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in the Adobe Admin Console documentation.
    
1.  Add **Adobe Workfront Fusion** to the products assigned to the user.
