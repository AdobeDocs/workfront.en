---
filename: copy-and-duplicate-tasks
product-area: projects
navigation-topic: manage-tasks
---



# Copy and duplicate tasks {#copy-and-duplicate-tasks}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


You can copy a task from a project to another project, or you can duplicate a task within the same project. 


You can copy or duplicate one or several tasks or parent tasks at a time. 


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a task </p> <p>Contribute or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Considerations for copying tasks {#considerations-for-copying-tasks}

You can copy a task in the following areas of the *`Adobe Workfront`* web application: 



*  At the task level, from the `More icon` ![](assets/qs-more-menu-19x7.png) to the left of the task name. 
* In a task list, by right-clicking the name of a task.
* In a task list, by selecting the task (or tasks) and expanding the `More` menu at the top of the task list.
*  In a task list, by selecting a task and expanding the `More` icon ![](assets/more-icon-task-list.png) next to the task name.


  This option is not available when selecting multiple tasks. 



Consider the following when copying a task:



* Issues are not copied with the task.
* Milestones are transferred to the copied task and removed from the original task.




## Copy tasks in a list {#copy-tasks-in-a-list}




1. Go to the project that contains the task or tasks that you want to copy.
1.  Click `Tasks` in the left panel. 
1.  Click the `Plan mode menu` ![](assets/qs-list-mode-or-save-mode-icon-small.png) , then `Autosave`.
1.  Select the task or tasks that you want to copy and do one of the following:

    
    
    *  Click the `More menu ![](assets/qs-more-menu.png)    
    
      ` at the top of the task list, then click `Copy to`. 
    *  Right click the selected tasks, then click `Copy to`.
    *  When selecting one task, click the `More` menu ![](assets/more-icon-task-list.png) next to the task name in the list, then click  `Copy to`. 
    
    
   ![](assets/copy-task-in-list-nwe-350x131.png)




   >[!IMPORTANT] {type="important"}
   >
   >You can copy tasks in a list only when automatically saving your changes. For information about saving options when editing tasks, see [Edit tasks in a list](edit-tasks-in-a-list.md).



1.  Continue with copying the task, as described in the sections [Copy a task in the Production environment](#move) or ` [Copy a task in the Preview environment](#move2)` starting with Step 4 of each section.


&nbsp;



## Copy a task&nbsp;at the task level {#copy-a-task-at-the-task-level}

In addition to copying tasks in a list of tasks, you can also copy a task after you have opened it.&nbsp;

Copying a task differs depending on what environment you use to move a task. 



*  [Copy a task in the Production environment](#move) 
*  [Copy a task in the Preview environment](#move2) 




### Copy a task in the Production environment {#copy-a-task-in-the-production-environment}




1. Find a task in your *`Workfront`* system by searching for it.
1. Click the name of the task to open it.&nbsp;
1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">More</span> drop-down menu  <img src="assets/qs-more-menu.png"> next to the name of the task, then click  <span class="bold">Copy </span> <span class="bold">to</span>.</MadCap:conditionalText>` 


   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)




   The Copy Task box displays. 


   ![copy_task.png](assets/copy-task-350x191.png)



1.  (Optional) Update the task name. 


   >[!TIP] {type="tip"}
   >
   >This option is not available when selecting more than one task in a list.



1.  Type the name of the `Project`&nbsp;where you want the task copy the task to.&nbsp;


   If you want to copy the task within the same project, type the name of the current project.

1. (Optional) Click  `Next Step`&nbsp;to clear any information that you don't want to transfer to the copied task. Select to clear any of the following options:   

    
    
    * Constraints
    
    
      >[!NOTE]
      >
      >When moving or copying a task with date-specific constraints to another project and the constraint dates of the task are outside the dates of the new project, either the Task&nbsp;Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the projects are adjusted. Some examples of date-specific constraints are Must Start On, Must&nbsp;Finish On, Start No Earlier Than, Start No Later Than, etc. For information about task constraints and how task constraints or project dates can be affected, see [Task Constraint overview](task-constraint-overview.md) and look for a specific constraint.
    
    
    
    * Assignments
    * Approval Processes
    * Progress
    * All Predecessors
    
    
      This is selected by default. 
    
    * Financial information
    * Documents
    
    
      This includes versions, *`proofs`*, and linked documents.&nbsp;
    
    
      This does not include document approvals. Document approvals can never be moved when a task is moved.
    
    * Reminder Notifications
    * Expenses
    * Permissions
    * Custom Data
    
    
      Custom forms 
    
    
    

1. (Optional) Click `Go back a Step` to move to the previous step.
1.  (Optional) Click  `Next Step.`


   Or


   Click `Select Parent` if you want to choose a parent for the tasks that copy to the new project.


   If you do not select a parent task, the tasks are copied as main tasks rather than subtasks and they&nbsp;are placed at the end of the task list on the specified&nbsp;project.&nbsp;

1. (Optional) Select a parent by doing one of the following:  
   In the task list, select one of the parents in the project plan.  
   Or  
   Using the `Search` field, search for a parent task by name. The task should appear in the list.

1. Select the radio button for the parent, after you have found it.&nbsp;
1. (Optional) Click `Go back a Step` to move to the previous step
1.  Click `Finish and Copy Task.`


   The moved&nbsp;task now resides&nbsp;on the specified project and&nbsp;is either a subtask to a parent task, or the last task on the project.






### Copy a task in the Preview environment {#copy-a-task-in-the-preview-environment}




1. Find a task in your *`Workfront`* system by searching for it.
1. Click the name of the task to open it.&nbsp;
1.  Click the `More` drop-down menu ![](assets/qs-more-menu.png) next to the name of the task, then click `Copy` `to`. 


   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)




   The Copy Task box displays. 

1.  (Optional) Update the `Task Name`. 

   ` `**Tip: **`` `This field is dimmed and not editable when selecting to copy multiple tasks in` `a` `list. You can hover over the Task Name field and a list of all selected tasks displays.` 


   ![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)



1.  Type the name of the `Destination Project` where you want to copy the task in the `Select Destination Project` field.&nbsp;


   >[!TIP] {type="tip"}
   >
   >You can also start typing the Reference Number or enter the ID of the project. This might help you distinguish between projects with identical names. 


   The current project name displays by default. If you want to copy the task within the same project, leave this field unchanged. 

1.  (Conditional) Click  `Request Access` to request access to the project, if you don't have access to the selected project. 


   ![](assets/copy-task-request-access-from-project-nwe-350x156.png)




   >[!TIP] {type="tip"}
   >
   >Similar messages display if the project selected is in pending approval or completed or dead, when the *`Workfront administrator`* prevents adding tasks to these projects.&nbsp;For more information, see [Configure system-wide project preferences](set-project-preferences.md).



1.  Click  `Options` in the left panel, then deselect the task attributes that you do not want to copy with the task. All options are selected by default. 


   >[!TIP] {type="tip"}
   >
   >Selecting then deselecting `Select all` deselects all the options. 


   Deselect from the following options to not transfer them to the copied task. The following table describes what happens when the options are deselected: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Constraint</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The task constraint is set to As Soon As Possible or As Late As Possible based on the project Schedule Mode setting.</p> <p> When selected, the current constraint of the task transfers to the copied task. </p> <p>Note: When moving or copying a task with date-specific constraints to another project and the constraint dates of the task are outside the dates of the new project, either the Task&nbsp;Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the projects are adjusted. Some examples of date-specific constraints are Must Start On, Must&nbsp;Finish On, Start No Earlier Than, Start No Later Than, etc. For information about task constraints and how task constraints or project dates can be affected, see <a href="task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a> and look for a specific constraint.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Assignments</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>All the assignments are removed from the task. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Approval Process</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">All approval processes are removed from the task.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Progress</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The task status is New. Otherwise, the copied task keeps the status of the existing task.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Financial Information</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The financial information of the task is removed.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">All&nbsp;Predecessors</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This means that the dependencies will not carry over to the copied tasks. </p> <p>When selected, the predecessors within the group of copied tasks are preserved, others are deleted.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Documents</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The documents attached to the task are not transferred to the copied task. This includes versions, <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span>, and linked documents.</p> <p>This does not include document approvals. Document approvals can never be copied when a task is copied.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Reminder Notifications</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The task reminders do not transfer to the copied task. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Expenses</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The expenses logged on the task do not transfer to the copied task. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> removes the names of all the entities displaying in the Sharing list of the task. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Custom Data</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>The values for the custom fields are cleared and the custom forms are transferred to the copied task. </p> <p>When selected, both the forms and the values for the custom fields transfer to the copied task. </p> </td> 
  </tr> 
 </tbody> 
</table>


1.   (Optional) Click `Select Parent` in the left panel, then select the task in the destination project that you want to become the parent of the copied task. 


   >[!TIP] {type="tip"}
   >
   >`When selecting to copy multiple tasks in a list, all selected tasks become the children of the selected parent.` 


   Select a parent by doing one of the following:

    
    
    *  In the task list, select one of the parents in the project plan.
    *  Click the search icon ![Search icon](assets/search-icon.png) and search for a parent task by name. 
    
    
   The task should appear in the list.


   ![Select parent task when moving a task with search functionality ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)



1.  Select the radio button for the parent, after you have found it.&nbsp;


   If you do not select a parent task, the tasks are copied as main tasks rather than subtasks and they&nbsp;will be placed at the end of the task list on the destination project.&nbsp;

1.  
   Click `Copy Task`


   Or


   Click `Copy Tasks` when you select multiple tasks in a list. 
   The copied tasks are&nbsp;now on the specified project and&nbsp;are either subtasks to the selected parent task, or the last tasks on the project.





## Duplicate tasks {#duplicate-tasks}

You can quickly duplicate a task in a task list, if you need an identical task on the same project. 



*  [Considerations for duplicating tasks](#consider) 
*  [Duplicate tasks](#duplicat) 




### Considerations for duplicating tasks {#considerations-for-duplicating-tasks}




*  You can duplicate a task in a task list only when the list is sorted by task number. 





* The new task will have the same name as the original task.
* You cannot select what information is duplicated to the new task. Almost all the information from the original task will be transferred to the duplicated task, including parent relationship, by default. 
*  The following items are not transferred to the new task:

    
    
    *  Logged hours
    *  Notes
    *  Issues
    *  Only the predecessors which are in the same group of copied tasks are also copied with their successor tasks.
    
    
      ` `**Example: **``For example, if you copy Task 2 and its predecessor, Task 1, at the same time, then you have a copy of Task 2 and a copy of Task 1. The copy of Task 1 will be the predecessor of the copy of Task 2. But if you copy just Task 2 without copying its predecessor, then its copy will have no predecessor. 
    
    
    

* When you duplicate a parent task, all children tasks are also duplicated, even when the children tasks are not selected. 
*  You can duplicate multiple tasks as the same time.


  However, you cannot duplicate multiple tasks that are not sequential at the same time. 

*  Milestones are moved to the new task and removed from the original task.




### Duplicate tasks {#duplicate-tasks-1}




1.  Go to the project that contains the task or tasks that you want to duplicate.
1.  Click `Tasks` in the left panel.
1.  
   Do one of the following:

    
    
    *  `(Conditional) Click the `Plan mode menu` ![](assets/qs-list-mode-or-save-mode-icon-small.png) > `Autosave`, select the tasks you want to duplicate, then click the `More menu` ![](assets/qs-more-menu-29x11.png) > `Duplicate`.` 
    
    
      ![](assets/duplicate-tasks-in-list-nwe-350x196.png)    
    

    
    
    

    
    
    *  ` `(Conditional) Click the `Plan mode menu` ![](assets/qs-list-mode-or-save-mode-icon-small.png) > `Manual save` > `Standard` or `Timeline Planning`, then do the following:`` 
    *  `<li value="1">Select the task or tasks you want to duplicate, and click <span class="bold">Duplicate</span>. </li>` `<li value="2">(Optional) Click <span class="bold">Undo</span> to reverse your changes and not duplicate the tasks.</li>` `<li value="3">(Optional and conditional) Click <span class="bold">Redo</span> if you had previously clicked <span class="bold">Undo</span>, to keep the changes and duplicate the tasks.</li>` `<li value="4">Click <span class="bold">Save</span> to save your changes.</li>` 
    
    
    

    
    
    1. Edit tasks in a list
    
    



