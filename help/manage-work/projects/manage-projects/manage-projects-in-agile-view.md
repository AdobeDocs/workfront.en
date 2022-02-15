---
filename: manage-projects-in-agile-view
product-area: projects;agile-and-teams
navigation-topic: manage-projects
---



# Manage a project in the Agile View {#manage-a-project-in-the-agile-view}

You can leverage agile functionality for your project &nbsp;without the administrative challenges&nbsp;that typically accompany agile practices (such as managing a team backlog, creating iterations, and so forth).


If you want to work in a more pure agile environment that uses&nbsp;a team backlog and allows you to create iterations from tasks on the backlog, follow the instructions in [Work in an agile environment](_work-in-an-agile-environment.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to the following areas:</p> 
    <ul> 
     <li> <p>Projects</p> </li> 
     <li> <p>Reports, Dashboards, Calendars</p> </li> 
     <li> <p>Filters, Views,&nbsp;Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View permissions to the project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Understand Agile projects {#understand-agile-projects}




* [Agile functionality in a project](#agile-functionality-available-in-a-project) 
* [Differences when using the Agile view on a project versus on an iteration](#differen) 




### Agile functionality in a project {#agile-functionality-in-a-project}

The following agile functionality is available when managing a project in an agile view:



* Completion Status  
  For more detailed information about completion status, see [Iteration completion status overview](iteration-completion-status-overview.md).

* Story board  
  For more detailed information about the story board, see the [Scrum board](_scrum-board.md) section.



There are some differences when using agile views on a project versus working in a pure agile environment (with backlogs and iterations). For more information, see [Differences when using the Agile view on a project versus on an iteration](#differen) in this article.


### Differences when using the Agile view&nbsp;on&nbsp;a project versus on an iteration {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}




* [Tasks and subtasks follow different display rules on the Story Board](#tasks-and-subtasks-are-displayed-in-a-more-consistent-way) 
* [Backlogs and iterations are not used](#backlogs-and-iterations-are-not-used) 
* [Task order is maintained in the Agile view and cannot be reordered](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered) 
* [Tasks are measured only in Planned Hours](#tasks-are-measured-only-in-hours) 
* [The Agile Team is not used](#the-agile-team-is-not-used) 
* [Each user on the project can view the project in a different Agile view](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view) 




#### `Tasks and subtasks follow different display rules on the Story Board`  {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}




* Tasks that have neither a parent task nor a subtask are always displayed as a single story card on the story board.   
  For example, these tasks appear as follows in the project list view:   
  
  ![Agile project list - tasks with no parent or subtasks](assets/agile-project-single-list-nwe.png) These tasks appear as follows in the project agile view:   
  
  ![Project agile view - tasks with no parent or subtasks](assets/agile-project-singlecard-nwe.png)


* Parent tasks that have subtasks are always displayed in the `Stories` column of the story board. Subtasks are displayed in the swimlane of the parent task.   
  For example, these tasks appear as follows in the project list view:   
  
  ![Agile project list - tasks with parents and subtasks](assets/agile-project-parent-list-nwe.png)  
  These tasks appear as follows in the project agile view:   
  
  ![Agile project view - tasks with parents and subtasks](assets/agile-project-parent-nwe.png)


* Second-level subtasks (subtasks of subtasks) are displayed as a hanging gray card off the immediate parent task.
* Third-level subtasks (subtasks of subtasks of subtasks) are never displayed on the story board.




#### `Backlogs and iterations are not used`  {#backlogs-and-iterations-are-not-used}

When viewing a project in an agile view, the following agile components are not used:



* `Backlog:` No backlog is used because any tasks in the project are automatically displayed as stories.
* `Iterations:` Rather than creating iterations to define the dates when work will be accomplished, the days currently designated on the project timeline become the working days.




#### `Task order is maintained in the Agile view and cannot be reordered`  {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

The order in which&nbsp;tasks appear in a project is maintained when you view the project in an agile story board.


You cannot reaorder tasks in the project when viewing the project in an agile view. Because modifying the task order can&nbsp;affect other tasks that might have dependencies, you must view the project in a standard&nbsp;view in order to modify task order.


#### `Tasks are measured only in Planned Hours`  {#tasks-are-measured-only-in-planned-hours}

Tasks on a project are always measured in Planned Hours.


In an iteration, tasks (stories) can be measured in hours or points.


#### `The Agile Team is not used`  {#the-agile-team-is-not-used}

Because agile teams complete the work on iterations that are assigned to them, agile teams are not used when viewing a project in an agile view.


Instead, any users on the project essentially become&nbsp;the agile team for that project.


#### `Each user on the project can view the project in a different Agile view`  {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Unlike an agile iteration, users on a project can customize the agile view for themselves, while other users use a different agile view.


In an agile iteration, the information that is available on the agile story board (such as status columns that are available) is determined on the team level.


For information about how to customize an agile view, see&nbsp; [Views overview in Adobe Workfront](views-overview.md#customizing-an-agile-view) in&nbsp; [Views overview in Adobe Workfront](views-overview.md).&nbsp;


## View a project in the Agile view {#view-a-project-in-the-agile-view}




1. Go to the project you want to view in an agile view.
1. Click the `Agile` icon.  
   ![Agile icon](assets/agile-icon-nwe.png)  
   The project is displayed in the default agile view.   
   If you previously viewed the project in a custom agile view, the project is displayed in that&nbsp;view rather than in the default agile view.  

1. (Optional) If you have&nbsp;created a custom&nbsp;agile view, or if another user has created a custom&nbsp;agile view and shared it with you, you can view&nbsp;it instead of the default agile view.   
   Click the `View` drop-down menu, then click&nbsp;the custom agile view you want to view.  
  
   The custom agile view is used the next time you click the `Agile` icon.  
   For information about how to create a new agile view, see [Create and customize Agile views](#creating-a-new-agile-view).  
   The project is displayed in the custom&nbsp;agile view.

1. (Conditional) If tasks in your project are using statuses other than "New," "In Progress," or "Complete" (the default statuses for the Agile view), you must add the additional statuses to the agile view for any tasks in those statuses to be displayed.  
   If tasks are in a status that is not displayed on the agile story board, the task itself is not displayed on the agile story board&nbsp;(however,&nbsp;the Percent Complete of these tasks still&nbsp;contribute to the Percent Complete of any parent tasks and the Percent Complete of the overall project).  
   To add statuses to the agile view, either create a new agile view or customize an existing agile view, as described in&nbsp;the "Create or customize an Agile view" section in&nbsp;the article [Views overview in Adobe Workfront](views-overview.md).

1. (Optional) To return to the list view, click the `List` icon.  
   ![](assets/list-icon.png)






## Create and customize Agile views {#create-and-customize-agile-views}

As with standard views in *`Workfront`*, you can customize existing agile Views or create new agile Views from scratch. Unlike standard views, you cannot create new agile Views based on existing agile Views.


For more information about creating and customizing agile views, see &nbsp;the "Create or customize an Agile view" section in&nbsp;the article [Views overview in Adobe Workfront](views-overview.md).&nbsp;


## Share an existing Agile view {#share-an-existing-agile-view}

For information about how to share an agile view, see [Share a filter, view, or grouping in Adobe Workfront](share-filter-view-grouping.md).


## Remove an existing Agile view {#remove-an-existing-agile-view}

For information about how to delete a view, see the "Remove a view" section in the article [Views overview in Adobe Workfront](views-overview.md).&nbsp;
