---
filename: associate-milestones-with-tasks
product-area: projects
navigation-topic: manage-tasks
title: Associate milestones with tasks
description: You can associate milestones with tasks to indicate when important steps in the lifetime of the project are reached.
---

# Associate milestones with tasks

You can associate milestones with tasks to indicate when important steps in the lifetime of the project are reached.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you can associate a milestone with a task, the following must exist:

* The Workfront administrator must create a milestone path, as described in [Create a milestone path](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* In order to associate a milestone path with a project, the project must be in Planning or Current status.

>[!TIP]
>
>To get the best overview of the progress of milestones in your projects using the Milestone view, you should create parent tasks and associate them with each major phase of your project. Then, associate these parent tasks with each of the milestones of your milestone path.

## Associate a milestone with a task

1. Go to a project, then click the More icon , then Edit. 
1. Using the `Settings` section, set the milestone path to be used on the project. 
1. Click `Save`. 
1. Go to a task, then click the More icon , then Edit. 
1. After a milestone path is associated with a project, tasks can be assigned a milestone.

   Tasks and Milestones have a 1:1 relationship. You cannot attach the same milestone to multiple tasks. Each task can be linked to a single milestone, or each milestone can be mapped to one task.

1. Click  `Save`.
1. (Optional) In a list of tasks, add the `Status Icons` column to identify which tasks have milestones.

   ![](assets/amwt3.png)

1. (Optional) In a list of projects, select the `Milestone` view to identify the progress of your milestone tasks.

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)

