---
title: Create and Customize Priorities
description: You can control the priorities for projects, tasks, and issues in the Setup area of Workfront. Priorities give importance to your projects, tasks, or issues in Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
---
# Create and customize priorities

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Customizing existing priorities

As a Workfront administrator, you can make the following modifications to the default priorities provided in Workfront:

* Rename priorities.
* Reorder the priorities.

  For more information on how to reorder priorities, see [Create a priority for a project task, or issue](#create-a-priority-for-a-project-task-or-issue). 

* Change the default priority.

  For more information on the functionality of changing the default priority, see [Create a priority for a project task, or issue](#create-a-priority-for-a-project-task-or-issue).

* Edit the description for the priorities. 
* Set a color for each priority.

  The color of the priority is used in chart reports, when you group your results by **Priority**.

  For more information on chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Delete priorities.

  When you delete an existing priority, you must select a replacement one.

* Hide priorities.

  For more information on the functionality of hiding priorities, see [Create a priority for a project task, or issue](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >You must have at least one priority in your Workfront account for each object.

The priorities provided by default for each object type (project, task, and issue) are identical:

* None
* Low
* Normal
* High
* Urgent

## Create a priority for a project task, or issue {#create-a-priority-for-a-project-task-or-issue}

In addition to the default priorities provided in Workfront, you can add your own priorities to reflect the needs of your organization.

{{step-1-to-setup}}

1. In the left panel, click **Project Preferences** > **Priorities**.

1. Click the tab for the object type you want to create a priority for (**Project**, **Task**, or **Issue**).
1. Click **Add a New Priority**.
1. Specify the following information for the new priority:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Priority Name</td> 
      <td>Type a name for your priority.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td> <p>When adding a new priority, a number is assigned to it by default. Edit this number, if it does not match your needs.</p> <p>The <strong>Importance</strong> number for each priority must be unique for the object you selected.<br>The number of the priority reflects the importance of the project, task or issue: the highest number corresponds to the highest priority.</p> <p><b>NOTE</b>:  You cannot edit the Importance number, after you save the priority. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Choose a color for your priority.</p> <p>The color of the priority is used in chart reports and Agile Team Settings. For more information on chart reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> <p>For more information on Agile Team Settings, see in .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Default Priority</td> 
      <td> <p>Decide whether this should be a default priority or not, by selecting the radio button.</p> <p>If a priority is designated as the <strong>Default Priority</strong>, it is automatically picked for all the projects, tasks, or issues in Workfront. <strong>Normal</strong> is the default priority for all objects in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Add a description for your priority to explain its function.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hide</td> 
      <td> <p>Select this box if you want to hide the priority.</p><p>When you select the <b>Hide</b> option, the priority does not display anywhere in Workfront and users are not able to choose it for their projects, tasks, and issues.</p> 
      <p><b>IMPORTANT</b>:  We recommend that you hide the priorities that you no longer want to use, rather than deleting them. By hiding them, you still keep all your historic data, of objects that have been completed with this priority, while preventing people from choosing this priority in the future. </p>
      <p>Optionally, you can change the listing order of your priorities by dragging and dropping them in your desired order. This changes the order in which they display for projects, tasks, and issues. This does not change the <b>Importance</b> number. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

For instructions on applying priorities to projects, tasks and issues, see the following articles:

* [Understand and update project priorities](../../../manage-work/projects/planning-a-project/project-priority.md) 
* [Update Task Priority](../../../manage-work/tasks/task-information/task-priority.md) 
* [Update issue Priority](../../../manage-work/issues/issue-information/update-issue-priority.md)
