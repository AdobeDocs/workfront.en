---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configure system-wide project preferences
description: As an [!DNL Adobe Workfront] administrator, you can configure the default preferences for all projects created throughout the system. These preferences impact project, task, and issue behavior.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
---
# Configure system-wide project preferences

<!--Audited: 12/2023-->

As an [!DNL Adobe Workfront] administrator, you can configure the default preferences for all projects created throughout the system. These preferences impact project, task, and issue behavior.

>[!NOTE]
>
>By default, these preferences are locked and group administrators cannot modify them at the group level unless you unlock them for all groups throughout the system. For more information, see [Lock or unlock project preferences for all groups in the system](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan</p></td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL System Administrator]</p> <p><b>NOTE</b>:</p><p>If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configure project preferences for the entire organization

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects]**.

1. On the **Project Preferences** page, continue with one of the 4 sections listed below to configure preferences for [!UICONTROL Project Status], [!UICONTROL Timelines], [!UICONTROL Business Cases], and [!UICONTROL Life after Death].
1. If you want all groups throughout the organization to use the same project preferences, ensure that each preference is locked ![](assets/lock-toggle-button.png) (this is the default).

   >[!IMPORTANT]
   >
   >When a project preference is locked, any changes you make to that preference are inherited by all groups in the system. It's important to communicate with the users and groups throughout your organization to ensure that all needs are accounted for in the way you configure project preferences.

   For information about unlocking a preference so that all groups can configure and manage it on their own, see [Lock or unlock project preferences for all groups in the system](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Click **[!UICONTROL Save]**.

* [[!UICONTROL Project Status]](#project-status)
* [[!UICONTROL Timelines]](#timelines)
* [[!UICONTROL Business Cases]](#business-cases)
* [[!UICONTROL Life After Death]](#life-after-death)

### Project Status {#project-status}

Configure any of the following preferences for newly created projects throughout the system:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allow users to create projects without using a template]</td> 
   <td>  <p>This preference allows users to create projects without using a template when creating a project from the following areas: </p>
      <ul>
        <li>
        <p>Use the [!UICONTROL New Project] option in a list of projects</p>
        </li>
          <li>
          <p>Convert an issue to a project from the issue's page</p>
          </li>
         </ul>
        <p>This preference is enabled by default. </p> 
        <p><b>NOTE</b></p>
        <p> A group administrator can change this preference for a group. When a user belongs to multiple groups with different preferences, the user can create a project without a template if their Home Group has this preference enabled.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>Determine the status of new projects.</p>  <p><b>NOTE</b>  
     <ul> 
      <li>If you or another [!DNL Workfront] administrator hides the status selected here, the default status changes to the first status in the status list.</li> 
     </ul> 
     <ul> 
      <li> <p>If a locked system or group status is set as the default status and later someone unlocks it, the system tries to replace it with a locked status of the same status type.</p> <p>If it can't find one, it looks for a required status:</p> 
       <ul> 
        <li>If there is a required status that equates to the unlocked default status, the required status becomes the default status, even if it's unlocked.</li> 
        <li>If none of the required statuses equate to the unlocked default status, the first required status in the status list becomes the default status.</li> 
       </ul> <p>For information about required statuses, see the articles <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Access the list of system project statuses</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Access the list of system task statuses</a>, and <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Access the list of system issue statuses</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>Workfront calculates the percent complete of a project or parent task using the percent complete of each task in the project and either the Duration or the Planned Hours of each task.</p><p>The percent complete of each task is manually set by task assignees.</p><p>You can select here whether Workfront will use the Duration or the Planned Hours of tasks to calculate the percent complete of projects.</p> <p>If you select [!UICONTROL Duration], the Duration of each task in a project determines the overall percent complete for the project, and the Duration of each subtask determines the overall percent complete for its parent task.</p> <p>If you select [!UICONTROL Duration], make sure you specify the [!UICONTROL Typical hours per work day] and [!UICONTROL Typical work days per week] in the [!UICONTROL Timelines] section. [!DNL Workfront] uses this information when calculating a task's percent complete based on Duration. </p> <p>If you select [!UICONTROL Planned Hours], ensure that all tasks on each project have the amount of [!UICONTROL Planned Hours] defined, and that the amount is not zero.</p><p>For more information, see <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Project Percent Complete overview</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>This preference allows users to set the [!UICONTROL Condition] of a project manually to ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) or to have [!DNL Workfront] set the [!UICONTROL Condition] (Progress Status) automatically based on the project's progression on the timeline. For more information about the Condition of projects, see <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Overview of Project Condition and Condition Type</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>This preference automatically creates a baseline (snapshot) of task and project details when the status of the project changes to [!UICONTROL Current]. For information about creating baselines, see <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Create project baselines</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>The Performance Index Method (PIM) for the project controls the method [!DNL Workfront] uses to calculate Earned Value metrics such as [!UICONTROL Cost Performance Index] (CPI) and [!UICONTROL Estimate At Completion] (EAC). For more information, see <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calculate [!UICONTROL Cost Performance Index] (CPI)</a> and <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>: [!DNL Workfront] uses [!UICONTROL Planned Hours] to calculate performance metrics like EAC and CPI. When the PIM is calculated based on hours, the EAC displays as a number of hours. Ensure that you have a value for [!UICONTROL Planned Hours], other than zero.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>: [!DNL Workfront] uses [!UICONTROL Planned Labor Cost] to calculate performance metrics like EAC and CPI. Ensure that your job roles or users are associated with Cost per Hour rates. When the PIM is calculated based on Costs, the EAC displays as a currency value.</p> <p>The project manager can modify this setting at the project level, using the [!UICONTROL Finance] area in [!UICONTROL Project Details]. For more information, see <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Manage information in the project [!UICONTROL Finance] area</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>Determine which data [!DNL Workfront] uses to calculate the [!UICONTROL Estimate at Completion] (EAC) which represents the projected total cost of a project.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calculate at project level]</strong>: EAC for the parent task and project are determined by entering [!UICONTROL Actual Hours] or [!UICONTROL Actual Labor Cost] in the EAC Formulas. This calculation includes [!UICONTROL Actual Hours] or [!UICONTROL Costs and Expenses] added directly to the parent task or project.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>: EAC for the parent task and project are determined by summing up the EAC for each child task. This calculation excludes [!UICONTROL Actual Hours] or [!UICONTROL Actual Costs and Expenses] added directly to the parent task or project.</p> <p>The project manager can modify this setting at the project level, using the [!UICONTROL Finance] area in [!UICONTROL Project Details].For more information, see <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Manage information in the project [!UICONTROL Finance] area</a>.</p> </li> 
    </ul> <p>For more information on how the EAC calculates, see <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculate [!UICONTROL Estimate At Completion] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Timelines {#timelines}

Configure any of the following preferences for newly created projects throughout the system:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>Determine whether new projects are scheduled from Start Date or from Completion Date when they are created.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Date]</strong>: New tasks default to the [!UICONTROL As Soon As Possible] Task Constraint and project managers are prompted to provide a [!UICONTROL Planned Start Date] for the project.</li> 
     <li><strong>[!UICONTROL Completion Date]</strong>: New tasks default to the [!UICONTROL As Late As Possible] Task Constraint and project managers are prompted to provide a [!UICONTROL Planned Completion Date] for the project.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Determine whether the time off of the Primary Assignee of a task adjusts the planned dates for that task on a project.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong>: Any time off scheduled for a task's Primary Assignee adjusts the task's planned dates if the time off occurs during the task's duration. This is the default setting. </p> <p>For example, if a task with a Constraint of [!UICONTROL As Soon As Possible] is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task's planned dates adjust to June 1 through June 4.</p> <p><b>IMPORTANT</b>:</p> <p>The Duration of the task does not change when you select this setting. Only the planned dates change, depending on the Task Constraint.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong>: The planned dates of each task on a project remain as originally planned, even if the Primary Assignee of a task has time off during its duration.</li> 
    </ul> <p>Consider the following when selecting options for this setting:</p> 
    <ul> 
     <li>When you change this setting, only the projects and templates created after the change inherit the updated setting. </li> 
     <li> <p>The Task Constraint value of the task determines which planned task dates to adjust: </p> 
      <ul> 
       <li>The Planned Start Date</li> 
       <li>The Planned Completion Date</li> 
       <li>Both dates</li> 
       <li>Neither date. </li> 
      </ul> <p>For example, if a task has a Constraint of [!UICONTROL Fixed Dates], the dates do not adjust when the Primary Assignee has time off, even if the option [!UICONTROL Consider user time off in task duration] is selected. For information about task constraints, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Task Constraint overview</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Project timelines are automatically re-calculated]</p> </td> 
   <td> <p>Determine when the timeline of a project is recalculated. For information about recalculating the project timeline, see <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculate project timelines</a>.</p> <p>The following options are enabled by default. You can select one or more of the following settings:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>: Select this to recalculate project timelines every night. Any changes you make to the project that might affect the timeline are not immediately visible. [!DNL Workfront​​​] recalculates timelines at night only for projects where both of the following conditions are met:</p> <p> 
       <ul> 
        <li>Have a status of [!UICONTROL Current]</li> 
        <li>Have had an update in the past 3 months</li> 
        <li>Have had an Update Type of one of the following:</li>
        <ul>
        <li>Automatic and On Change</li>
        <li>Change Only</li>
        <li>Automatic Only</li> 
      </ul>       
    <b>TIP:</b>
    <p>Projects that have an Update Type of Manual Only are not affected by this setting.</p>
    <li> <p><strong>When a project's scope changes</strong>: Select this to recalculate project timelines immediately as a project scope change occurs. For information about what constitutes a project scope change, see <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculate project timelines</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>If a project does not have a schedule assigned or if the users assigned to its tasks do not have a Schedule assigned to them, [!DNL Workfront] uses the system default schedule to calculate the timeline of the tasks.</p> <p>If you assign multiple users to the same task in a project and the project has an assigned schedule and the users assigned to the tasks also have a schedule assigned to them, [!UICONTROL Workfront] uses the following schedules:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong>: [!DNL Workfront] uses the schedule of the Primary Assignment on the task to calculate timelines.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] uses the schedule of the project to calculate the timeline of each task.</li> 
    </ul> <p>For more information about schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Create a schedule</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>: Set the number of hours in a typical workday for the users who will be working on projects. The default is 8 hours.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typical work days per week]</strong>: Set the standard workweek for the users who are working on projects. The default is 5 days.</li> 
    </ul> <p>These 2 options convert days to hours, or weeks to days.</p> <p>For example, if you have a task with 8 Planned Hours and the duration is calculated based on Planned Hours, [!DNL Workfront] converts those hours into days in order to show the Duration as days.</p> <p>From the Typical [!UICONTROL work days per week] field, [!DNL Workfront] calculates the Full Time Equivalent (FTE) value for your system. This is what [!DNL Workfront] uses when calculating allocations for users.</p> <p>These values are used when you are planning projects timelines, budgeting for resources, or logging time against projects. </p> <p>They are not used when you are establishing timesheets for users in the system, as described in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] timesheet and hour preferences</a>.</p> <p><b>NOTE</b>:</p> <p>[!DNL Workfront] administrators cannot unlock [!UICONTROL Timeline Calculations] preferences.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>Configure custom yearly quarters for the users who will be working on projects. Custom quarters are usually quarters that do not match the traditional breakdown of quarters during a calendar year. You can add multiple custom quarters. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Enable custom quarters for projects</a>.</p>  <p><b>NOTE</b>: </p><p>[!DNL Workfront] administrators cannot unlock [!UICONTROL Custom Quarters] preferences.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Business Cases] {#business-cases}

You can create a Business Case for newly created projects throughout the system to submit project requests. You can define preferences to determine which areas are visible on the **[!UICONTROL Business Case]** form. We recommend that you enable these options so that other tools, such as the [!UICONTROL Portfolio Optimizer], update properly. For more information about what each field displays, see [Define a Business Case: article index](../../../manage-work/projects/define-a-business-case/define-business-case.md).

After the [!DNL Workfront] administrator enables the sections on the [!UICONTROL Business Case], a Project Owner can then create a Business Case at the project level. For information about creating a Business Case, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Life After Death]  {#life-after-death}

Configure any of the following preferences for newly created projects throughout the system:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>Determine the rules for your organization (or group, if you are configuring project preferences for a group) regarding whether a task or an issue can be deleted after the project status has been marked [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong>: Allows users to delete tasks from a project after the project has been marked [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong>: Allows users to delete issues from a project after the project has been marked [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>Determine the rules for your organization (or group, if you are configuring project preferences for a group) regarding what happens to tasks, issues, documents, and other objects in a project after the project status has been marked <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, or is <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Add and edit tasks]</strong> Allows users to:
      <ul>
       <li>Edit tasks within a project after the project has been marked [!UICONTROL Complete], [!UICONTROL Dead], or is [!UICONTROL Pending Approval]. This includes adding hours and changing expense entries on a task.</li>
       <li>Add tasks to a project.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Add and edit issues]</strong>: Allows users to:
      <ul>
       <li>Edit issues within a project after the project has been marked [!UICONTROL Complete], [!UICONTROL Dead], or [!UICONTROL Pending Approval].</li>
       <li>Add issues to a project after the project has been marked [!UICONTROL Complete] or [!UICONTROL Dead]. (You cannot add issues to a project that is [!UICONTROL Pending Approval].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong>: Allows users to add documents to a project (or to add documents to tasks and issues within the project) after the project has been marked [!UICONTROL Complete] or [!UICONTROL Dead].</p> <p>This option does not apply to projects that are pending approval.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>: Allows users to attach templates to a project after the project has been marked [!UICONTROL Complete] or [!UICONTROL Dead].</p> <p>This option does not apply to projects that are pending approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
