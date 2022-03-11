---
filename: set-custom-condition-default-tasks-issues
title: Set a custom Condition as the default for tasks and issues
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
title: Set a custom condition as the default for tasks and issues
description: When a user clicks Work on It or adds an update comment to a new task they have been assigned to (without manually setting a condition for the task), Adobe Workfront displays the default condition for tasks, which is configured in Setup. The same is true for issues.
---

# Set a custom condition as the default for tasks and issues

When a user clicks Work on It or adds an update comment to a new task they have been assigned to (without manually setting a condition for the task), Adobe Workfront displays the default condition for tasks, which is configured in Setup. The same is true for issues.

Workfront uses the built-in condition `Going Smoothly` as the default condition for tasks and, separately, for issues. As a Workfront administrator, you can change the default condition for both of these object types to a custom condition you have created.

## Access requirements

You must have the following to perform the steps in this article:

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

## Set a custom condition as a default condition for tasks or for issues:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Conditions</span>.</li> 
 <li value="3">Click the <span class="bold">Tasks</span> or <span class="bold">Issues</span> tab. </li> 
 <li value="4">Click <span class="bold">Set Default Conditions</span>. </li> 
 <li value="5">In the drop-down menu, click the custom condition you want as the default condition for tasks (or issues). </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

>[!NOTE]
>
>* A user who is assigned to a task or issue, or who has Manage permissions on it, can change its condition manually. For more information, see [Update Condition for tasks and issues](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* The three default conditions for tasks and issues that come with Workfront are Going Smoothly, Some Concerns, and Major Roadblocks. You cannot hide or delete these conditions, but you can change their names and colors. Or you can create new ones to use instead, as described in [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>

For information about configuring a custom condition as a default condition for projects, see [Set a custom condition as the default for projects](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

For information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
