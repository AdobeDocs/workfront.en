---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Create an agile story
description: You can create an agile story on an iteration in various ways. After you create an agile story, you can add subtasks to the story.
author: Lisa
feature: Agile
---

# Create an agile story

You can create an agile story on an iteration in various ways. After you create an agile story, you can add subtasks to the story.

When you add a story or subtask in an iteration, the Duration Type is set to Simple and the Task Constraint is set to Fixed Dates, with the dates locked within the iteration. You cannot modify the Duration Type or Task Constraint in an iteration. Also, the task duration must be greater than 0 minutes.

For information about how to manage the story after it is added to the iteration, see [Iterations](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>Manage access to the project the story is on</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create an agile story in an iteration

1. Go to the agile iteration where you want to create the story:

   1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Teams**.
   
   1. (Optional) Click the **Switch team** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new Scrum team from the drop-down menu or search for a team in the search bar.
   
   1. In the left panel, select **Iterations** to choose a specific iteration, or select **Current Iteration**.
   1. Click the name of the specific iteration where you want to create a story.

   ![Add new story to iteration](assets/iteration-add-story.png)

1. Click **New Story.**
1. Specify the following information:  

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Story Name</strong></td>
      <td>Type a name for the story.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description</strong></td>
      <td>Type a description for the story.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Ready</strong></td>
      <td>Select this option if the story is ready to be added to an iteration. When this option is selected, it indicates&nbsp;to users which stories in the backlog are ready to be added to an iteration.<br>A story can be added to an iteration whether or not it is marked <strong>Ready.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Estimate (points)</strong></td>
      <td>Specify the estimate for the story. If your&nbsp;agile team is configured to estimate stories in points, then by default 1 point equals 8 hours. Estimates are added as Planned Hours on the story.<br>For example, if you estimate a story as 3 points, the default behavior is to add 24 Planned Hours&nbsp;to the story.<br>If a story contains subtasks, remember that the combined&nbsp;estimates for all subtasks determines the estimate of the parent story. For more information, see <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Add stories to an existing iteration</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Parent Project</strong></td>
      <td>Begin typing the name of the project that this story will be associated with.<br>By default, the story color is displayed as the same color as other stories from this project.<br>The status of the project must be set to Current. If the status of the project is anything but Current, it is not displayed in the drop-down menu.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Parent Task</strong></td>
      <td>After you choose a parent project, you have the option to choose a parent task. When you select a parent task,&nbsp;the story is created as a subtask of the parent task on the project that you selected.<br>Begin&nbsp;typing the name of the parent task for the story, then click it when it appears in the drop-down list.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Custom Forms</strong></td>
      <td>Select any custom forms to add to the story.</td>
     </tr>
    </tbody>
   </table>

1. Click **Save Story**.

## Create an agile story in the backlog

You can create an agile story from the agile backlog, as described in the section [Create new stories on the backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) in the article [Manage the agile backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Add a task or issue as an agile story

You can add an existing task or issue as a story to an iteration. For more information, see [Add stories to an existing iteration](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) or [Add stories and issues from the Scrum board](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Create subtasks to an agile story

You can create a subtask to an agile story by using either of the following methods:

* By using the **Subtasks** tab, as described in [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Directly from the story board, as described in [Create an iteration](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

