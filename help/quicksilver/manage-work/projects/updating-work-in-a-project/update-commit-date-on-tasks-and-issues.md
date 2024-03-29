---
product-area: projects
navigation-topic: update-work-in-a-project
title: Update Commit Dates on tasks and issues
description: You can manually update the Commit date of a task or an issue that you are assigned to. For more information about Commit Dates in Adobe Workfront, see Commit Date overview.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
---
# Update Commit Dates on tasks and issues

You can manually update the Commit date of a task or an issue that you are assigned to. For more information about Commit Dates in Adobe Workfront, see [Commit Date overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Access requirements

<!--Audited: 01/2024-->

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
   <td> 
   For the new licenses:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For current licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Prerequisites

Before you begin, you must be assigned to the task or issue you need to update the Commit Date for.

## Update Commit Dates on tasks and issues

Updating the Commit Date is identical for tasks and issues.

1. Go to a task or issue that you are assigned to as the **Owner**.

   For more information about finding out who the Task Owner for an issue or task is, see the section [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) in the article [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Click **Task Details** or **Issue Details** in the left panel. 
1. Click **Overview** to expand it.
1. Update the **Commit Date** field.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Click **Save Changes**.

   The following happens after making this change:&nbsp;

   * The Commit Date and the Planned Completion date of the task or issue are no longer the same.

     Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * If you are using the legacy Updates area, the Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. This functionality is not supported in the new commenting experience. For information, see [The new commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     For information about the notifications and updates that are triggered by this change, see the section [Notifications and updates triggered by changing the Commit Date](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) in the article [Commit Date overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
