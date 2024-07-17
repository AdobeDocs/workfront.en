---
product-area: projects
navigation-topic: manage-tasks
title: Edit tasks
description: You can edit information on tasks that you have created, or that you have Contribute or Manage permissions to.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
---
# Edit tasks

<!--Audited: 07/2024-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a field, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


You can edit information on tasks that you have created, or that you have Contribute or Manage permissions to.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a task to edit the following information in the Task Details area: </p>
     <ul>
     <li>Description</li>
     <li>Status</li>
     </ul>  
      </li> 
     <li> <p>Manage permissions to a task to edit all the information in the Details area and the Edit Task box</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute or higher permissions to the project</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Limitations for editing tasks

There are some limitations that might prevent you from editing tasks.

Consider the following when editing tasks:

* Updating tasks triggers notifications for projects that are a Current status. To avoid confusion for users who are assigned to the tasks, limit editing tasks as much as possible when the project is in the Current status. 
* You cannot edit tasks that are in an Approval Process. You can only log time or update the Status for a task in an approval process.

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* You can edit and add documents to tasks on a project that has a status of Complete, Dead, or is Pending Approval only when your Workfront administrator or a group administrator enabled this functionality in the Project Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md). 

* You can always edit the following information on a task when the project has been marked Complete, Dead, or is in an Approval Process:

   * Log time
   * Edit existing expenses
   * Attach a custom form

* Other users must refresh their pages before they can view the updates you make to a task.

## Edit a task in a list

You can edit task information in a list of tasks, by inline editing fields displayed in the view of the list.

