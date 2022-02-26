---
filename: adjust-budgeting-dates
product-area: resource-management
navigation-topic: resource-planning
title: Adjust budgeting dates in the Resource Planner
description: If you find that there are overallocations of your resources after you have budgeted them in the Resource Planner, you can explore what-if scenarios by moving the Budgeted Hours, FTE, or Costs to another time frame. Based on the findings in these scenarios, you can then adjust your budgeted Hours, FTE, or Cost.
---

# Adjust budgeting dates in the *Resource Planner*

If you find that there are overallocations of your resources after you have budgeted them in the *Resource Planner*, you can explore what-if scenarios by moving the Budgeted Hours, FTE, or Costs to another time frame. Based on the findings in these scenarios, you can then adjust your budgeted Hours, FTE, or Cost.

Overallocations can appear when the Budgeted Hours, FTE, or Costs of your resources are higher then their Available Hours, FTE, or Costs. This generates a negative Net value.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Resource Management that includes access to&nbsp;Edit priorities and budget hours in the <em>Resource Planner</em></p> <p>Edit access to Financial Data, Projects, and Users</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the projects you want to budget information for with ability to Manage Finances</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## `Adjust Budgeting Dates`

<ol> 
 <li value="1"> <p> Go to the <em>Resource Planner</em> and select <span class="bold">View by Project</span>.</p> <note type="note">
   You can use the Adjust Budgeted Dates option only when you view the 
   <em>Resource Planner</em> by project. 
  </note> </li> 
 <li value="2"> Hover over the name of a project, then click the <span class="bold">More</span> menu. </li> 
 <li value="3"> <p>Click <span class="bold">Adjust Budgeting Dates</span>.<br>The project allocation timeline is displayed.<br>The time frame where the hours are currently budgeted is highlighted in orange if there is a budgeting conflict and in blue if there are no conflicts. </p> <p> <img src="assets/rp-adjust-budgeting-dates-with-no-done-button-350x106.png" style="width: 350;height: 106;"> </p> </li> 
 <li value="4"> Drag and drop the highlighted time frame to another time to understand where there are no budgeting conflicts for the selected project. When you find a time frame where the Net value is positive, the highlighted time frame changes to blue. </li> 
 <li value="5">Click the "x" in the upper right corner of the project allocation timeline to close it. </li> 
 <li value="6"> Remove the budgeted hours from the existing timeline of the project and add them to the timeline that shows the most availability. </li> 
 <li value="7"> Click <span class="bold">Save</span>. </li> 
 <li value="8"> (Conditional and optional) If the time frames without budgeting conflicts are outside the timeline of the project, click the name of the project to access the project. </li> 
 <li value="9"> (Conditional and optional) Click <span class="bold">Edit Project</span>, then edit the <span class="bold">Planned Start Date</span> or the <span class="bold">Planned Completion Date</span> to modify the timeline of the project for the time frame with no budgeting conflicts. <br>For more information about editing projects, see the article <a href="../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li> 
 <li value="10"> (Conditional and optional) Click <span class="bold">Save Changes</span>. </li> 
 <li value="11"> Return to the <em>Resource Planner</em> and re-enter the Budgeted Hours, FTEs, or Costs in the time frame without budgeting conflicts. </li> 
 <li value="12"> Click <span class="bold">Save</span>. </li> 
</ol>

