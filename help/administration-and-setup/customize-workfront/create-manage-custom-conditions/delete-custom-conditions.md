---
filename: delete-custom-conditions
title: Delete a custom Condition
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
title: Delete a custom condition
description: You must have the following to perform the steps in this article:
---

# Delete a custom condition

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

## Delete a custom condition

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Conditions</span>.<br></li> 
 <li value="3">Select the tab of the object type (<span class="bold">Project</span>, <span class="bold">Task</span>, or <span class="bold">Issue</span>) where the condition that you want to delete is located.</li> 
 <li value="4"> <p>Hover over the condition you want to delete, then click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> that appears on the far right.</p> </li> 
 <li value="5">In the confirmation message that appears, click <span class="bold">Delete Condition</span>.<br></li> 
 <li value="6"> <p>In the <span class="bold">Delete Condition</span> box that appears, select a new condition in the drop-down list for all projects that were using the condition that you are deleting.</p> <p>Custom conditions are available in the drop-down list only if they equate with the same built-in condition as the one you are deleting. For example, if you are deleting a condition that equates with At Risk, only custom conditions that also equate with At Risk are available to select.</p> </li> 
 <li value="7">Click <span class="bold">Delete Condition</span>.</li> 
</ol>

>[!NOTE]
>
>You cannot delete&nbsp;the built-in conditions, which are On Target, At Risk, and In Trouble. However, you can change their names and colors.

For information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
