---
filename: create-an-agile-story
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
---



# Create an agile story {#create-an-agile-story}

You can create an agile story on an iteration in various ways. After you create an agile story, you can add subtasks to the story.


When you add a story or subtask in an iteration, the Duration Type is set to Simple and the Task Constraint is set to Fixed Dates, with the dates locked within the iteration. You cannot modify the Duration Type or Task Constraint in an iteration. Also, the task duration must be greater than 0 minutes.


For information about how to manage the story after it is added to the iteration, see [Iterations](_iterations.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage access to the project the story is on</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create an agile story in an iteration {#create-an-agile-story-in-an-iteration}




1.  Go to the agile iteration where you want to create the story:  

    
    
    1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Teams`.
    
    1. (Optional) Click the `Switch team` icon ![Switch team icon](assets/switch-team-icon.png), then either select a new Scrum team from the drop-down menu or search for a team in the search bar.
    
    1. In the left panel, select `Iterations`, then select `All Iteration`.
    1. Click the name of the specific iteration where you want to create a story.
    
    

1. Click the `Work Items` tab then `Stories`.  
   ![Screen_Shot_2018-06-04_at_4.24.17_PM.png](assets/screen-shot-2018-06-04-at-4.24.17-pm-350x164.png)


1.  Click `New Story.`
1. Specify the following information:  

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 196px;">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Story Name:</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for the story.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Description:</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Type a description for the story.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Ready:</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select this option if the story is ready to be added to an iteration. When this option is selected, it indicates&nbsp;to users which stories in the backlog are ready to be added to an iteration.<br>A story can be added to an iteration whether or not it is marked <span class="bold">Ready.</span></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Estimate (points)</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Specify the estimate for the story. If your&nbsp;agile team is configured to estimate stories in points, then by default 1 point equals 8 hours. Estimates are added as Planned Hours on the story.<br>For example, if you estimate a story as 3 points, the default behavior is to add 24 Planned Hours&nbsp;to the story.<br>If a story contains subtasks, remember that the combined&nbsp;estimates for all subtasks determines the estimate of&nbsp;the parent story. For more information, see&nbsp;<a href="add-stories-to-existing-iteration.md" class="MCXref xref">Add stories to an existing iteration</a>.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Parent Project</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Begin typing the name of the project that this story will be associated with.<br>By default, the story color is displayed as the same color as other stories from this project.<br>The status of the project must be set to Current. If the status of the project is anything but Current, it is not displayed in the drop-down menu.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Parent Task</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">After you choose a parent project, you have the option to choose a parent task. When you select a parent task,&nbsp;the story is created as a subtask of the parent task on the project that you selected.<br>Begin&nbsp;typing the name of the parent task for the story, then click it when it appears in the drop-down list.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Custom Forms</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Select any custom forms to add to the story.</td>
  </tr>
 </tbody>
</table>


1. Click `Save Story`.




## Create an agile story in the backlog {#create-an-agile-story-in-the-backlog}

You can create an agile story from the agile backlog, as described in the section [Create new stories on the backlog](manage-the-agile-backlog.md#creating-new-stories) in the article [Manage the agile backlog](manage-the-agile-backlog.md).


## Add a task or issue as an agile story {#add-a-task-or-issue-as-an-agile-story}

You can add an existing task or issue as a story to an iteration. For more information, see [Add stories to an existing iteration](add-stories-to-existing-iteration.md)`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  or  <a href="add-story-from-scrum-board.md" class="MCXref xref">Add stories and issues from the Scrum board</a></MadCap:conditionalText>`.


## Create subtasks to an agile story {#create-subtasks-to-an-agile-story}

You can create a subtask to an agile story by using either of the following methods:



* By using the `Subtasks`&nbsp;tab, as described in [Create subtasks](create-subtasks.md#creating-subtasks) in [Create subtasks](create-subtasks.md).

* Directly from the story board, as described in&nbsp; [Create an iteration](create-an-iteration.md).


