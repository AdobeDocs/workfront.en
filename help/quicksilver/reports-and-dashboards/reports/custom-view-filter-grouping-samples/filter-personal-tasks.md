---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Personal Tasks'
description: This task filter returns ad hoc work requests sent to a user, or to-do items added by users in their Home area. Personal tasks are not connected to a project but they can be moved to a project, if needed.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
---
# Filter: personal tasks

<!--Audited: 10/2024-->

This task filter returns ad hoc work requests sent to a user, or to-do items added by users in their To-dos widget in the Home area. 

Ad hoc work requests and to-do items are saved in Adobe Workfront as personal tasks. 

Personal tasks are not connected to a project but they can be moved to a project, if needed. For information, see [Create personal tasks](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md). 

![Personal tasks report](assets/personal-tasks-report.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
    <p>New:</p>
   <ul><li><p>Contributor to modify a filter </p></li>
   <li><p>Standard to modify a report</p></li> </ul>

   <p>Current:</p>
   <ul><li><p>Request to modify a filter </p></li>
   <li><p>Plan to modify a report</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Filter personal tasks

To create this filter:

1. Go to a list of tasks or a task report.
1. From the **Filter** drop-down menu, click **New filter**.
1. (Conditional) Click **Add a filter rule** of you are accessing the filter from a report, or start selecting your filter criteria in the first field, if you are accessing the filter from a list.
1. (Conditional) Select the following filtering criteria: 

    * From a list filter: **Task** > **Personal** **Is true**
    * From a report filter: **Task** > **Personal** > **Equal (Case sensitive)** > **True**. 
1. Save the filter. 

    The list displays only personal tasks that are not on any projects.
