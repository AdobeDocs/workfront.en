---
filename: manage-allocation-percentage-on-tasks
product-area: projects;user-management
navigation-topic: assign-tasks
title: Manage allocation percentage on tasks
description: Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task.
---

# Manage allocation percentage on tasks

Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task.

>[!NOTE]
>
>When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task</p> <p>Edit permissions to update allocation percentage in the Edit Task box</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations about modifying percent allocations for tasks

* Users are allocated an equal percentage of time to tasks they are assigned to, by default. 
* You can manually modify the allocation percentage for users and job roles assigned to tasks only when the Duration Type of the task is Calculated Work or Effort Driven.

  For information, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 

* You cannot modify the percent allocation for teams assigned to tasks.
* You cannot modify the percentage allocation for users and job roles assigned to issues.

## Modify the percent allocation for a task

<ol> 
 <li value="1">Go to a task for whose resources you are changing the percent allocation.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the name of the task, then click <span class="bold">Edit</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the name of the task, then click <span class="bold">Edit</span>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Assignments</span> area in the task header, then click&nbsp;<span class="bold">Advanced</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Assignments</span> area in the task header, then click&nbsp;<span class="bold">Advanced</span>.</p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Ensure that the <span class="bold">Duration&nbsp;Type</span> of the task is one of the following:</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Ensure that the <span class="bold">Duration&nbsp;Type</span> of the task is one of the following:</p> 
  <ul> 
   <li>Calculated Work</li> 
   <li>Effort Driven</li> 
  </ul> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li> <p>For the Calculated Assignment Duration Type, <em>Workfront</em> uses the following formula to calculate the allocation percentage of each assignee: </p> <p><code>Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day </code>/ <code>Number of assignees</code>.</p> </li> 
   </ul> 
   <ul> 
    <li>For the Simple Duration Type, you can estimate the hours assigned to each resource, not the allocation percentage. </li> 
   </ul> 
  </div> </li> 
 <li value="4"> <p>Click <span class="bold">Assignments</span>, then modify the <draft-comment>
    <span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Allocations</span>
   </draft-comment><span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Allocations</span> for each task assignee. </p> <p>You can only modify the allocation percentage for user and job role assignments. </p> <p>You cannot modify the allocation percentage for a team assigned to a task.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png" style="width: 350;height: 251;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png" style="width: 350;height: 251;"> </p> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

