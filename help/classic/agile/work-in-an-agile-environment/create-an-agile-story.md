---
filename: create-an-agile-story
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Create an agile story
description: You can create an agile story on an iteration in various ways. After you create an agile story, you can add subtasks to the story.
---

# Create an agile story

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can create an agile story on an iteration in various ways. After you create an agile story, you can add subtasks to the story.

When you add a story or subtask in an iteration, the Duration Type is set to Simple and the Task Constraint is set to Fixed Dates, with the dates locked within the iteration. You cannot modify the Duration Type or Task Constraint in an iteration. Also, the task duration must be greater than 0 minutes.

For information about how to manage the story after it is added to the iteration, see [Iterations](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the project the story is on</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create an agile story in an iteration

1. Go to the agile iteration where you want to create the story:

   1. Click **People**&nbsp;in the Global Navigation Bar.
   1. Click the **Teams**&nbsp;tab, then use the drop-down menu to&nbsp;select the team whose iterations you want to view.
   1. Click the **Iterations**&nbsp;tab, then click **All Iterations.** 
      By default, iterations are grouped by&nbsp;Current, Future, and Past. 
   
   1. Click the name of the specific iteration where you want to create a story.

1. Click the **Work Items** tab then **Stories**.  
   ![Screen_Shot_2018-06-04_at_4.24.17_PM.png](assets/screen-shot-2018-06-04-at-4.24.17-pm-350x164.png)

1. &nbsp;Click **New Story.**
1. Specify the following information:  

   <table cellspacing="0">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Story Name:</td>
      <td>Type a name for the story.</td>
     </tr>
     <tr>
      <td role="rowheader">Description:</td>
      <td>Type a description for the story.</td>
     </tr>
     <tr>
      <td role="rowheader">Ready:</td>
      <td>Select this option if the story is ready to be added to an iteration. When this option is selected, it indicates&nbsp;to users which stories in the backlog are ready to be added to an iteration.<br>A story can be added to an iteration whether or not it is marked <strong>Ready.</strong></td>
     </tr>
     <tr>
      <td role="rowheader">Estimate (points)</td>
      <td>Specify the estimate for the story. If your&nbsp;agile team is configured to estimate stories in points, then by default 1 point equals 8 hours. Estimates are added as Planned Hours on the story.<br>For example, if you estimate a story as 3 points, the default behavior is to add 24 Planned Hours&nbsp;to the story.<br>If a story contains subtasks, remember that the combined&nbsp;estimates for all subtasks determines the estimate of&nbsp;the parent story. For more information, see&nbsp;<a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Add stories to an existing iteration</a>.</td>
     </tr>
     <tr>
      <td role="rowheader">Parent Project</td>
      <td>Begin typing the name of the project that this story will be associated with.<br>By default, the story color is displayed as the same color as other stories from this project.<br>The status of the project must be set to Current. If the status of the project is anything but Current, it is not displayed in the drop-down menu.</td>
     </tr>
     <tr>
      <td role="rowheader">Parent Task</td>
      <td>After you choose a parent project, you have the option to choose a parent task. When you select a parent task,&nbsp;the story is created as a subtask of the parent task on the project that you selected.<br>Begin&nbsp;typing the name of the parent task for the story, then click it when it appears in the drop-down list.</td>
     </tr>
     <tr>
      <td role="rowheader">Custom Forms</td>
      <td>Select any custom forms to add to the story.</td>
     </tr>
    </tbody>
   </table>

1. Click **Save Story**.

## Create an agile story in the backlog

You can create an agile story from the agile backlog, as described in the section [Create new stories on the backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) in the article [Manage the agile backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Add a task or issue as an agile story

You can add an existing task or issue as a story to an iteration. For more information, see [Add stories to an existing iteration](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Create subtasks to an agile story

You can create a subtask to an agile story by using either of the following methods:

* By using the **Subtasks**&nbsp;tab, as described in [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Directly from the story board, as described in&nbsp; [Create an iteration](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

