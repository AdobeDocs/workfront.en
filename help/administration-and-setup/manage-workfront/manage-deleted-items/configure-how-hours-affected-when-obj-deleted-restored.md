---
filename: configure-how-hours-affected-when-obj-deleted-restored
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configure affect on hours when an object is deleted and restored
description: You can configure what happens to hours when someone deletes a project, task, or issue that the hours are logged against. The option you choose also determines what happens to the hours if the project, task, or issue is restored at a later time. (For more information about restoring items in Workfront, see Restore deleted items.)
---

# Configure affect on hours when an object is deleted and restored

You can configure what happens to hours when someone deletes a project, task, or issue that the hours are logged against. The option you choose also determines what happens to the hours if the project, task, or issue is restored at a later time. (For more information about restoring items in Workfront, see [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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

## Configure how hours are managed when an item is deleted and restored

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">Expand&nbsp;<span class="bold">Timesheets & Hours</span>, then click<span class="bold"> Preferences</span>.</li> 
 <li value="3">Locate the <span class="bold">Project, Task or Issue Deletion Preferences</span> section.</li> 
 <li value="4">(Conditional) To configure how hours are managed when a project is deleted, select one of the following options in the <span class="bold">When deleting projects</span> section:</li> 
 <ul> 
  <li>Keep logged hours already added to timesheets as general hours (If this project is restored at a later time, the hours remain on the timesheet)<br>This option is selected by default.</li> 
  <li>Delete any logged hours (If this project is restored at a later time, logged hours are restored to the project)</li> 
 </ul> 
 <li value="5">(Conditional) To configure how hours are managed when a task or issue&nbsp;is deleted, select one of the following options in the <span class="bold">When deleting tasks or issues</span>&nbsp;section:</li> 
 <ul> 
  <li>Move any logged hours to the project where the task or issue resides (If this task or issue is restored at a later time, the hours remain on the project)<br>This option is selected by default.</li> 
  <li>Delete any logged hours (If this task or issue is restored at a later time, logged hours are restored to the task or issue)</li> 
 </ul> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

