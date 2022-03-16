---
filename: reorder-group-statuses-from-groups-area
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Reorder group statuses
description: s mAs a group administrator, you can change the order of project, task, and issue statuses for a group you manage.
---

# Reorder group statuses

s mAs a group administrator, you can change the order of project, task, and issue statuses for a group you manage.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

>[!NOTE]
>
>* A Workfront administrator can reorder the statuses at the system level. This does not affect the order of statuses within groups. 
>
>  However, the statuses within a newly created top-level group inherit the order of the system-level statuses. (A new subgroup inherits the order of the statuses in the group one level up.)
>
>* You can reorder locked statuses. For information about locked statuses, see Create or edit a group status.
>

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>* </td> 
   <td> <p>Any</p> </td> 
  </tr> Adobe Workfront license* Plan You must be a group administrator of the group or a Workfront administrator. For more information, see Group administrators and Grant a user full administrative access. 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## Default order of statuses

By default, statuses display in the following order:

<table cellspacing="15"> 
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

Reorder statuses for tasks and projects in a group Click Setup near the upper-right corner of Adobe Workfront on the Global Navigation Bar. In the left panel, click Groups. Select the name of the group, then click More > Settings. In the left panel, click Statuses. Above the Statuses list that displays, click the Projects or Tasks tab. Drag and drop the statuses in the order you want. The new status order is saved automatically. To test the new status order, go to a task or project associated with the group, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured. Reorder statuses for issues Click Setup near the upper-right corner of Adobe Workfront on the Global Navigation Bar. In the left panel, click Groups, then click the name of the group. In the left panel, click Statuses. Click the Issues tab. (Optional) Select an issue type (Bug Report, Change Order, Issue, or Request). Note: You cannot customize the order of statuses for the Master List. We recommend that you order of statuses for each issue type the same way. For more information about issue types, see Configure request types. Drag and drop the statuses in the order you want. The new status order is saved automatically. To test the new status order, go to an issue associated with the group, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.  