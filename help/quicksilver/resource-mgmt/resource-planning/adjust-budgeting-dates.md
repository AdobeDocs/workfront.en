---
product-area: resource-management
navigation-topic: resource-planning
title: Adjust Budgeting Dates in the Resource Planner
description: If you find that there are overallocations of your resources after you have budgeted them in the Resource Planner, you can explore what-if scenarios by moving the Budgeted Hours, FTE, or Costs to another time frame. Based on the findings in these scenarios, you can then adjust your budgeted Hours, FTE, or Cost.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
---
# Adjust budgeting dates in the Resource Planner

If you find that there are overallocations of your resources after you have budgeted them in the Resource Planner, you can explore what-if scenarios by moving the Budgeted Hours, FTE, or Costs to another time frame. Based on the findings in these scenarios, you can then adjust your budgeted Hours, FTE, or Cost.

Overallocations can appear when the Budgeted Hours, FTE, or Costs of your resources are higher then their Available Hours, FTE, or Costs. This generates a negative Net value.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
    <td><p>New: Any</p>
       <p>or</p>
       <p>Current: Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>or</p>
       <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Resource Management that includes access to Edit priorities and budget hours in the Resource Planner</p> <p>Edit access to Financial Data, Projects, and Users</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the projects you want to budget information for with ability to Manage Finances</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adjust Budgeting Dates

1. Go to the Resource Planner and select **View by Project**.

   >[!NOTE]
   >
   >You can use the Adjust Budgeted Dates option only when you view the Resource Planner by project.

1. Hover over the name of a project, then click the **More** menu. 
1. Click **Adjust Budgeting Dates**.  
   The project allocation timeline is displayed.  
   The time frame where the hours are currently budgeted is highlighted in orange if there is a budgeting conflict and in blue if there are no conflicts.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Drag and drop the highlighted time frame to another time to understand where there are no budgeting conflicts for the selected project. When you find a time frame where the Net value is positive, the highlighted time frame changes to blue. 
1. Click the "x" in the upper right corner of the project allocation timeline to close it. 
1. Remove the budgeted hours from the existing timeline of the project and add them to the timeline that shows the most availability. 
1. Click **Save**. 
1. (Conditional and optional) If the time frames without budgeting conflicts are outside the timeline of the project, click the name of the project to access the project. 
1. (Conditional and optional) Click **Edit Project**, then edit the **Planned Start Date** or the **Planned Completion Date** to modify the timeline of the project for the time frame with no budgeting conflicts.   
   For more information about editing projects, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Conditional and optional) Click **Save Changes**. 
1. Return to the Resource Planner and re-enter the Budgeted Hours, FTEs, or Costs in the time frame without budgeting conflicts. 
1. Click **Save**.
