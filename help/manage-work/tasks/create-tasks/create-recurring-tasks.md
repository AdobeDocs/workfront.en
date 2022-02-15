---
filename: create-recurring-tasks
product-area: projects
navigation-topic: create-tasks
---



# Create recurring tasks {#create-recurring-tasks}

You can create recurring tasks for tasks you have to repeat as part of a single project.


For general information about recurring tasks, including the impact of editing an existing recurring task, see [Recurring tasks overview](recurring-tasks-overview.md). 


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information about access to tasks, see <a href="grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="share-a-task.md" class="MCXref xref">Share a task in&nbsp;Adobe Workfront</a>. </p> <p>For information on requesting additional permissions, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a recurring task {#create-a-recurring-task}



>[!NOTE]
>
>You cannot create a recurring task by modifying an existing task. You must create a task from scratch.






1.  Go to the project where you want to create a recurring task, then click the `Tasks` section in the left panel.
1.  Click `New Task.`


   The New Task dialog box displays.


   ![](assets/nwe-create-task-small-screen-350x272.png)



1.  Click `More Options` then enter a name for the task in the `Task Name` field.
1.   Continue updating the task the same way you would if you added a new task. For more information about adding a new task, see [Create tasks in a project](create-tasks-in-project.md)
1.  Click `Overview` in the left panel.
1.  Scroll down to the `Recurrence Schedule` section, then select the `Make this a recurring task` option.


   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)



1.  In the `Frequency` drop-down list, select the number of time units when you want the task to occur and the type of time units.&nbsp;Select from the following options: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 150px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <thead> 
  <tr> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadH-Column1-">Recurrence Type</th> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadG-Column2-">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Day</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The task repeats every day, every 2 days, every 3 days, and so forth, depending on the cadence that you select. You can configure tasks to repeat up to every 6th day. The default setting is 1 Day. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Working Day</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> The task repeats every working day, every 2 working days, every 3 working days, and so forth, depending on the cadence that you select. You can configure tasks to repeat up to every 6th working day.</p> <p>This option uses the default schedule that is defined by the system administrator, as described in <a href="create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Week</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> The task repeats every week, every 2 weeks, every 3 weeks, and so forth, depending on the cadence that you select.</p> <p>In the <span class="bold">Repeats</span> field, select the day of the week when you want each task to occur. You can select multiple days. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Month</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>The task repeats every month, every 2 months, every 3 months, and so forth, depending on the cadence that you select. You can select between 1 and 12 months. </p> <p>In the <span class="bold">Repeats</span> field, select from the following options when you want the task to occur:</p> 
    <ul> 
     <li> <p><span class="bold">every month on day &lt;month date&gt;</span> </p> <p>You can select days from 1 to 30 or you can select <span class="bold">last</span>. For example, you can select "every month on the 30th". </p> </li> 
     <li> <p><span class="bold">every month on the &lt;number&gt; &lt;day of the week&gt;</span> </p> <p>In the first drop-down menu, you can select a number between 1 and 4 for the number of the week in the month, or you can select "last". </p> <p>In the second drop-down menu, you can select any day of the week. </p> <p>For example, you can select "every month on the 2nd Tuesday". </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



   >[!NOTE]
   >
   >If you have a Schedule Exception associated with the project's schedule, recurring tasks can't start during the exception. Recurring tasks that occur during the schedule exception are scheduled to start on the first business day that follows the exception. For more information on schedule exceptions, see the article [Create a schedule](create-schedules.md).



1.  In the `Starts` field, select the date and time when you want the recurring tasks to begin. 
1.  In the `Ends` field, select the date and the time when you want the recurring tasks to complete


   Or


   Select `after <number> occurrences` to indicate how many times the recurring task should occur. *`Workfront`* creates the same number of recurrences for the tasks as the number you indicate in this field. 

1.  Click `Create Task.`


   The task list displays. The recurring task is created as a parent, and all the recurrences are its children. *`Workfront`* auto-generated the names of the children tasks, using the name you entered for the parent followed by a number. For more information about what fields are auto-filled from the parent recurring task, see [Recurring tasks overview](recurring-tasks-overview.md). 


   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)



1.  (Optional) Modify each recurring task as you would any other task in the project.


   For example, you can add assignments, predecessors, `durations,`and modify any other information about the task, including custom fields. 


   >[!IMPORTANT] {type="important"}
   >
   >Modifying the parent recurrence after the children have been modified individually may cause different information between the children or between the children and the parent.&nbsp;For more information, see [Recurring tasks overview](recurring-tasks-overview.md). 





