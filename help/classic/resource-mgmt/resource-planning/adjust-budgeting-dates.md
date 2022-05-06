---
filename: adjust-budgeting-dates
product-area: resource-management
navigation-topic: resource-planning
title: Adjust budgeting dates in the Resource Planner
description: If you find that there are overallocations of your resources after you have budgeted them in the Resource Planner, you can explore what-if scenarios by moving the Budgeted Hours, FTE, or Costs to another time frame. Based on the findings in these scenarios, you can then adjust your budgeted Hours, FTE, or Cost.
---

# Adjust budgeting dates in the Resource Planner

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

If you find that there are overallocations of your resources after you have budgeted them in the Resource Planner, you can explore what-if scenarios by moving the Budgeted Hours, FTE, or Costs to another time frame. Based on the findings in these scenarios, you can then adjust your budgeted Hours, FTE, or Cost.

Overallocations can appear when the Budgeted Hours, FTE, or Costs of your resources are higher then their Available Hours, FTE, or Costs. This generates a negative Net value.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Resource Management that includes access to&nbsp;Edit priorities and budget hours in the Resource Planner</p> <p>Edit access to Financial Data, Projects, and Users</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the projects you want to budget information for with ability to Manage Finances</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## **Adjust Budgeting Dates**

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