For information about editing tasks in lists, see [Edit tasks in a list](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Edit a task in a list using the Summary

You can edit a task in a list using the Summary panel. For information about editing a task in the Summary panel, see the "Edit a task in the Summary" section in the [Edit tasks in a list](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) article.

## Edit a task in the Edit Task box

You can edit a task using the Edit Task or Task Details areas. The following steps describe editing a task in the Edit Task box.

{{step1-click-main-menu}}

1. Click **Projects**, then click the name of a project to open it.
1. Click **Tasks** in the left panel. 
1. Click the task that you want to edit.
1. (Conditional) To edit limited information about a task, click **Task Details** in the left panel.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Consider editing information in the following areas in the Task Details section:

   * **Overview**

     This area is expanded by default.
   
   * **Custom Forms**

     Names of customs forms display only if there are custom forms attached to the object.
   
   * **Finance**

   >[!NOTE]
   >
   >Depending on how your Workfront administrator or Group administrator modified your Layout Template, the fields in the Task Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   For information about the fields visible in the Task Details section, continue with editing the task in the Edit Task box as described below.

   To edit information in the Details section, do the following:

   1. (Optional) Click the **Collapse All** icon ![](assets/collapse-all-icon.png) in the upper-right corner to collapse all areas. 
   1. (Optional and conditional) When an area is collapsed, click the **right-pointing arrow** ![](assets/right-pointing-arrow.png) next to each area to expand the area you want to edit. 
   1. For more information about editing information in the Task Details tab, see the following articles:

      * [Manage task information in the Task Details Overview area](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md) 
      * [Manage task finances in the Task Details section](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Optional) If there are no custom forms attached to the task, start typing the name of a form in the **Add custom form** field, then select it when it displays in the list, then click **Save Changes**.
   1. (Optional) Click the **Export** icon ![](assets/export.png) to export the Overview and custom forms information to a PDF file, then click **Export**. Select from the following:

      * Select all (displays only when there is at least one custom form attached)
      * Overview
      * The name of one or multiple custom forms

      The PDF file downloads to your computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      For more information, see [Export custom forms and object details](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Conditional) To edit all information about the task, as a user with Manage permissions to the task, click the **More** menu ![](assets/more-icon.png) next to the name of the task, then click **Edit**.

   Or

   From a list of tasks, select a task, then click the **Edit** icon ![](assets/edit-icon.png) at the top of the list.

   The Edit Task box opens.

   >[!IMPORTANT]
   >
   >You must have Manage permissions to the task to see the Edit option.

   All task fields are available in the Edit Task box and are grouped by the areas listed in the left panel.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator or Group administrator modified your Layout Template, the fields in the Task Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Consider specifying information in any of the following sections:

   * [Task Name](#task-name) 
   * [Overview](#overview) 
   * [Assignments](#assignments) 
   * [Custom Forms](#Custom%C2%A0F) 
   * [Finance](#finance) 
   * [Settings](#settings)

   >[!NOTE]
   >
   >Depending on how your Workfront administrator or Group administrator sets up your Layout Template, the fields in the Edit Task box might be rearranged or not display. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Task Name {#task-name}

1. Begin editing your task as described above.
1. Click **Task Name** in the left panel.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Update the name of the task.  

1. Click **Save** or continue with the following sections.

### Overview {#overview}

1. Begin editing your task as described above.
1. Click **Overview** in the left panel.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Update the following information about the task: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Add additional information about the task. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Basic information section</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Select the status of the task that indicates what stage of development the task is in.</p> <p><b>TIP</b> 
      
      You can update the task Status in the task header. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priority</td> 
      <td> <p>This is a visual flag for you that allows you to prioritize your tasks. </p> <p>Select from the following options: </p> 
       <ul> 
      <li> <p> None</p> </li> 
      <li> <p> Low </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>High </p> </li> 
      <li> <p> Urgent </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For information about task priorities, see <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Update Task Priority</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Task dates and constraints section</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Task Constraint</td> 
      <td> <p>Decide when the task must be completed by specifying a Task Constraint. </p> <p>Select from the following options: </p> 
       <ul> 
      <li> <p><span>Fixed Dates</span> </p> <p>Specify a <strong>Planned Start</strong> and a <strong>Planned Completion Date</strong>. </p> </li> 
      <li> <p><span>Must Start On</span> </p> <p>Specify a <strong>Planned Start Date</strong>. </p> </li> 
      <li> <p><span>Must Finish On</span> </p> <p>Specify a <strong>Planned Completion Date</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>As Soon as Possible</span></p> </li> 
      <li> <p><span>As Late as Possible</span></p> </li> 
      <li> <p><span>Earliest Available Time</span></p> </li> 
      <li> <p> <span>Latest Available Time</span></p> </li> 
      <li> <p><span>Start No Later Than</span> </p> </li> 
      <li> <p>Specify a Planned Start Date</p> </li> 
      <li> <p><span>Start No Earlier Than</span> </p> <p>Specify a <strong>Planned Start Date</strong>. </p> </li> 
      <li> <p> Finish <span>No Later Than</span></p> <p>Specify a <strong>Planned Completion Date</strong>. </p> </li> 
      <li> <p> Finish <span>No Earlier Than</span></p> <p>Specify a <strong>Planned Completion Date</strong></p> </li> 
       </ul> <p>For more information on Task Constraint, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commit Date and time</td> 
      <td> <p>This is the date by which the user assigned to the task commits to have it completed. This can be different from the Planned Completion Date. Only assignees can edit this field. For information about Commit Dates in Workfront, see <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Start Date and time</td> 
      <td> <p>When the task is planned to start. The planned start date of a task is set and influenced by a number of factors:</p> 
       <ul> 
      <li>Depending on the system-wide preference for the task planned start date, the start date of a new task on a project can either be today, or the start date of the project, by default. <span>The group administrator for the group associated with the project can also set this preference for the group.</span> For more information about the system-level or group-level task preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</li> 
      <li>Depending on the predecessors of the task, the planned start date is picked by Workfront to be the next available date after the predecessors finish, or start, depending on the predecessor relationship. For more information about predecessor relationships, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</li> 
      <li>The project manager or the task owner can manually set the planned start date when the task constraint is either Fixed Dates or Must Start On. For more information about task constraints, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Completion Date and time</td> 
      <td> <p>The anticipated completion date as shown when the task is planned. Workfront sets the Planned Completion Date using some of the following factors:</p> 
       <ul> 
      <li>The planned completion date is calculated from the planned start date by adding the Duration of the task to the planned start date. When the project manager or Workfront specifies the Duration of the task, this triggers an update to the planned completion date. If the planned date changes, it will often be because the Duration of the task has been updated.</li> 
      <li>The project manager or the task owner can manually set the planned completion date when the task constraint is either Fixed Dates or Must Finish On. For more information about task constraints, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</li> 
      <li>If the Duration Type of the task changes, and the number of resources on the tasks changes at the same time, the planned completion date will change, as well. For more information about duration types, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Start Date and time</td> 
      <td> <p>Specify an Actual Start Date for the task. The default is typically populated automatically when you change the status of the task to In Progress. The actual start date can also be manually modified by the project manager, or the task owner. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Completion Date and time</td> 
      <td> <p>Specify the actual date and time when the task completes. The default date and time when a task is completed always coincides with the actual time when the status becomes Completed. The actual completion date can also be manually modified by the project manager, or the task owner. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Working time section</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Work Effort </td> 
      <td> 
       
      <p>The amount of effort required to complete the task. Your project manager might decide to use this field instead of Planned Hours to estimate the effort needed to complete a task. This field is visible only when the following conditions are met:</p> 
      <ul> 
      <li> <p>The task has a Simple Duration Type. </p> <p><b>TIP</b> 
      
      If you change the task Duration Type, this field becomes dimmed. </p> </li> 
      <li>Your project manager has enabled the Use Work Effort to automatically calculate task Planned Hours field on the project. </li> 
      </ul> 
      <p>Select from the following options:</p> 
      <ul> 
      <li>Small</li> 
      <li>Medium <span style="font-weight: normal;">(this is the default value for a new task)</span></li> 
      <li>Large</li> 
      </ul> 
      <p><b>NOTE</b>
        
      Updating the amount of effort could update the task Planned Hours. The update is immediate if the project Update Type is Automatic. When the project Update Type is Manual you must recalculate the timeline to see the updated Planned Hours. </p> 
      
      <p>For information about using Work Effort instead of Planned Hours to estimate task effort, see <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** or continue with the following sections.

### Assignments {#assignments}

1. Begin editing your task as described above.
1. Click **Assignments** in the left panel.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Click **Search people, role and teams** and start typing the name of a user, role, or team that you want to assign to the task, then click it or press Enter when it displays on the list.

   >[!NOTE]
   >
   >If the user's name contains a special character, you must include the special character in the search field.

   >[!TIP]
   >
   >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
   >
   >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: 
   >
   >* Reassign the work item to active resources. 
   >* Associate the users in a deactivated team with an active team and reassign the work item to the active team. 

1. (Optional) Indicate whether an assignee is the primary assignee on the task, by selecting the **Owner** radio button next to their name. A team cannot be the primary assignee of a task. 
1. (Conditional and optional) Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Duration Type</td> 
      <td> <p>This identifies the relationship between the following: </p> 
       <ul> 
      <li> <p>The number of resources assigned to a task </p> </li> 
      <li> <p>The total effort required to complete the task </p> </li> 
      <li> <p> The total duration of the task. </p> </li> 
       </ul> <p>Your Workfront administrator or a group administrator selects the default Duration Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>Duration Types enable you to set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> <p>Select from the following options: </p> 
       <ul> 
      <li> <p>Calculated Assignment </p> </li> 
      <li> <p> Calculated Work </p> </li> 
      <li> <p>Effort Driven </p> </li> 
      <li> <p>Simple</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Duration per Occurrence</td> 
      <td> <p>This displays only on the parent of recurring tasks. It displays the duration of each recurring task, as defined when the task was created. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p> <b>NOTE</b> 
      
      Durations modified in individual recurring tasks do not display the value indicated in this field. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duration</td> 
      <td> 
      <div> 
      <div> 
      <p>This is the amount of time that you allow a task to remain open before it is completed. </p> 
      <p><b>IMPORTANT</b>
      
      Because the task duration is typically the amount of time between the Planned Start and the Planned Completion Dates, it affects the timeline of the project.</p> 
      
      <p>To indicate the Duration of the task and the unit of time do the following:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Type the length of time and select from the units of time available in the drop-down menu.</p> <p><b>TIP</b></p>
      When you update the Duration of tasks in a task list, you can use the abbreviation for the unit of time. </p> </li> 
      </ul> 
      <p> You can choose from the regular time or elapsed time options in the following table: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Unit of Time</td> 
      <td>Abbreviation</td> 
      </tr> 
      <tr> 
      <td>Minutes</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Hours</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Days. This is the default. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>Weeks</td> 
      <td>W</td> 
      </tr> 
      <tr> 
      <td>Months</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>Elapsed Minutes</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Elapsed Hours</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Elapsed Days</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Elapsed Weeks</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Elapsed Months</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table> 

      <p><b>NOTE</b>
         
   <p>Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. 

   Regular time takes into account holidays, weekends, and time off and excludes them from the Duration of the task. For more information about task duration, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Planned Hours</td> 
   <td> <p>Specify the number of Planned Hours for the task, in hours. This is the amount of actual time that it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the Duration Type is set to Calculated Assignment. For more information about duration types, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> 
   <b>NOTE</b>
   <p>
   When creating recurring tasks, the Planned Hours are those of each occurrence. The Planned Hours of the parent tasks are the total of all Planned Hours from all the occurrences. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>.
   </p>
   
   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allocation</td> 
   <td> <p>If your Task Constraint is Calculated Work or Effort Driven, specify the <strong>Allocation %</strong> (allocation percentage) for each assignee. This is the amount of time from the schedule of the assignee that they can spend on this task. Changing the allocation percentage for an assignee will change the Planned Hours of a task. </p> <p>When the Task Constraint is Simple, you can specify the following:</p> 
      <ul> 
      <li> <p>Allocation Hours of each assignee.</p> </li> 
      <li> <p>Planned Hours of the task</p> </li> 
      <li> <p>Duration of the task</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Assignee's Role</td> 
   <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this task. </p> <p><b>TIP</b>
   
    Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
      </tr> 
      </tbody> 
      </table>

1. Click **Save** or continue with the following sections.

### Custom Forms

You can define default custom forms to be automatically attached to tasks when the tasks are added to a project. For information about setting up the project to include default task custom forms for all new tasks, see the "Tasks"section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Begin editing the task as described above.
1. Click **Custom Forms** in the left panel, or click the name of a custom form if it is already attached.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Click **Add custom form** and select the custom form or forms that you want to associate with the task. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list.

   For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can add up to ten custom forms to a task.

1. (Conditional) If you attached a custom form to the task, edit any fields on the form. You must specify all the required fields before you can save the task.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the task itself. For information about setting task permissions, see [Share a task](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Click **Save** or continue with the following sections.

### Finance {#finance}

1. Begin editing your task as described in the [Edit tasks](#Edit2) section in this article.
1. Click **Finance** in the left panel.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cost Type</td> 
      <td> <p>Specify the Cost Type for the task. This is going to determine how the cost of the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options: </p> 
       <ul> 
        <li> <p>No Cost</p> </li> 
        <li> <p>Fixed Hourly </p> </li> 
        <li> <p> User Hourly </p> </li> 
        <li> <p> Role Hourly</p> </li> 
       </ul> <p>For more information about tracking costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a> . Your Workfront administrator or a group administrator selects the default Cost Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenue Type</td> 
      <td> <p>Specify the Revenue Type for the task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options: </p> 
       <ul> 
      <li> <p> Not Billable </p> </li> 
      <li> <p>User Hourly </p> </li> 
      <li> <p>Role Hourly </p> </li> 
      <li> <p>Fixed Hourly </p> </li> 
      <li> <p>User Hourly w/Cap </p> </li> 
      <li> <p>Role Hourly w/Cap </p> </li> 
      <li> <p>User Hourly Plus Fixed </p> </li> 
      <li> <p>Role Hourly Plus Fixed </p> </li> 
      <li> <p>Fixed Revenue </p> </li> 
       </ul> <p>For more information about tracking revenue, see<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a> . </p> <p>Your Workfront administrator or group administrator selects the default Revenue Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** or continue with the following section.

### Settings {#settings}

1. Begin editing your task as described in the [Edit tasks](#Edit2) section in this article. 
1. Click **Settings** in the left panel.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tracking Mode</td> 
      <td> <p>Specify how the progress status of the task is tracked. </p> <p>Select from the following options: </p> 
       <ul> 
      <li> <p> User Must Update </p> </li> 
      <li> <p>Assume on Time </p> </li> 
      <li> <p>Ignore Late Warnings</p> </li> 
      <li> <p> Autocomplete </p> </li> 
      <li> <p>Predecessor </p> </li> 
       </ul> <p>For more information about the Tracking Mode on tasks, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Leveling</td> 
      <td> <p>Select the <strong>Exclude from Resource Leveling</strong> field if you want the resources assigned to the task to be excluded from leveling.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leveling Delay</td> 
      <td> <p>Specify the Leveling Delay in hours. </p> <p> For more information about leveling delays, see <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Update task Leveling Delay</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approval process</td> 
      <td> <p>Select an approval process that you want to associate with the task. Your Workfront administrator must define system-level Approval Processes before you can associate them with tasks. A user with administrative access to Approval processes can also create group-specific approval processes. </p> <p>For more information about creating Approval Processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Create an approval process for work items</a>. Consider the following when adding approval processes: </p> 
       <ul> 
      
      <li> <p>Only active approval processes display in the list. </p> </li> 

      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list. </p> 
        
      <p><b>IMPORTANT</b>  
      
      If the group of the project changes, the group-specific approval process previously attached becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p>
      
      </li> 
        
      <li> <p>You can define default approval processes to be automatically attached to tasks when the tasks are added to a project. For information about setting up the project to include default task approval processes, see the "Tasks" section in the article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>. </p> </li> 
        
      <li> <p>When bulk-editing tasks, the following scenarios exist: </p> 
      <ul> 
      <li> <p>When you select multiple tasks from the same group, both system-level and group-level approval processes display in this field. </p> </li> 
      <li> <p>When you select multiple tasks from different groups, only system-level approval processes display in this field. </p> </li> 
      <li> <p>When any of the tasks have a single-use approval process attached, it is replaced by the system-level or group-level approval process you select. </p> </li> 
         
      </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Click **Save**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Edit a task in the task header (limited)

You can edit a limited amount of information in the task header.

Your system or group administrator can customize the fields you see in the task header. For more information, see [Customize object headers using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

The following fields are included in the task header, by default:

* Task name
* Percent complete
* Assignments
* Planned Completion Date 

  >[!CAUTION]
  >
  >Some Task Constraints and other dependencies might prevent you from editing this field. For information about Task Constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Status
* Make approval decisions if you are set as the approver in a current approval process

## Edit tasks in bulk

You can edit tasks in bulk in a list and update all their information at the same time when you select to automatically save the changes you are making to tasks in the list.

For information about saving tasks in bulk, see the "Edit tasks in bulk" section in the article [Edit tasks in a list](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
