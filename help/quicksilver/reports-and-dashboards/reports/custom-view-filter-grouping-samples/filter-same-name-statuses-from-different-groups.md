---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: display items by same-name statuses when the statuses are associated with different groups'
description: You can have a task status assigned to Group A named New Status with the 3-letter key NST. You may have another task status assigned to Group B also named New Status with the 3-letter key NES. Although the names for the 2 statuses can be identical, the 3-letter code is always unique. For more information about group statuses, see Create or edit a group status.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
---
# Filter: display items by same-name statuses when the statuses are associated with different groups

You can have a task status assigned to Group A named *New Status* with the 3-letter key *NST*. You may have another task status assigned to Group B also named *New Status* with the 3-letter key *NES.* Although the names for the 2 statuses can be identical, the 3-letter code is always unique.  
For more information about group statuses, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Using the filter builder, you cannot identify between the 2 statuses that have the same name. You must use Text&nbsp;Mode to distinguish between the 2 statuses.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request to modify a filter </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Display items by same-name statuses when the statuses are associated with different groups

1. Go to the filter you want to customize for a list of tasks, for example.  
   This works the same for projects and issues as well.
1. Click **Add a Filter Rule** for the **Status** field of the object of your list.  
   For example, in a task report, add **Status Equal New Status**, if you want to display only tasks which are in a status of **New Status**.

   >[!TIP]
   >
   >Notice that you have only one option for a status named New Status.

1. Click **Switch to Text Mode**.  
   The following code should display:  
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Only one status displays here. The status line displays one of the 3-letter keys for one of the statuses.

1. Add the following 2 lines of code to add the status that is missing from the filter:  
   <pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>

1. Click&nbsp;**Done**, then **Save Filter**.

   The list displays both tasks with a status of "New Status" from Group A and with a status of "New Status"&nbsp;from Group B.
