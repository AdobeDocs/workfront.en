---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: eliminate items in a list by comparing two fields'
description: You can filter items out of a list by comparing two of their fields. For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
---
# Filter: eliminate items in a list by comparing two fields

<!--Audited: 10/2024-->

You can filter items out of a list by comparing two of their fields. For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date.

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

## Filter items by comparing two fields

1. Go to a list of tasks. 
1. From the **Filter** drop-down menu, select **New filter**.

1. Add a filter for **Task:Actual Completion Date** > **Greater Than** > **Select a date**.

   >[!TIP]
   >
   >Choose the filter modifier you want to use for the selected field, if available.

1. Click **Text mode**.
1. In the area displayed, add the following code:

   `
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   `

1. Click **Apply** > **Save as new**.
