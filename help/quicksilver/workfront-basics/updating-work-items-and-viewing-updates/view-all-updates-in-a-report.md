---
filename: view-all-updates-in-a-report
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: View all updates in a Note report
description: View all updates in a Note report
---

# View all updates in a Note report

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

The Updates area of an object displays a maximum number of 200 updates by default.&nbsp;To see all the updates that any of the users have entered for an object, you can create a Note report that displays all the updates.

>[!NOTE]
>
>You can build a report to view updates on objects in Preview with the Journal entry report. For more information, see [Report on the Updates area](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p> <p>Note: If you do not have View permission or higher to an object, information for that object does not display in the report.</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a Note report

Creating a report for Notes for any object is identical, regardless of the object.

For example, to create a Note report for all the notes on a project:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click&nbsp;**Reports**.
1. Click **New Report**, then choose&nbsp;**Note**.

1. (Optional) Click **Views**, then **Add Column** to add the **Name** of the **Project** in the view of the report.&nbsp;

1. (Optional) Click **Groupings**, then **Add Grouping** to group by the **Project Name**, if you are reporting on multiple projects at the same time.  
   This ensures that the notes are grouped by their respective projects, making the report easier to read.&nbsp;

1. (Optional) Click **Filters,** then&nbsp;**Add a Filter Rule** to filter for just one project, or specific projects.

1. (Conditional and optional) Set the **Project Name** as&nbsp;**Equal** to the project name of the project you want to view updates for.&nbsp;&nbsp;  

1. Click **Save + Close**.  
   All the updates entered on the project by all users with permissions to at least View the project are displayed in the report.

