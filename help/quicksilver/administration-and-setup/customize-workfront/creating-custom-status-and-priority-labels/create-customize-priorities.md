---
title: Create and Customize Priorities
description: You can control the priorities for projects, tasks, and issues in the Setup area of Workfront. Priorities give importance to your projects, tasks, or issues in Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
---
# Create and customize priorities

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

You can control the priorities for projects, tasks, and issues in the Setup area of Workfront. Priorities give importance to your projects, tasks, or issues in Adobe Workfront.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
     <p>New: Standard</p>
     <p>or</p>
     <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Customizing existing priorities

As a Workfront administrator, you can make the following modifications to the default priorities provided in Workfront:

* Rename priorities.
* Reorder the priorities.

  For more information on how to reorder priorities, see [Create a priority for a project, task, or issue](#create-a-priority-for-a-project-task-or-issue). 

* Change the default priority.

  For more information on the functionality of changing the default priority, see [Create a priority for a project, task, or issue](#create-a-priority-for-a-project-task-or-issue).

* Edit the description for the priorities. 
* Set a color for each priority.

  The color of the priority is used in chart reports, when you group your results by **Priority**.

  For more information on chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Delete priorities.

  When you delete an existing priority, you must select a replacement one.

* Hide priorities.

  For more information on the functionality of hiding priorities, see [Create a priority for a project, task, or issue](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >You must have at least one priority in your Workfront account for each object.

The priorities provided by default for each object type (project, task, and issue) are identical:

* None
* Low
* Normal
* High
* Urgent

## Create a priority for a project, task, or issue {#create-a-priority-for-a-project-task-or-issue}

In addition to the default priorities provided in Workfront, you can add your own priorities to reflect the needs of your organization.

{{step-1-to-setup}}

1. In the left panel, click **Project Preferences** > **Priorities**.

1. Click the tab for the object type you want to create a priority for (**Project**, **Task**, or **Issue**).
1. Click <span class="preview">**New row** at the bottom of the table</span>, or **Add a New Priority**.
1. Configure the following options for the priority:

   * **Priority Name**: Type a name for the priority.
   * **Importance**: When adding a new priority, a number is assigned to it by default. Edit this number, if it does not match your needs.
     
     The Importance number for each priority must be unique. The number of the priority reflects the importance of the project, task or issue: the highest number corresponds to the highest priority.

     You cannot edit this number after you save the priority.
   
   * **Color**: Choose a color for the priority.

     The color of the priority is used in chart reports and Agile Team Settings. For information on chart reports, see [Add a chart to a report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). For information on Agile Team Settings, see [Create an agile team](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Default Priority**: Select the priority you want Workfront to apply automatically to all newly created projects, tasks, or issues.

     **Normal** is the default priority for all objects in Workfront.

     You cannot make a hidden priority the default.

     <div class="preview">

     The default priority is indicated with an icon ![Default priority icon](assets/default-icon.png). To choose a new default, do one of the following:

       * Select the check box next to the priority name and select **Make Default** in the action bar at the bottom of the screen.
       * Hover over the priority name and click the **More** menu that appears. Then, select **Make Default**.

         The new default priority is labeled with the icon.

     </div>

   * **Description**: Type a description for the priority to explain its function.
   * <span class="preview">**Hide Choice**</span> or **Hide**: <span class="preview">Select **Yes**</span> or select the check box to hide a priority that is no longer needed.

     A hidden priority does not display anywhere in Workfront, so users can't choose it for their projects, tasks, or issues.

     >[!IMPORTANT]
     >
     >Instead of deleting priorities that you no longer want to use, we suggest that you hide them. This way, you keep all your historic data on objects already completed with the priority, while preventing people from using the priority in the future.

1. (Optional) Change the listing order of your priorities by dragging and dropping them in the order you want.

   This changes the order in which they display for projects, tasks, or issues. It does not change the **Importance** number.

1. Click **Save**.

For instructions on applying priorities to projects, tasks and issues, see the following articles:

* [Understand and update project priorities](../../../manage-work/projects/planning-a-project/project-priority.md) 
* [Update Task Priority](../../../manage-work/tasks/task-information/task-priority.md) 
* [Update issue Priority](../../../manage-work/issues/issue-information/update-issue-priority.md)
