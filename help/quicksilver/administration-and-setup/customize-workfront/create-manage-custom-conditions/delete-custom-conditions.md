---
title: Delete a Custom Condition
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: You can delete a custom condition.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
---
# Delete a custom condition

You can delete a custom condition if it is no longer needed.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Delete a custom condition

{{step-1-to-setup}}

1. Click **Project Preferences** > **Conditions**. 

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Select the tab of the object type (**Project**, **Task**, or **Issue**) where the condition that you want to delete is located.

1. Hover over the condition you want to delete, then click the **Delete** icon ![](assets/delete.png) that appears on the far right.
1. In the confirmation message that appears, click **Delete Condition**.  

1. In the **Delete Condition** box that appears, select a new condition in the drop-down list for all projects that were using the condition that you are deleting.

   Custom conditions are available in the drop-down list only if they equate with the same built-in condition as the one you are deleting. For example, if you are deleting a condition that equates with At Risk, only custom conditions that also equate with At Risk are available to select.

1. Click **Delete Condition**.

>[!NOTE]
>
>You cannot delete the built-in conditions, which are On Target, At Risk, and In Trouble. However, you can change their names and colors.

For information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
