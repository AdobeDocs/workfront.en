---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Display Items by Same-name Statuses When the Statuses Are Associated with Different Groups'
description: You can have a task status assigned to Group A named New Status with the 3-letter key NST. You may have another task status assigned to Group B also named New Status with the 3-letter key NES. Although the names for the 2 statuses can be identical, the 3-letter code is always unique. For more information about group statuses, see Create or edit a group status.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
---
# Filter: display items by same-name statuses when the statuses are associated with different groups

<!--Audited: 10/2024-->

You can have a task status assigned to Group A named *New Status* with the 3-letter key *NST*. You may have another task status assigned to Group B also named *New Status* with the 3-letter key *NES.* Although the names for the 2 statuses can be identical, the 3-letter code is always unique.

For more information about group statuses, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Using the filter builder, you cannot identify between the 2 statuses that have the same name. You must use Text Mode in a custom filter to distinguish between the 2 statuses.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Display items by same-name statuses when the statuses are associated with different groups

1. Go to the **Filter** drop-down for the filter that you want to customize for a list of tasks, for example.  
   This works the same for projects and issues as well.
1. Click **New filter**.
1. From the first drop-down in the upper-left corner, select Task > Status. 
1. Select **Equals** for the modifier, then select one of the statuses you want to report on. 

   For example, in a task report, add **Status Equals New Status**, if you want to display only tasks which are in a status of **New Status**.

   >[!TIP]
   >
   >Notice that you have only one option for a status named New Status.

1. Click **Text Mode**.  
   The following code should display in the space provided:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Only one status displays here. The status line displays one of the 3-letter keys for one of the statuses.

1. Add the following 2 lines of code to add the status that is missing from the filter:  

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Click **Apply**, then **Save as new**.

   The list displays both tasks with a status of "New Status" from Group A and with a status of "New Status" from Group B.
