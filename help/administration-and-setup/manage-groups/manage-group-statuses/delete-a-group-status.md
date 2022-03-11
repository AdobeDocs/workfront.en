---
filename: delete-a-group-status
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Delete a group status
description: As a group administrator, you can delete a status for a group that you manage if it is not configured as a required or locked status on the system level or for a higher group in the hierarchy.
---

# Delete a group status

As a group administrator, you can delete a status for a group that you manage if it is not configured as a required or locked status on the system level or for a higher group in the hierarchy.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## Delete a group status

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span>.</li> 
 <li value="3"> Click the name of the top-level group.</li> In the left panel click Statuses. 
 <li value="5"> <p>In the list of statuses that displays, hover over the status you want to delete, then click <span class="bold">Delete</span> when it appears to the far right.</p> <p> <img src="assets/hover-click-delete-350x141.jpg" style="width: 350;height: 141;"> </img> </p> </li> 
 <li value="6"> <p> In the box that displays, select a status to designate a replacement status for objects (projects, tasks, issues, and approval processes) that were using the status that you are deleting.</p> <p>Only statuses that equate with the status you are deleting are available. For example, if you are deleting a status that equates with Current, you can see only statuses that equate with Current.</p> <p>Also, the statuses that display depend on whether the status you are deleting is unlocked or locked:</p> 
  <ul> 
   <li> <p><span class="bold">If it's unlocked</span>: Non-hidden locked and unlocked statuses are available.</p> <p>Along with the statuses that were created for the subgroup, statuses inherited from system-level and upper level groups are included.</p> </li> 
   <li> <p><span class="bold">If it's locked</span>: One of the following is true:</p> 
    <ul> 
     <li>If there are other locked, non-hidden statuses, only those are available.</li> 
     <li> <p>If there is no locked non-hidden status, the default Workfront status is available, even if it’s hidden or unlocked.</p> <p>For information about the default Workfront statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">Access the list of system project statuses</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref">Access the list of system task statuses</a>, and the information about the 4 required issue statuses in <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>.</p> </li> 
    </ul> </li> 
  </ul> </li> 
 <li value="7"> <p> Click <span class="bold">Delete Status</span>.</p> 
  <div> 
   <ul> 
    <li>If the deleted status was the default status for that type in the group, the replacement status takes its place.</li> 
    <li>If the deleted status was set as the default project status in project preferences, the preference is now set to the replacement status.</li> 
   </ul> 
  </div> </li> 
</ol>

## When a group is deleted

When a group is deleted and replaced by another group, any unique statuses that the deleted group had are added to the statuses of the replacement group. For more information, see [Custom statuses in a group that is moved or deleted](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
