---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: View all updates in a Note report
description: To see all the updates that any of the users have entered for an object, you can create a Note report that displays all the updates.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
---
# View all updates in a Note report

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

The Updates area of an object displays a maximum number of 200 updates by default. To see all the updates that any of the users have entered for an object, you can create a Note report that displays all the updates.

>[!NOTE]
>
>You can build a report to view updates on objects in Preview with the Journal entry report. For more information, see [Report on the Updates area with a Journal Entry report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Create a Note report

Creating a report for Notes for any object is identical, regardless of the object.

For example, to create a Note report for all the notes on a project:

{{step1-to-reports}}

1. In the upper-left corner of the page, click **New Report**, then select&nbsp;**Note**.

1. (Optional) Click **(Columns) View**, then **Add Column** to add the **Name** of the **Project** in the view of the report.&nbsp;

1. (Optional) If you are reporting on multiple projects at the same time, click **Groupings**, then **Add Grouping** to group by the **Name** of the **Project**. This ensures that the notes are grouped by their respective projects, making the report easier to read.&nbsp;

1. (Optional) Click **Filters**, then **Add a Filter Rule**.
1. Add a filter for **Note** > **Note Text** > **Is Not Blank**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   If a project field was updated but no note was added at the time of the update, the **Note Text** of the update displays as **(No text added to update)**.


1. (Optional) Add another filter for **Project** > **Name** > **Equals to** and add one or several project names for which you want to view notes. 
1. Click **Save + Close**. All the updates entered on the project by all users with permissions to View the project are displayed in the report.
