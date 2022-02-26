---
filename: filter-same-name-statuses-from-different-groups
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Filter: display items by same-name statuses when the statuses are associated with different groups
description: You can have a task status assigned to Group A named New Status with the 3-letter key NST. You may have another task status assigned to Group B also named New Status with the 3-letter key NES. Although the names for the 2 statuses can be identical, the 3-letter code is always unique. For more information about group statuses, see Create or edit a group status.
---

# Filter: display items by same-name statuses when the statuses are associated with different groups

You can have a task status assigned to Group A named *New Status* with the 3-letter key *NST*. You may have another task status assigned to Group B also named *New Status* with the 3-letter key *NES.* Although the names for the 2 statuses can be identical, the 3-letter code is always unique.  
For more information about group statuses, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Using the filter builder, you cannot identify between the 2 statuses that have the same name. You must use Text&nbsp;Mode to distinguish between the 2 statuses.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Display items by same-name statuses when the statuses are associated with different groups

<ol> 
 <li value="1">Go to the filter you want to customize for a list of tasks, for example.<br>This works the same for projects and issues as well.</li> 
 <li value="2"> <p>Click <span class="bold"> Add a Filter Rule</span> for the <span class="bold">Status</span> field of the object of your list.<br>For example, in a task report, add <span class="bold">Status Equal <em>New Status</em></span>, if you want to display only tasks which are in a status of <span class="bold">New Status</span>.</p> <note type="tip">
   Notice that you have only one option for a status named New Status.
  </note> </li> 
 <li value="3">Click <span class="bold">Switch to Text Mode</span>.<br>The following code should display:<br><pre xml:space="preserve">status=NST<br>status_Mod=in </pre><note type="note">
   Only one status displays here. The status line displays one of the 3-letter keys for one of the statuses.
  </note></li> 
 <li value="4">Add the following 2 lines of code to add the status that is missing from the filter:<br><pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre></li> 
 <li value="5"> <p>Click&nbsp;<span class="bold">Done</span>, then <span class="bold">Save Filter</span>.</p> <p>The list displays both tasks with a status of "New Status" from Group A and with a status of "New Status"&nbsp;from Group B.</p> </li> 
</ol>

