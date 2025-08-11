---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Make Smart Assignments
description: You can use smart assignments to identify who the best user is to complete the work. Smart assignments are suggestions for users, roles, or teams that Adobe Workfront presents to you when you assign work items to resources based on an algorithm that determines the most appropriate resource for the job. For information about smart assignments, see Smart assignments overview.
author: Lisa
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
---
# Make smart assignments

<!--Audited: 07/2024-->

You can use smart assignments to identify who the best user is to complete the work. 

Smart assignments are suggestions for users, roles, or teams that Adobe Workfront presents to you when you assign work items to resources. Workfront bases its suggestions on an algorithm that determines the most appropriate resource for the job.

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

For more information about the criteria used in determining smart assignments, see [Smart assignments overview](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p>
      Or
      <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p>View or higher access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions with the ability to make assignments on tasks and issues</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

+++

## Make smart assignments

Smart assignments are available in most locations where you can make assignments in Workfront.

1. Go to an the following areas the click the **Assignments** or **Assign this to** field: 

   * A task or issue list or report 
   * A task or issue header
   * The task or issue Summary panel
   * A task or issue in the Workload Balancer
   <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->
   
1. Place your cursor in the Assignments field, and wait for two seconds. 

   <!--For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![](assets/smart-assignments-issue-header.png)-->

   Smart assignments display in the following sections<!--, depending on which phase of the algorithm's calculation identified the assignments-->: 

      <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
      * **Users and teams** or **Job roles** <!--or **Rate card job roles**: Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

      ![Smart assignments example in task list](assets/smart-assignments-task-list.png)
   
      For more information, see [Smart assignments overview](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Select the resource in the recommendations list by clicking their name. 

1. (Optional) Click **Assign to me** to assign the work item to yourself.

   >[!TIP]
   >
   >If there are no suggestions, the suggestion list does not open.

1. (Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired resource and select the name when it appears in the list.
1. Click **Enter** to make the assignment.

   The selected user is assigned to the task or issue.
