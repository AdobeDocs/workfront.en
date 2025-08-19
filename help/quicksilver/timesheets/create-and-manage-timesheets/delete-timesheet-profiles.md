---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Delete timesheet profiles
description: You can delete a timesheet profile that might no longer be relevant.
author: Alina
feature: Timesheets
exl-id: 1fb39f74-205b-485e-9e8b-a2ab3f9f1ac4
---
# Delete timesheet profiles

<!--Audited:6/2025-->

Creating and assigning timesheet profiles to users ensures consistency in the way Adobe Workfront creates their timesheets.

You can delete a timesheet profile that might not be releavant anymore.

For information about timesheet profiles, see [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Access requirements

+++ Expand to view access requirements. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   Or
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must have administrative access to Timesheets. </p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Delete timesheet profiles

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. If you are deleting a system-level timesheet profile, click **Timesheet & Hours**.

   Or

   If you deleting a timesheet profile for a group, click **Groups** > click the group's name, then click **Timesheet Profiles**.
1. Select at least one timesheet profile that you want to delete, then click the **More** icon ![](assets/more-icon.png) > **Delete** for the system-wide timesheet profile

1. Click **Timesheet Profiles**.
1. Select at least one timesheet profile that you want to delete, then click the more icon ![more icon](assets/more-icon.png) > **Delete**.
   Or
   Click **More** > **Delete** for the group-level timesheet profile.
1. (Conditional) If the timesheet profile is already assigned to users, the **Replacement Timesheet Profile** box displays. Do the following:
   1. Select another timesheet profile from the drop-down list. The timesheet profile you are deleting will be replaced by the timesheet profile you replace it with for all assigned users. Timesheets will generate according to the newly assigned profile in the following timesheet generation cycle. 
   1. Click **Delete It** to confirm the deletion. 
1. (Conditional) If the timesheet profile is not assigned to users, the **Delete Timesheet** box displays.

   Click **Delete** to confirm the deletion.
