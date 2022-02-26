---
filename: manage-allocation-hours-on-tasks
product-area: projects;user-management
navigation-topic: assign-tasks
title: Manage allocation hours on tasks
description: When assigning users or roles to a task, they are allocated to work a certain number of hours to complete the task. You can manually modify the amount of hours that each user or job role is allocated when they are assigned to a task when the task Duration Type is Simple.
---

# Manage allocation hours on tasks

When assigning users or roles to a task, they are allocated to work a certain number of hours to complete the task. You can manually modify the amount of hours that each user or job role is allocated when they are assigned to a task when the task&nbsp;Duration&nbsp;Type is Simple.

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
   <td> <p>Contribute or higher permissions to the task</p> <p>Edit permissions to update allocation hours in the Edit Task box</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations for modifying the allocation hours for a task

>[!IMPORTANT]
>
>After you manually modify assignment allocations on tasks, the Planned Hours of the tasks might update accordingly. For more information, see the section "Update task Planned Hours when managing user allocations" in the article [Planned Hours overview](../../../manage-work/tasks/task-information/planned-hours.md).

* The total of hours allocated to individual resources assigned to the task represents the Planned Hours of the task. 
* If there is one user or role assignment to a task, the amount of hours allocated to the user or role matches the Planned Hours of the task.
* In the case of multiple assignments, each user or job role is assigned an equal amount of hours to work on the task, by default, if the task Duration Type is Simple. For more information, see the following articles:

  * [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) 
  * [Duration Type overview: Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* When the task has a Simple Duration&nbsp;Type, you can manually change the amount of allocated hours for each user or job role to indicate that some of the task assignees might have more time to work on a task than others. 
* You cannot modify the amount of hours allocated to teams assigned to tasks.
* You cannot manually modify the user or job role allocation for issues. 
* You can also manage daily, weekly, or monthly allocations of users to tasks or issues by using the *Workload Balancer*. For more information, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modify the allocation hours for a task

<ol> 
 <li value="1">Go to a task for whose assignments you want to change the allocation hours.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the name of the task, then click <span class="bold">Edit</span>, then <span class="bold">Assignments</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the name of the task, then click <span class="bold">Edit</span>, then <span class="bold">Assignments</span>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Assignments</span> area in the task header, then click&nbsp;<span class="bold">Advanced</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Assignments</span> area in the task header, then click&nbsp;<span class="bold">Advanced</span>.</p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Ensure that the <span class="bold">Duration&nbsp;Type</span> of the task is <span class="bold">Simple</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Ensure that the <span class="bold">Duration&nbsp;Type</span> of the task is <span class="bold">Simple</span>.</p> </li> 
 <li value="4"> <p>Modify the <draft-comment>
    <span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Allocations</span>
   </draft-comment><span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Allocations</span> for each task assignee. These are overall allocations for each assignments to this task, for the entire duration of the task. This might also update the overall Planned Hours of the task. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png" style="width: 350;height: 198;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png" style="width: 350;height: 198;"> </p> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

