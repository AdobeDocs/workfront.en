---
product-area: projects
navigation-topic: update-work-in-a-project
title: View and Update Percent Complete for Tasks
description: You can update the percent complete of a task to indicate the progress that you have made on the task towards completing it. Updating the percent complete for issues is similar to updating it for a task. This article describes how to update the percent complete of a task.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/1r6vdvrnoBbelMtKkHNUHSJ7ppNWcwK0g15omdYWtCM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# View and update Percent Complete for tasks

<!--Audited: 05/2025-->

You can update the percent complete of a task to indicate the progress that you have made on the task towards completing it. 

Updating the percent complete for issues is similar to updating it for a task. This article describes how to update the percent complete of a task. 

## Access Requirements

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
   <td> <p>Standard</p> 
   <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
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
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Areas where you can update the percent complete of a task

You can update the percent complete for a task in any of the following areas:

* **In a task list**: You can update the percent complete of a task when the Percent Complete column displays. 

  For more information about inline editing, see [Inline edit items in a list in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In the Milestone view**: You can update the percent complete of a task when using the Milestone view on a project list or a project report. 

  >[!TIP]
  >
  >  You cannot update the percent complete of issues in the Milestone view. 


  For more information, see [Use the Milestone view](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **In the task header**: You can update the percent complete of a task in the task header. 

  ![Update percent in header](assets/nwe-updatetaskpercentinheader-350x54.png)

* **In the Summary panel of a task**: You can update the percent complete of a task at the top of the Summary panel when viewing the task in the following areas: 

  * Task list or report
  * Timesheet
  * Workload Balancer

  ![Update percent in task Summary highlighted](assets/update-percent-complete-in-task-summary-highlighted.png)
  
  For more information, see [Summary overview](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Home**: You can update the percent complete of a task or issue from the Summary panel in the Home area, or from the My Work widget. 

  For information, see  [Getting started with Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md). 

## Considerations about updating the percent complete of a task

* When you mark a task as 100% complete, the task Status updates to Complete. An issue's status updates to Closed.
* Completing a task also updates the percent complete of the parent and of the project. 
* The following scenarios exist for parent tasks and projects: 
  * You cannot update the percent complete of a parent task to 100% when the Summary Completion Mode of the project is set to Automatic and the subtasks are not completed.
  * You can update the percent complete of a parent task or of a project to 100% when the Summary Completion Mode of the project is set to Manual and the subtasks are completed or incomplete. 

  For more information, see [Edit projects](../manage-projects/edit-projects.md).

## Update the percent complete of a task

1. Go to any of the areas where you want to update the percent complete of a task. 

    For information, see the section [Areas where you can update the percent complete of a task](#areas-where-you-can-update-the-percent-complete-of-a-task) in this article. 
    
1. Locate the **Percent Complete** field for the task whose percent complete you want to update. 

    >[!TIP]
    >
    >The Percent Complete field always displays at the top of the Summary panel.

1. Click inside the **Percent Complete** field and type a number between 0 and 100
    
    Or

    Click and drag the **Percent Complete** blue bubble to the necessary number to indicate how much of the task you completed, when available.

    >[!NOTE]
    >
    >    * You cannot enter a decimal number when you click inside the Percent Complete bubble.
    >    * When you drag and drop the blue bubble in the Summary panel, the Percent Complete updates in one point increments.
    >
    >    * When you drag and drop the blue bubble in the task header, the Percent Complete updates in 5 point increments.

1. Press Enter on your keyboard to save the percent complete. 

    The Percent Complete of the project or any parent tasks might also automatically update. 

    The status of the task or of the issue also updates. 

