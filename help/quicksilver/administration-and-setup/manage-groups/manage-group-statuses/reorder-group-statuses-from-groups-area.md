---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Reorder Group Statuses
description: As a group administrator, you can change the order of project, task, and issue statuses for a group you manage.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
---
# Reorder group statuses

As a group administrator, you can change the order of project, task, and issue statuses for a group you manage.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

>[!NOTE]
>
>* A Workfront administrator can reorder the statuses at the system level. This does not affect the order of statuses within groups. 
>
>  However, the statuses within a newly created top-level group inherit the order of the system-level statuses. (A new subgroup inherits the order of the statuses in the group one level up.)
>
>* You can reorder locked statuses. For information about locked statuses, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan* </td> 
   <td>Any</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## Default order of statuses

By default, statuses display in the following order:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Project</th> 
   <th width="33.33%">Task</th> 
   <th width="33.33%">Issue</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>Current</p> 
     <p>Dead</p> 
     <p> On Hold </p> 
     <p> Planning </p> 
     <p> Complete </p> 
     <p> Requested </p> 
     <p> Approved </p> 
     <p> Rejected </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>New</p> 
     <p>In Progress</p> 
     <p>Complete</p> 
   </td> 
   <td> 
     <p>New</p> 
     <p>In Progress</p> 
     <p>Reopened</p> 
     <p>Awaiting Feedback</p> 
     <p>On Hold</p> 
     <p>Cannot Duplicate</p> 
     <p>Closed</p> 
     <p>Resolved</p> 
     <p>Verified Complete</p> 
     <p>Won't Resolve</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Reorder statuses for tasks and projects in a group you manage

{{step-1-to-setup}}

1. In the left panel, click **Groups**, then click the name of the group.
1. In the left panel, click **Statuses**.
1. Above the Statuses list that displays, click the **Projects** or **Tasks** tab.

1. Drag and drop the statuses in the order you want.

   The new status order is saved automatically.

1. To test the new status order, go to a task or project associated with the group, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.

## Reorder statuses for issues

{{step-1-to-setup}}

1. In the left panel, click **Groups**, then click the name of the group.
1. In the left panel, click **Statuses**.
1. Click the **Issues** tab.
1. (Optional) Select an issue type (**Bug Report**, **Change Order**, **Issue**, or **Request**).

   >[!NOTE]
   >
   >* You cannot customize the order of statuses for the Master List.
   >* We recommend that you order of statuses for each issue type the same way. For more information about issue types, see [Configure request types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Drag and drop the statuses in the order you want.

   The new status order is saved automatically.

1. To test the new status order, go to an issue associated with the group, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.
