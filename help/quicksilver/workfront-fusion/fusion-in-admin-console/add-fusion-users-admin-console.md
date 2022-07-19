---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add users to Adobe Workfront Fusion through the Adobe Admin Console
description: You can add a user to the Adobe Admin Console and assign them to Adobe Workfront Fusion, or assign an existing user in the Adobe Admin Console to Workfront Fusion.
author: Becky
feature: Workfront Fusion
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
    
1.  In the list that displays, select the link at the top.
    
    This is your Production instance where your users work.
    
    ![Fusion instance in Admin Console](assets/fusion-instances-admin-console.png)
    
    >[!TIP]
    > 
    > Your Preview instance, the second link in the list, is a testing environment that replicates your live Production environment. For more information, see The Adobe Workfront Preview Sandbox Environment.
    >    
    > You might also see links to sandbox environments in the list. For more information, see The Adobe Workfront Preview Sandbox Environment.
    
1.  In the list that displays, with the Product Profiles tab selected, click the name of the Workfront Product Profile link.
    
    ![Workfront Fusion Product Profile](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)
    
    This list includes all users that are already assigned to your Production instance of Workfront.
    
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    
1.  Go to the user and admin area in the Admin Console, as described in [Add users to Adobe Workfront Fusion through the Adobe Admin Console](#Access) in this article.
1.  With the Users tab selected above the list, select **Add User**.
    
1.  In the **Add users to this product profile** box, enter the email address or name of a user you want to add, then select **Save**.
    
    The user is created in Workfront with the Requestor access level.
    
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    
1.  In Workfront, change the user's access level.
    
    For instructions on how a Workfront administrator can change the user's access level, see Edit a user's profile.
    
1.  Repeat steps 6 and 7 to add more users.
    

## Assign an existing user in the Adobe Admin Console to Workfront Fusion

1.  Begin editing the user as described in the "Edit user details" section of the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in the Adobe Admin Console documentation.
    
1.  Add **Adobe Workfront Fusion** to the products assigned to the user.