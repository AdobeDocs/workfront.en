---
filename: use-custom-statuses-as-default-statuses
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Use custom statuses as default statuses
description: When a custom status is set as a default status, the new default status is used throughout the system in various ways. The ways in which it’s used depends on whether it is set as a default system-level status, or a default group-level status.
---

# Use custom statuses as default statuses

When a custom status is set as a default status, the new default status is used throughout the system in various ways. The ways in which it’s used depends on whether it is set as a default system-level status, or a default group-level status.

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

## `About setting custom default system-level statuses`

When you set a custom status as a default system status, any new groups created in the system inherit that status.

Groups that already existed when you set the new default system status do not automatically inherit it.

For example, suppose there are 2 groups already created in your Adobe Workfront environment (Marketing and Sales). You create a new custom status that equates with Current, and call the status In Process. You now create a new group called Engineering. In this scenario, the Engineering group inherits the new default status; the Marketing and Sales groups do not.

## `About setting custom default group-level statuses`

A custom status that you set as a default group status is used in the following circumstances:

* `When the Workfront system chooses a status automatically, the default group status is used:` The custom status that you set as the default group status is used when the Workfront system automatically assigns a status to an object.

  For example, a task can be&nbsp;configured to automatically change to Complete status when the percent complete reaches 100%. If you create a custom status that equates with Complete and you set that custom status as a default status, Workfront changes the status of the task to the new default status.

  Custom statuses are used in this way only with group statuses that are associated with a task or issue. Custom statuses cannot be used in this way for statuses associated with a project.

* The `status of a project is determined by the group associated with the project`: If the group associated with a given project changes, the status of the project changes depending on the default statuses defined for the group. (A group can be associated with a project via the `Groups` field when editing the project.)

  If that group changes, the status of the project changes if the new group has a different default status defined that equates with the current status of the project.

  For example, a project can be associated with the Marketing group, and the status of the project is set to Planning. The project is edited so that it is now associated with the Sales group. The Sales group has a custom default group status called Thinking (and this status equates with Planning). Because the Group on the project was changed, the status of the project changes now to Thinking.

## Set a custom status as a default status

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span> > <span class="bold">Statuses</span>.</li> 
 <li value="3">(Conditional) To set a default status for a group, begin typing the name of the group in the menu in the upper-right corner.</li> 
 <li value="4">Click the <span class="bold">Set Default Statuses</span> drop-down menu.</li> 
 <li value="5">In the drop-down area that displays, next to the status where you want to set the default status, select the default status you want.</li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
 <li value="7"> <p>Associate the project with the group where the status resides. <!--
    This step isn’t in older documentation
   --></p> <p>Users can use the custom status only if the group where the status resides is associated with the project. </p> <note type="note">
    If you are setting the custom status for a group, and you later assign the project to a different group, the project status will reload and could change.
  </note> 
  <ol> 
   <li value="1"> <p>Go to the project where you want to use the custom status.</p> </li> 
   <li value="2"> <p> Click the More menu , then click Edit. </p> </li> 
   <li value="3">In the <span class="bold">Edit Project</span> box that displays, in the <span class="bold">Group</span> field under <span class="bold">Project association</span>, select the group where the status resides.</li> 
   <li value="4">Click <span class="bold">Save Changes</span>.</li> 
  </ol> </li> 
</ol>

