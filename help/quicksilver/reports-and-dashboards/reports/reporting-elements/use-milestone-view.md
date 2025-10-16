---
product-area: reporting
navigation-topic: reporting-elements
title: Use the Milestone view
description: You can apply the Milestone view to a project list or report. You can use the Milestone view to view all milestones that are associated with tasks within the projects you are viewing.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
---
# Use the Milestone view

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 

You can apply the Milestone view to a project list or report. You can use the Milestone view to view all milestones that are associated with tasks within the projects you are viewing.

Before you can use the milestone view, the following elements must exist:

* Milestones paths are configured. For information, see [Create a milestone path](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* Milestone paths need are added to projects. For information, see [Edit projects](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md). 
* Milestones are associated with tasks. For information, see [Associate milestones with tasks](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

The Milestone view is available when viewing a project list or a project report. The following sections describe how to view and use the milestone view.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Work or higher</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to&nbsp;Reports,&nbsp;Dashboards, Calendars</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
    <td> <p>View permissions to a project report to apply the Milestone view to a report</p></td> 
   </td> 
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

<div class="preview">

The Milestone view is available on project lists and project reports. You can quickly view all milestones that are associated with tasks within the projects you are viewing.

![Project with milestone view](assets/project-with-milestone-view-with-complete.png)

</div>

>[!NOTE]
>
>The Milestone view is not available in the following areas:
>
>* Timesheets, in the project list when adding a project.

For information about how to switch to the Milestone view, see the section [Switch to the Milestone view](#switch-to-the-milestone-view) in this article.


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
  Dates are displayed for the Start and Completion dates of the project, as well as for the Completion of each Milestone task in the Milestone Path. 

   If you are viewing Projected Dates, the dates cannot be edited. Projected Dates are calculated by Workfront and cannot be manually changed.

   If you are viewing Planned Dates and you also have Manage access to the project, you can edit the following dates directly from the Milestone view: 

   * **Project Start Dates:** If a project is scheduled from the Start Date, you can manually change the Planned Start Date of the project, and the Planned Completion Date is then calculated.
   * **Project Completion Dates:** If a project is scheduled from the Planned Completion Date, you can manually change the Planned Completion Date of the project, and the Planned Start Date is then calculated.
   * **Task Completion Dates:** You can manually update the Planned Completion Date for tasks directly from the Milestone view.

* **Percent Complete:** Displays the completion percentage of each task and project.  

  You can disable the completion percentage from being displayed, as described in the section [Configure what information displays in the Milestone view](#configure-what-information-displays-in-the-milestone-view) in this article. 

  You can adjust the completion percentage directly from the Milestone view, as described in the section [Adjust Percent Complete for tasks in the Milestone view](#adjust-percent-complete-for-tasks-in-the-milestone-view) in this article.

* **Task progress status icons:** Depending on what environment you use to view the milestone view, the following are icons that indicate the tasks's progres status: 

   * In the Production environment, the following status icons display next to each project and task in the Milestone view: 

      * On Time  
      ![On time icon](assets/gantt-ontime.png)

      * Behind  
      ![Behind icon](assets/gantt-behind.png)

      * At Risk  
      ![At risk icon](assets/gantt-atrisk.png)

      * Late  
      ![Late icon](assets/gantt-late.png)

      <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

   <div class="preview">

   * In the Preview environment, the following colored circles display next to each project and task in the Milestone view:  

      * On Time - green
      * Behind - yellow
      * At Risk - blue
      * Late - red
   
   </div>

  You can disable these status icons from being displayed, as described in the section [Configure what information displays in the Milestone view](#configure-what-information-displays-in-the-milestone-view) in this article. 

  For more detailed information about each status type, see the article [Task Progress Status overview](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Task status shading for completed tasks**: After a task is marked Complete, the background of the task is shaded in the Milestone view to indicate whether the task was completed on time or late:

   * **Red shading for task column**: The background of a task is red when the Progress Status is **Late**.
   
   * **Green shading for task column**: The background of a task is green when the Progress Status is **On Time**.

* **Project status shading for the Project Start and Completion columns**:

   * **Project Start Column**: The background of the Project Start column is red or green only when the Actual Start Date is populated:

      * **Red shading for Project Start column**: The background of the Project Start column is red when the Progress Status of the project is **Late**.
      
      * **Green shading for Project Start column**: The background of the Project Start column is green when the Progress Status of the project is **On Time**.

      >[!TIP]
      >
      >You must go to the Project Details page to view the Actual Start Date of the project.

   * **Project Completion column**: The background of the Project Completion column is red or green only when the Actual Completion Date is populated:

      * **Red Shading for Project Completion column**: The background of the Project Completion column is red when the Progress Status of the project is **Late**.
      
      * **Green shading for the Project Completion column**: The background of the Project Completion column is green when the Progress Status of the project is **On Time**.

      >[!TIP]
      >
      >You must go to the Project Details page to view the Actual Completion Date of the project.

   * No color shading is assigned to the Start and Completion columns when the tasks have a Progress Status of At Risk or Behind. 

   <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->
   
   ![Milestone view with shading](assets/milestone-view-with-shading.png)

* **Project name**: The project name is displayed with a link to the project.
* **Project Condition icon**: Depending on the environment you are accessing the Milestone view from the following indicators show the project Condition: 

   * In the Production environment, an icon displays next to the project name, indicating the condition of the project. The Condition of the project might be one of the following:

      * On Target
      * At Risk
      * In Trouble

   <div class="preview">

   * In the Preview environment, a condition icon in the shape of a colored circle displays next to each project. The possible project conditions and circle colors are: 

      * On Target - green
      * At Risk - yellow
      * In Trouble - red
   
      </div>
   

## Configure what information displays in the Milestone view {#configure-what-information-displays-in-the-milestone-view}

You can configure whether the following elements are displayed in the Milestone view:

* Progress status icons
* Percent complete of projects and tasks

By default, progress status icons and percent complete of projects and tasks display.

Any changes you make to these options apply only to you; other users are not affected. The changes you make are retained the next time you log in to Workfront.

To configure whether project status icons and completion percentage of projects display:

{{step1-to-projects}}

1. Click the **View** drop-down menu, then click **Milestone**. 

1. In the Production environment, click **Options** in the upper-right corner of the Milestone view, then select from the options in the next step.   

   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

   <div class="preview">In the Preview environment, select from the options in the next step, from the upper-right corner of the Milestone view.</div>

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->
  

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

You can adjust the Percent Complete for tasks in the Milestone view. You cannot adjust the Percent Complete for a parent task (a task that contains subtasks) or for a project.

To adjust the percent complete for a task in the Milestone view:

{{step1-to-projects}}

1. Click the **View** drop-down menu, then click **Milestone**.  

1. (Conditional) If completion percentages are not current displaying in the Milestone view, enable viewing the Percent Complete of tasks and projects, as described in the section [Configure what information displays in the Milestone view](#configure-what-information-displays-in-the-milestone-view) in this article. 

1. In the Production environment, click the completion percentage below a task, specify a new percentage, then press Enter.

   <div class="preview">In the Preview environment, move the Percent Complete slide to the new percent complete to update it. </div>
