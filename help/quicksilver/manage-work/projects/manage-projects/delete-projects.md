---
filename: delete-projects
title: Delete projects
product-area: projects
navigation-topic: manage-projects
title: Delete projects
description: You can delete a project if the project and its data are no longer needed.
---

# Delete projects

You&nbsp;can delete a project if the project and its data are no longer needed.&nbsp;

As an alternative to deleting a project, Adobe Workfront recommends&nbsp;editing the project and changing the status to Complete or Dead. This removes all current tasks related to the project from a user's task list, but saves all data associated with the project.

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project, tasks and issues on the project with ability to Delete the project, tasks, and issues. </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.
You can delete a project in a project list or at the project level.

## Understand the process of deleting projects

* [Limitations for deleting projects](#limitations-for-deleting-projects) 
* [The impact of deleting projects](#the-impact-of-deleting-projects)

### Limitations for deleting projects  {#limitations-for-deleting-projects}

* Deleted items move to the Recycle Bin for 30 days and can be recovered only by the Workfront administrator.

  For more information about restoring objects, see&nbsp;the article [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* ```If the project has tasks or issues with logged hours, the Workfront ```or group administrator``` must allow the deletion of these tasks by configuring the Task & Issue Preferences in your Workfront instance for you to be able to delete the project that contains the tasks.```

  ```For more information about enabling the deletion of tasks, issues``` ```, or projects``` ```where hours are logged, see the "Deletion" section in``` [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### The impact of deleting projects {#the-impact-of-deleting-projects}

* When you delete a project, you impact other objects linked to the project.

  The following objects attached to a project are also deleted when you delete a project:

   * Documents

     You cannot delete a project that has an attached document which has been checked out. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).
   
   * Tasks 
   * Subtasks
   * Issues
   * Notes
   * Approvals
   * Expenses

* Depending on how your Workfront administrator configures the Project, Task, or Issue Deletion Preferences in the Timesheet & Hour Preferences of your Workfront instance, hours logged for the tasks, issues, or the project are handled in one of the following ways when deleting the project:

   * The hours stay on the timesheet as general time. 
   * The hours are deleted and will be restored if the project is ever restored.

  For more information about configuring the deletion preferences for hours logged on issues, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* If the project you delete is linked to an initiative in the Workfront Scenario Planner:

   * The initiative remains on the plan, but the link to the project is removed. 
   * If the project you delete is linked to the only published initiative from a plan, the indication that the plan has been published is also removed. 
   * If you recover a deleted project, the project is recovered, but its link to the initiative is not restored and the Scenario Planner area no longer displays in Project&nbsp;Details.

     The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

     For information about projects linked to initiatives in the Scenario Planner, see [Update or create projects by publishing initiatives in the Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

* If the project is also an activity for a goal in Workfront Goals:

   * The project is deleted from the goal. The progress indicated on the goal by the project is also removed.

   * If you recover the deleted project, the project is also restored as the goal's activity.

     This requires an additional license. For information about Workfront Goals, see [Adobe Workfront Goals overview](../../../workfront-goals/goal-management/wf-goals-overview.md).

     For information about associating projects with goals, see [Overview of connecting projects to goals in Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Delete a project in a list

You can delete projects from a list of projects.

1. Go to a list of projects or a project report.
1. Select the project you want to delete, then click **Delete** at the top of the list.  

1. Click **Yes, Delete It** to confirm the deletion.&nbsp;

   The project is deleted and stored in the Recycle Bin for 30 days. Your Workfront administrator can restore it from the Recycle Bin during this time.

## Delete a project at the project level

1. Go to the project you want to delete. 
1. &nbsp;Click the **More** icon ![](assets/qs-more-menu.png).

1. Click&nbsp;**Delete** **Project****.** 

1. Click **Yes,****Delete it**. &nbsp;

   The project is deleted and stored in the Recycle Bin for 30 days. Your Workfront administrator can restore it from the Recycle Bin during this time.

## Restoring Deleted Projects

A system or group administrator can restore projects&nbsp;within 30 days after they are deleted, as described in the article [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
