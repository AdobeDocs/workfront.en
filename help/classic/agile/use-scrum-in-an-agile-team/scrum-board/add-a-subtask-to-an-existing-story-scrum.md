---
filename: add-a-subtask-to-an-existing-story-scrum
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Add a subtask to an existing story on the Scrum board
description: When creating subtasks for existing stories, keep in mind the following:
---

# Add a subtask to an existing story on the Scrum board

When creating subtasks for existing stories, keep in mind the following:

**When the Completion Mode setting for the project is set to Manual:**

* Moving a parent story with subtasks to Complete updates the parent story to 100% and the Status to Complete. Subtasks are not updated.
* To&nbsp;update the Percent Complete for the story, you must update it from the Stories tab or from the&nbsp;Details page of the object.

**When the Completion Mode setting for the project is set to Automatic**:&nbsp;

* Moving a parent story with subtasks to Complete updates the parent story to 100% and the Status to Complete. Subtasks are also&nbsp;updated to 100% and the Status is updated to Complete.
* To update the Percent Complete for the story, you must update the Percent Complete for any subtasks. The Percent Complete for the story is calculated based on the Percent Complete of all subtasks.

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
   <td> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or Manage access to the task the subtask is on</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add a subtask to an existing story on the Scrum board

1. Go to the agile iteration or project that contains the story&nbsp;where&nbsp;you want to add a subtask. For information about how to navigate to an iteration, see [View an iteration](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Go to the story tile on the story board where you want to add a subtask.
1. Click **Add Subtask** on the main story card&nbsp;to create a subtask to the story.

   ![agile_story_addsubtask.png](assets/agile-story-addsubtask-350x212.png)

   Or

   Click **Add Subtask**&nbsp;on a subtask tile to create a subtask to the subtask.

   Workfront supports infinite levels of subtasks, but only two levels (subtasks of subtasks)&nbsp;are displayed on the agile story board.

   ![agile_story_addsubtask2.png](assets/agile-story-addsubtask2-350x212.png)

   When adding a subtask to a story that currently does not have a swimlane, the parent task is promoted to the Stories column and the subtask moves inside&nbsp;the swimlane.

1. Specify the following information:  

   <table cellspacing="0">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Subtask Name:</strong></td>
      <td> Specify a name for the subtask.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description:</strong></td>
      <td>Specify a description for the subtask.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Estimate:</strong></td>
      <td>Specify the estimate for the subtask.<br><p>Keep in mind the following when creating estimates:</p>
       <ul>
        <li>If your&nbsp;agile team is configured to estimate stories in points, then by default 1 point equals 8 hours. Estimates are added as Planned Hours on the story.</li>
        <li>The combined&nbsp;estimates for all subtasks determines the estimate of&nbsp;the parent story. For more information, see <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Update the status of stories and subtasks on the Scrum board</a>.</li>
        <li>When you create a new subtask, the Estimate field is already set. If you reset the estimate on the subtask, you are resetting the estimate on the parent story (because the parent story is the sum of all its subtasks).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Planned Hours:</strong></td>
      <td> (Available only in projects) Specify the number of planned hours for the task.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Assignment:</strong></td>
      <td>Begin typing the name of the team where you want to assign the subtask, then click it when it appears in the drop-down list.</td>
     </tr>
    </tbody>
   </table>

1. Click **Create**.

