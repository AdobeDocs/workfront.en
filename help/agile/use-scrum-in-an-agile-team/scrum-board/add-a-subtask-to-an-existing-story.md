---
filename: add-a-subtask-to-an-existing-story
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
---




# Add a subtask to an existing story on the Scrum board {#add-a-subtask-to-an-existing-story-on-the-scrum-board}

When creating subtasks for existing stories, keep in mind the following:&nbsp;


**When the Completion Mode setting for the project is set to Manual:** 



* Moving a parent story with subtasks to Complete updates the parent story to 100% and the Status to Complete. Subtasks are not updated.
* To&nbsp;update the Percent Complete for the story, you must update it from the Stories tab or from the&nbsp;Details page of the object.


**When the Completion Mode setting for the project is set to Automatic**:&nbsp;



* Moving a parent story with subtasks to Complete updates the parent story to 100% and the Status to Complete. Subtasks are also&nbsp;updated to 100% and the Status is updated to Complete.
* To update the Percent Complete for the story, you must update the Percent Complete for any subtasks. The Percent Complete for the story is calculated based on the Percent Complete of all subtasks.


To add a subtask to an existing story:&nbsp;



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Teams**.

1. Click the **Switch team** icon ![](assets/switch-team-icon.png), then either select a new Scrum team from the drop-down menu or search for a team in the search bar.

1.  In the left panel, select **Iterations**, then select **All Iteration**.
1. Go to the agile iteration or project that contains the story&nbsp;where&nbsp;you want to add a subtask. For information about how to navigate to an iteration, see .
1. Go to the story tile on the story board where you want to add a subtask.
1.  Click **Add Subtask** on the main story card&nbsp;to create a subtask to the story.


   Or


   Click **Add Subtask**&nbsp;on a subtask tile to create a subtask to the subtask.


   `Workfront` supports infinite levels of subtasks, but only two levels (subtasks of subtasks)&nbsp;are displayed on the agile story board.


   When adding a subtask to a story that currently does not have a swimlane, the parent task is promoted to the Stories column and the subtask moves inside&nbsp;the swimlane.

1. Specify the following information:  

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 164px;">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>Subtask Name:</b></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> Specify a name for the subtask.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Description:</b></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Specify a description for the subtask.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>Estimate:</b></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify the estimate for the subtask.<br><p>Keep in mind the following when creating estimates:</p>
    <ul>
     <li value="1">If your&nbsp;agile team is configured to estimate stories in points, then by default 1 point equals 8 hours. Estimates are added as Planned Hours on the story.</li>
     <li value="2">The combined&nbsp;estimates for all subtasks determines the estimate of&nbsp;the parent story. For more information, see <a href="update-status-of-stories-and-subtasks.md" class="MCXref xref">Update the status of stories and subtasks on the Scrum board</a>.</li>
     <li value="3">When you create a new subtask, the Estimate field is already set. If you reset the estimate on the subtask, you are resetting the estimate on the parent story (because the parent story is the sum of all its subtasks).</li>
    </ul><br></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Planned Hours:</b></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> (Available only in projects) Specify the number of planned hours for the task.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray"><b>Assignment:</b></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Begin typing the name of the team where you want to assign the subtask, then click it when it appears in the drop-down list.</td>
  </tr>
 </tbody>
</table>


1. Click **Create**.


