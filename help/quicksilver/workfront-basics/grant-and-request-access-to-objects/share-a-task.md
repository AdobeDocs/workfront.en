---
title: Share a task
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Your Adobe Workfront administrator can grant you access to view or edit tasks when they assign access levels. For more information about granting access to tasks, see Grant access to tasks.
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
---
# Share a task

Your Adobe Workfront administrator can grant you access to view or edit tasks when they assign access levels. For more information about granting access to tasks, see [Grant access to tasks](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Along with the access level that users are granted, you can also grant them permissions to View, Contribute, or Manage specific tasks that you have access to share.

Permissions are specific to one item in Workfront and define what actions one can take on that item.


## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following to share objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p> 
   Or
   <p>Current: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View access or higher to the objects you want to share</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p></td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Considerations when sharing a task

In addition to the considerations below, also see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* The creator of a task has Manage permissions for it by default.
* You can share tasks individually, or you can share several of them at a time, in bulk.  
  Sharing tasks is identical to sharing other objects. For more information about sharing items in Workfront, see [Share an object](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md). 

* You can grant the following permissions to a task:&nbsp;

   * View
   * Manage
   * Contribute  
* When you share a task, users inherit the same permissions on all the children objects associated with the task by default. For example, they inherit the same permissions on the children tasks, issues, and documents attached to the task.   
  For more information about the hierarchy of objects in Workfront, see&nbsp; [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  The Workfront administrator can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* You can remove inherited permissions from a task.  
  For more information about removing inherited permissions from objects, see&nbsp; [Remove permissions from objects](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Ways to share a task

You can share a task in the following ways:

* Manually, either individually or in bulk. 

* Automatically, by doing the following:

   * Specify the permissions on any of the parent objects of the task: project, program, or portfolio. Tasks inherit the permissions from their parent objects. For information about viewing inherited permissions on objects, see [View inherited permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md). 
   * Add entities to Project Sharing on a template used to create the project the task is on. For information about sharing projects from templates, see [Share a template](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Specify the permissions on all tasks in a project when you edit the project.&nbsp;For information about managing the access to tasks on the project based on a user's permissions to the project, see the [](../../manage-work/projects/manage-projects/edit-projects.md#access) section in the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >If you don't specify what task permissions you want users to have when they are assigned to the tasks on the project, they receive the same permissions they have on the project by default.

## Share a task

1. Navigate to the task you want to share.

1. To the right of the task name, click **Share**. The **Share [Task Name]** dialog box opens.

    ![Share task button](assets/share-task-button.png)

1. In the **Grant task access to** field, begin typing the name of the user, team, role, group, or company you want to share the task with, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >You can only share a task with active users, teams, roles, or companies.


1. (Optional) Select the **Who has access** drop-down and select the task's access level:

   * **Only invited people can access:** Only users who are invited to the task can access it (Default).
   * **Everyone in the system can view**: All users in the system can view the task without an invitation.

1. Click the drop-down to the right of the user's name and select their permission level for this task:

   * **View**: User can review and share the task. 
   * **Contribute**: User can make updates, log information, make minor edits, and share the task (also includes all View permissions).
   * **Manage**: User has full access to the task without administrative rights, which are granted at the access level (also includes all View and Contribute permissions).

1. (Optional) Click the advanced options icon next to the permission level you've granted to configure specific permissions on the task.

    ![Configured advanced permission options](assets/advanced-permission-options.png)

1. (Optional) To turn off inherited permissions for the task's children objects, click **Turn off** inline with **Inherited permissions**. 

1. (Optional) To quickly share the task using a link, click **Copy link** and then forward it to the recipient.

1. Click **Save**.


## Share tasks in bulk 

1. Navigate to the project that contains the tasks you want to share. 

1. In the **Tasks** tab on the project page, select the box to the left of each task you want to share, then click the **Share** icon ![Share icon](assets/share-icon.png) at the top of the page. The share modal opens.

    ![Bulk share tasks](assets/bulk-share-tasks.png)

1. In the **Grant task access to** field, begin typing the name of the user, team, role, group, or company you want to share the tasks with, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >You can only share tasks with active users, teams, roles, or companies.


1. (Optional) Select the **Who has access** drop-down and select the tasks' access level:

   * **Only invited people can access:** Only users who are invited to the tasks can access them (Default).
   * **Everyone in the system can view**: All users in the system can view the tasks without an invitation.


1. Click the drop-down to the right of the user's name and select their permission level for the tasks:

   * **View**: User can review and share the tasks. 
   * **Contribute**: User can make updates, log information, make minor edits, and share the tasks (also includes all View permissions).
   * **Manage**: User has full access to the tasks without administrative rights, which are granted at the access level (also includes all View and Contribute permissions).

1. (Optional) Click the advanced options icon next to the permission level you've granted to configure specific permissions on the tasks.

    ![Configured advanced permission options](assets/advanced-permission-options.png)

1. Click **Save**.

## Task permissions

The following table displays what permissions you can grant users when allowing them to View, Contribute, or Manage a task:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Manage</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>View</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Add Task(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Add Predecessors</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Add Issue(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Delete Task</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>General Task edit<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Change Task Status</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Edit Task Constraint</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">View Task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Add Document(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Copy Task*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Move Task*</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Log Hours</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Modify Planned Dates</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Accept Assignment</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Make an Assignment</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Attach Custom Form</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Edit Custom Fields</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Create an Approval Process</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Approve A Task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Edit Finance*</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">Add/Edit Expenses</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td scope="row">View Finance</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Updates/Comments</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Share</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Share System-wide</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controlled by access level and the permissions on the project.
