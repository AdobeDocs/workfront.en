---
title: Set a Custom Condition as the Default for Tasks and Issues
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: When a user clicks Work on It or adds an update comment to a new task they have been assigned to (without manually setting a condition for the task), Adobe Workfront displays the default condition for tasks, which is configured in Setup. The same is true for issues.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
---
# Set a custom condition as the default for tasks and issues

When a user clicks Work on It or adds an update comment to a new task they have been assigned to (without manually setting a condition for the task), Adobe Workfront displays the default condition for tasks, which is configured in Setup. The same is true for issues.

Workfront uses the built-in condition Going Smoothly as the default condition for tasks and, separately, for issues. As a Workfront administrator, you can change the default condition for both of these object types to a custom condition you have created.

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

## Set a custom condition as a default condition for tasks or for issues:

{{step-1-to-setup}}

1. Click **Project Preferences** > **Conditions**.

1. Click the **Tasks** or **Issues** tab. 

1. Click **Set Default Conditions**. 
1. In the drop-down menu, click the custom condition you want as the default condition for tasks (or issues). 
1. Click **Save**.

>[!NOTE]
>
>* A user who is assigned to a task or issue, or who has Manage permissions on it, can change its condition manually. For more information, see [Update Condition for tasks and issues](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* The three default conditions for tasks and issues that come with Workfront are Going Smoothly, Some Concerns, and Major Roadblocks. You cannot hide or delete these conditions, but you can change their names and colors. Or you can create new ones to use instead, as described in [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>

For information about configuring a custom condition as a default condition for projects, see [Set a custom condition as the default for projects](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

For information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
