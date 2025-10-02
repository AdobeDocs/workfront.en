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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Delete a custom condition

{{step-1-to-setup}}

1. Click **Project Preferences** > **Conditions**.

1. Select the tab of the object type (**Project**, **Task**, or **Issue**) where the condition that you want to delete is located.

1. Click **Delete** next to the condition name you want to delete.
1. In the **Delete condition** box that appears, select a new condition in the drop-down list for all projects, tasks, or issues that were using the condition you are deleting.

   Custom conditions are available in the drop-down list only if they equate with the same built-in condition as the one you are deleting. For example, if you are deleting a condition that equates with At Risk, only custom conditions that also equate with At Risk are available to select.

1. Click **Delete condition**.

>[!NOTE]
>
>You cannot delete the built-in conditions, which are On Target, At Risk, and In Trouble. However, you can change their names and colors.
>
>For information about editing custom conditions, see [Create or edit a custom condition](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
