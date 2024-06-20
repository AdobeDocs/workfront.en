---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Make smart assignments
description: You can use smart assignments to identify who the best user is to complete the work. Smart assignments are suggestions for users, roles, or teams that Adobe Workfront presents to you when you assign work items to resources based on an algorithm that determines the most appropriate resource for the job. For information about smart assignments, see Smart assignments overview.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
---
# Make smart assignments

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

You can use smart assignments to identify who the best user is to complete the work. 

Smart assignments are suggestions for users, roles, or teams that Adobe Workfront presents to you when you assign work items to resources. Workfront bases its suggestions on an algorithm that determines the most appropriate resource for the job.

<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues. </span>

For more information about the criteria used in determining smart assignments, see [Smart assignments overview](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Access requirements

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
   <td role="rowheader">Adobe Workfront license*</td> 
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

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Make smart assignments

Smart assignments are available in most locations where you can make assignments in Workfront.

1. Go to an the following areas the click the **Assignments** or **Assign this to** field: 

   * A task or issue list or report 
   * A task or issue header
   * The task or issue Summary panel
   * <span class="preview">A New Task or New Issue box, as you add a new task or issue to a project</span>
   * The Assignments field for an item listed in the Home area
   * A task or issue in the Workload Balancer

1. Place your cursor in the Assignments field, and wait for two seconds. 

   <div class="preview">
   One or several of the following sections with smart assignment suggestions displays: 

   * **Suggested assignments**: Displays for tasks. <!--remove the note when we go to production with smarter assignments-->

      >[!TIP]
      >
      >   The list header displays **Here are a few recommendations** instead of **Suggested assignments** in the Production environment.
      >
   * **Users and teams**: Displays for tasks and issues.
   * **Job roles**: Dispays for tasks and issues. 
   * **Rate card job roles**: Displays for tasks. For more information, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>
   
   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>

     
   For tasks, the smart assignments display in the following sections, depending on which phase of the algorithm's calculation identified the assignments: 

   * **Suggested assignments**: Assignments identified in the first phase of the task smart assignment's algorithm calculation. <span class="preview">This section is not available for issues.</span>
   * <span class="preview">**Users and teams**, **Job roles**, or **Rate card job roles**: Assignments identified in the second phase of the task smart assignment's algorithm calculation. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>
   
   For more information, see [Smart assignments overview](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Select the user in the recommendations list by clicking their name. 

1. (Optional) Click **Assign to me** to assign the work item to yourself.

   >[!TIP]
   >
   >If there are no suggestions, the suggestion list does not open.

1. (Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired resource and select the name when it appears in the list.
1. Click **Enter** to make the assignment.

   The selected user is assigned to the task or issue.
