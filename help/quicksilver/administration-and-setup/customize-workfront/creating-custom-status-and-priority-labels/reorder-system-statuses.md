---
filename: reorder-system-statuses
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Reorder system-level and group statuses
description: As a Workfront administrator, you can change the order of project, task, and issue statuses for everyone in the system or for a single group.
---

# Reorder system-level and group statuses

As a Workfront administrator, you can change the order of project, task, and issue statuses for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> everyone in the system or for a single group</MadCap:conditionalText>```.

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.</p>
-->

![](assets/statuses-350x116.png)

>[!NOTE]
>
>* Reordering the statuses at the system level doesn't affect the order of statuses within groups.
>
>  However, the statuses within a newly created top-level group inherit the order of the system-level statuses. (A new subgroup inherits the order of the statuses in the group one level up.)
>
>* You can reorder locked statuses. For information about locked statuses, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Group administrators can also reorder statuses used in their groups. For more information, see [Reorder group statuses](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan* </td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## Default order of statuses

By default, statuses display in the following order:

<table> 
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
    <ul> 
     <li>Current</li> 
     <li>Dead</li> 
     <li> On Hold </li> 
     <li> Planning </li> 
     <li> Complete </li> 
     <li> Requested </li> 
     <li> Approved </li> 
     <li> Rejected </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Complete</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Reopened</li> 
     <li>Awaiting Feedback</li> 
     <li>On Hold</li> 
     <li>Cannot Duplicate</li> 
     <li>Closed</li> 
     <li>Resolved</li> 
     <li>Verified Complete</li> 
     <li>Won't Resolve</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Reorder statuses for tasks and projects system wide or for a group

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Project Preferences > Statuses**.
1. (Conditional) If you are reordering statuses for a group, start typing the name of the group in the box in the upper-right corner, then click the name when it appears.

   ![](assets/system-statuses-in-upper-rt-corner-group-350x139.jpg)

1. Above the Statuses list that displays, click the **Projects** or **Tasks** tab.

1. Drag and drop the statuses in the order you want.

   The new status order is saved automatically.

1. To test the new status order, go to a task or project, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.

## Reorder statuses for issues

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Project Preferences > Statuses.**
1. (Conditional) If you are reordering statuses for a group, start typing the name of the group in the box in the upper-right corner, then click the name when it appears.

   ![](assets/issue-statuses-group-name-350x162.png)

1. Click the **Issues** tab.
1. (Optional) Select an issue type (**Bug Report**, **Change Order**, **Issue**, or **Request**).

   >[!NOTE]
   >
   >* You cannot customize the order of statuses for the Master List.
   >* We recommend that you order of statuses for each issue type the same way. For more information about issue types, see [Configure request types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Drag and drop the statuses in the order you want.

   The new status order is saved automatically.

1. To test the new status order, go to an issue, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.

