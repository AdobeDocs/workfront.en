---
filename: create-edit-custom-conditions
title: Create or edit a custom Condition
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
title: Create or edit a custom condition
description: As an Adobe Workfront administrator, you can create or edit a custom condition for projects, tasks, and issues to match the needs of your organization.
---

# Create or edit a custom condition

As an *Adobe Workfront administrator*, you can create or edit a custom condition for projects, tasks, and issues to match the needs of your organization.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create or edit a custom condition

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Conditions</span>.<br></li> 
 <li value="3">Click the tab of the object type (<span class="bold">Project</span>, <span class="bold">Task</span>, or <span class="bold">Issue</span>) that you want to associate with the condition.</li> 
 <li value="4"> <p>To create a new condition, click <span class="bold">Add a New Condition</span>.</p> <p>Or</p> <p>To edit an existing condition, hover over the condition you want to edit, then click the <span class="bold">Edit</span> icon that appears to the far right.<br></p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/custom-condition-edit-nwe-350x137.jpg" style="width: 350;height: 137;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/custom-condition-edit-nwe-350x137.jpg" style="width: 350;height: 137;"> </p> </li> 
 <li value="5"> <p>Configure your custom condition using the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Condition Name</td> 
     <td>(Required) Type a descriptive name for the condition.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>(Optional) Type a description of the condition's purpose for those who will use it.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Color</td> 
     <td>(Optional) Click the color icon, then choose the color you want for the condition when it displays in projects, task, or issues. You can also type a hex number.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Equates With </td> 
     <td>(Required, for projects only) Click the option in the drop-down list that best describes the function of your new condition. For example, for a condition named Tracking Well, you would click On Target. This determines how your default conditions work. Every condition you create must equate with one of the options in the drop-down menu.<p> For information about default conditions, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Set a custom condition as the default for projects</a> and <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Set a custom condition as the default for tasks and issues</a>.</p><p>This option cannot be modified after you finish creating the condition.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Key</td> 
     <td>(Required) For a project condition, type an alphanumeric abbreviation that users will be able to recognize. For a task or issue condition, type a two-digit numeric code from 01 to 99. <p>This key, which is used in the API and can be used for reporting purposes, must&nbsp;be unique for each object.</p><p>You cannot change the key for a condition after you save the condition. </p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hide Condition</td> 
     <td>(Optional) This option is available for custom conditions that you no longer want people to use, but want to keep for historical reasons. <p>If you hide a custom condition that has been used on work items, it continues to appear on those work items after you hide it. </p></td> 
    </tr> 
   </tbody> 
  </table> <note type="tip">
   You can standardize condition terminology and colors across all three object types. To do this, copy the condition Name and the Color hex code from one tab (Project, Task, Issue) to the corresponding condition on the other two tabs. 
  </note> </li> 
 <li value="6"> <p>(Optional) Drag <img src="assets/move-icon---dots.png"> any condition to a new position to re-order the list.</p> <p>This changes the order in which conditions display in projects, tasks and issues:</p> 
  <ul> 
   <li> <p>When a user is editing a project</p> <p> <img src="assets/change-condition-edit-project-350x96.png" style="width: 350;height: 96;"> </p> </li> 
   <li> <p>When a user is changing the condition for a task or issue on the Updates tab:</p> <p> <img src="assets/change-condition-update-comment-350x141.png" style="width: 350;height: 141;"> </p> </li> 
   <li> <p>When a user is changing the condition for a task or issue in a list view:</p> <p> <img src="assets/change-conditions-list-drop-down-only-350x172.png" style="width: 350;height: 172;"> </p> </li> 
  </ul> </li> 
 <li value="7">Click <span class="bold">Save</span>.</li> 
</ol>

You can set your custom condition as a default condition for projects or for tasks and issues. For more information, see [Set a custom condition as the default for projects](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) and [Set a custom condition as the default for tasks and issues](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

For more information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
