---
product-area: reporting
navigation-topic: reporting-elements
title: Use the Milestone view
description: You can apply the Milestone view to a project list or report.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
---
# Use the Milestone view

<!-- Audited: 1/2024 -->

You can apply the Milestone view to a project list or report.

Before you can use the milestone view, Milestones need to be configured, Milestone Paths need to be added to projects, and Milestones need to be associated with tasks, as described in the articles [Create a milestone path](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) and [Associate milestones with tasks](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

The Milestone view is available when viewing a project list or project report. The following sections describe how to view and use the milestone view.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license</strong></td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or higher access to&nbsp;Reports,&nbsp;Dashboards, Calendars</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View permissions to a project report to apply the Milestone view to a report</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Switch to the Milestone view {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Click the **View** drop-down menu, then click **Milestone**.

   The list or report displays in a Milestone view.

   For information about the milestone view, see the section [Milestone view overview](#milestone-view-overview) in this article.

## Milestone view overview {#milestone-view-overview}

The Milestone view is available on project lists and project reports. This view enables you to quickly view all milestones that are associated with tasks within the projects you are viewing.


>[!NOTE]
>
>The Milestone view is not available in the following areas:
>
>* Timesheets, in the project list when adding a project.


For information about how to switch to the Milestone view, see the section [Switch to the Milestone view](#switch-to-the-milestone-view) in this article.

![Project with milestone view](assets/project-with-milestone-view-with-complete.png)

### Milestone view sections

When applying the Milestone view to a list of projects, the projects display in the following sections:

* The projects that are associated with a Milestone Path display first, listed under the name of their respective Milestone Paths. 

   Workfront sorts the projects in the first section by the following criteria, in this order:

   1. Milestone Path ID. You can view the Milestone Path ID in a Milestone Path report. 
   
   2. The field selected as the first sorting field for the project list in the view previously applied to the project list, before you selected the Milestone view.

* The projects not associated with a Milestobe Path display next, in the Unassigned section. Workfront sorts the projects in the Unassiged section by the field selected as the first sorting field for the project list in the view previously applied to the project list, before you selected the Milestone view.

### Project information in the Milestone view

When viewing a project list or project report in the Milestone view, the following information is available:

* **Planned Dates or Projected Dates:** Specify whether you want to display Planned Dates or Projected Dates in the Milestone view.  
  Dates are displayed for the Start and Completion, as well as for each Milestone within the Milestone Path.  
  If you are viewing Planned Dates and you also have Manage access to the project, you can edit the following dates directly from the Milestone view: (If you are viewing Projected Dates, the dates cannot be edited because Projected Dates are calculated and cannot be manually changed.)

   * **Project Start Dates:** If a project is scheduled from the Start Date, you can manually change the Start Date of the project, and the Completion Date is then calculated.
   * **Project Completion Dates:** If a project is scheduled from the Completion Date, you can manually change the Completion Date of the project, and the Start Date is then calculated.
   * **Task Completion Dates:** You can manually update Completion for tasks directly from the Milestone view.

* **Percent Complete:** Displays the completion percentage of each task and project.  
  You can disable the completion percentage from being displayed, as described in the section [Configure what information displays in the Milestone view](#configure-what-information-displays-in-the-milestone-view) in this article.  
  You can adjust the completion percentage directly from the Milestone view, as described in the section [Adjust Percent Complete for tasks in the Milestone view](#adjust-percent-complete-for-tasks-in-the-milestone-view) in this article.

* **Task status icons:** A status icon is displayed next to each project and task in the Milestone view.

   * On Time  
     ![](assets/gantt-ontime.png)

   * Behind  
     ![](assets/gantt-behind.png)

   * At Risk  
     ![](assets/gantt-atrisk.png)

   * Late  
     ![](assets/gantt-late.png)

  You can disable these status icons from being displayed, as described in the section [Configure what information displays in the Milestone view](#configure-what-information-displays-in-the-milestone-view) in this article.  
  For more detailed information about each status type, see the article [Task Progress Status overview](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Task status shading for completed tasks**: After a task is marked Complete, the background of the task is shaded in the Milestone view to indicate whether the task was completed on time or late:

   * **Red shading for task column**: The background of a task is red when the Progress Status is **Late**.
   
   * **Green shading for task column**: The background of a task is green when the Progress Status is **On Time**.

* **Project status shading for the Project Start and Completion columns**:

   * **Project Start Column**: The background of the Project Start column is red or green only when the Actual Start Date is populated:

      * **Red shading for Project Start column**: The background of the Project Start column is red when the Progress Status of the project is **Late**.
      
      * **Green shading for Project Start column**: The background of the Project Start column is green when the Progress Status of the project is **On Time**.

   * **Project Completion column**: The background of the Project Completion column is red or green only when the Actual Completion Date is populated:

      * **Red Shading for Project Completion column**: The background of the Project Completion column is red when the Progress Status of the project is **Late**.
      
      * **Green shading for the Project Completion column**: The background of the Project Completion column is green when the Progress Status of the project is **On Time**.

   * No color shading is assigned to the Start and Completion columns when the tasks have a Progress Status of At Risk or Behind. 
   
   ![Milestone view with shading](assets/milestone-view-with-shading.png)

* **Project name**: The project name is displayed with a link to the project.
* **Project Condition icon**: An icon is displayed next to the project name, indicating the condition of the project.

## Configure what information displays in the Milestone view {#configure-what-information-displays-in-the-milestone-view}

You can configure whether the following elements are displayed in the Milestone view:

* Progress status icons
* Percent complete of projects and tasks

By default, project status icons and percent complete of projects display.

Any changes you make to these options apply only to you; other users are not affected. The changes you make are retained the next time you log in to Adobe Workfront.

To configure whether project status icons and completion percentage of projects display:

{{step1-to-projects}}

1. Click the **View** drop-down menu, then click **Milestone**.  
   If you are viewing a list of projects inside a Portfolio or a Program, select the **Milestone** subtab.  

1. Click **Options** in the upper-right corner of the Milestone view.  
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. Select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Progress Status</td> 
      <td> <p>Select this option to display progress status icons next to each project and task.</p> <p>This option is enabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percent Complete</td> 
      <td> <p>Select this option to display the completion percentage next to each project and task.</p> <p>This option is enabled by default.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Adjust Percent Complete for tasks in the Milestone view {#adjust-percent-complete-for-tasks-in-the-milestone-view}

You can adjust the Percent Complete for tasks in the Milestone view. You cannot adjust the Percent Complete for a parent task (a task that contains subtasks).

To adjust the percent complete for a task in the Milestone view:

{{step1-to-projects}}

1. Click the **View** drop-down menu, then click **Milestone**.  

1. (Conditional) If completion percentages are not current displaying in the Milestone view, click **Options** in the upper-right corner of the Milestone view, then ensure that **Percent Complete** is enabled.

1. Click the completion percentage below a task, specify a new percentage, then press Enter.
