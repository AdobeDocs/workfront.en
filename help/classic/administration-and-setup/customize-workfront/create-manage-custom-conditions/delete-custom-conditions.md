---
filename: delete-custom-conditions
title: Delete a custom Condition
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
title: Delete a custom condition
description: You must have the following access to perform the steps in this article - EDIT ME.
---

# Delete a custom condition

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Access requirements

You must have the following access to perform the steps in this article: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Delete a custom condition

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. Click **Project Preferences** > **Conditions**. 

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Select the tab of the object type (**Project**, **Task**, or **Issue**) where the condition that you want to delete is located.

1. Hover over the condition you want to delete, then click the **Delete** icon ![](assets/delete.png) that appears on the far right.
1. In the confirmation message that appears, click **Delete Condition**.  

1. In the **Delete Condition** box that appears, select a new condition in the drop-down list for all projects that were using the condition that you are deleting.

   Custom conditions are available in the drop-down list only if they equate with the same built-in condition as the one you are deleting. For example, if you are deleting a condition that equates with At Risk, only custom conditions that also equate with At Risk are available to select.

1. Click **Delete Condition**.

>[!NOTE]
>
>You cannot delete&nbsp;the built-in conditions, which are On Target, At Risk, and In Trouble. However, you can change their names and colors.

For information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
