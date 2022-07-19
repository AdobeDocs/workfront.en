---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Export data from Adobe Workfront via Kick-Starts
description: As an Adobe Workfront administrator, you can use the Kick-Starts data exporter to export data from Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Export data from Adobe Workfront via Kick-Starts

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

As an Adobe Workfront administrator, you can use the Kick-Starts data exporter to export data from Workfront. You can use it in other applications after you export it.

Exporting data through Kick-Starts is also helpful in understanding what fields are associated with each object, how these fields are coded, as well as how the values of these fields&nbsp;are formatted in the database.

## Access requirements

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Advantages and disadvantages of using kick-starts to export data

There are two ways to export data within Workfront:

* Exporting data from a report or a list

  For more information about exporting data from a report or a list, see [Export data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exporting data via kick-starts

The following table shows the advantages and disadvantages of each method:&nbsp;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>&nbsp;</p> </th> 
   <th> <p>Exported Data Includes Object and Field Values</p> </th> 
   <th> <p>Ability to Export Data around Multiple Object Types Simultaneously</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exporting Data from a List View</strong> </p> <p>For more information about exporting data from a list, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Export data</a></p> </td> 
   <td> <p>Yes</p> <p>Both Workfront native fields and custom fields associated with the objects are exported.</p> </td> 
   <td> <p>No</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exporting Data via Kick-Starts</strong> </p> </td> 
   <td> <p>Yes (limited)</p> <p>Most Workfront native fields associated with objects are exported, but some are not. For example, you cannot export the Schedule, Project Owner, or Project Sponsor fields through a project kick-start export.</p> <p>In a project that has a custom form attached, any data entered in the fields on the form is not exported.</p> <p>But you can export a custom form. The resulting file lists the fields configured in the form, such as text boxes and radio buttons.</p> </td> 
   <td> <p>Yes</p> <p>Using Kick-Starts to export Workfront data&nbsp;enables you to export data related to multiple object types in a single export. For example, you can include tasks, issues, and projects in a single export.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Export limits

The following limitations exist&nbsp;when exporting data via kick-starts (data is exported in an Excel file format):&nbsp;

* **50,000 rows:**&nbsp;The number of rows allowed in the file.
* **65,530 hyperlinks:**&nbsp;This is a limit imposed by Excel on documents that contain more than 65,530 hyperlinks. These documents cannot be opened after they are exported. Note that an Excel document may have just 200 rows of data, but if there are more than 65,530 links inside the document, the document does not open.

## Export data via kick-starts

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **System** > **Kick-Starts,** then click **Export Data.**

1. Select the object&nbsp;you want to export.
1. Click **More Options**&nbsp;to see the full list of objects.

   All&nbsp;of the objects listed here&nbsp;can be&nbsp;used to also import data into Workfront.

   The only exception is the **Access Levels** object. The Access Levels data sheet that is included in an export is provided for reference purposes only. It allows you to assign an access level to a new user account by ID.

   For more information about importing data into Workfront via kick-starts, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)The following is a list of all objects that can be exported through kick-starts:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Object</p> </th> 
      <th> <p>Exported Sheets of the Excel File</p> </th> 
      <th> <p>Export Format</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Access Level</td> 
      <td scope="col" valign="top">Access Level<br>Preferences</td> 
      <td scope="col" valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Assignment</td> 
      <td scope="col" valign="top">Assignment<br>Preferences</td> 
      <td scope="col" valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Company</td> 
      <td scope="col" valign="top"> Company<br>Preferences </td> 
      <td scope="col" valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Email Template</td> 
      <td scope="col" valign="top"> Email Template<br>Preferences </td> 
      <td scope="col" valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Expense</td> 
      <td valign="top"> Expense<br>Preferences </td> 
      <td scope="col" valign="top">&nbsp;Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">External Page</td> 
      <td valign="top"> External Page<br>Preferences </td> 
      <td scope="col" valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Filter</td> 
      <td valign="top"> Filter<br>Preferences </td> 
      <td valign="top">Exports as a .zip file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Group</td> 
      <td valign="top"> Group<br>Preferences&nbsp; </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Grouping</td> 
      <td valign="top"> Grouping<br>Preferences </td> 
      <td valign="top">Exports as a .zip file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Hour</td> 
      <td valign="top"> Hour<br>Preferences </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Issue</td> 
      <td valign="top"> Issue<br>Preferences </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Job Role</td> 
      <td valign="top"> Job role<br>Preferences </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Milestone Path</td> 
      <td valign="top"> Milestone<br>Milestone Path<br>Preferences </td> 
      <td valign="top"> Exports as Excel file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Note</td> 
      <td valign="top"> Note<br>Preferences </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Preferences&nbsp; </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Project</td> 
      <td valign="top"> Queue<br>Project<br>Routing Rule<br>Queue Topic<br>Preferences </td> 
      <td valign="top">&nbsp;Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Resource Estimate</td> 
      <td valign="top"> Resource Estimate<br>Preferences </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Resource Pool</td> 
      <td valign="top"> Resource Pool<br>Preferences </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Risk</td> 
      <td valign="top"> Risk<br>Preferences&nbsp; </td> 
      <td valign="top">Exports as Excel file.</td> 
     </tr> 
     <tr> 
      <td valign="top">Risk Type</td> 
      <td valign="top"> Risk Type<br>Preferences&nbsp; </td> 
      <td valign="top"> Exports as Excel file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">Scorecard Questions<br>Scorecard Option<br>Scorecard<br>Preferences&nbsp;</td> 
      <td valign="top">Exports as Excel file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Task</td> 
      <td valign="top"> Task<br>Preferences </td> 
      <td valign="top">Exports as Excel file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Template</td> 
      <td valign="top"> Queue<br>Template<br>Routing Rule<br>Queue Topic<br>Preferences </td> 
      <td valign="top"> Exports as Excel file.&nbsp;&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Template Assignment</td> 
      <td valign="top"> Template Assignment<br>Preferences </td> 
      <td valign="top">Exports as Excel file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Template Task</td> 
      <td valign="top"> Template Task<br>Preferences </td> 
      <td valign="top">Exports as Excel file.&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">Timesheet</td> 
      <td valign="top"> Timesheet Profile<br>Timesheet<br>Preferences </td> 
      <td valign="top"> Exports as Excel file.&nbsp;&nbsp;</td> 
     </tr> 
     <tr> 
      <td valign="top">&nbsp;View </td> 
      <td valign="top"> View<br>Preferences&nbsp; </td> 
      <td valign="top">Exports as .zip file.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Download.**

   The exported kick-start file is downloaded to your computer either as an Excel file, or a . zip file containing multiple Excel and properties files. Each Excel file is a collection of sheets, where each sheet represents a field associated with the object you selected. There is a **Properties** sheet associated with every export.

   The **Dashboard**&nbsp;and **Report**&nbsp;options allow you to select specific dashboards and reports to include in the download. You can export only&nbsp;Dashboards which are shared system-wide.

   You cannot export matrix reports. For more information about matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   You can select up to 100 Dashboards and 100 Reports in a single export.

   ![](assets/kickstart-export-350x381.png)

   You can export multiple objects at one time.

   By default, the following objects&nbsp;are displayed under the **What to include**&nbsp;label (prior to clicking **More Options**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Object</strong> </p> </th> 
      <th> <p><strong>Exported Sheets of the Excel File</strong> </p> </th> 
      <th> <p>&nbsp;<strong>Export Format</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Portal Tab Section<br>Dashboard<br>Preferences<br></p> </td> 
      <td scope="col" valign="top">&nbsp;Exports as .zip file.</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Report</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
      <td scope="col" valign="top">Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Preferences</td> 
      <td scope="col" valign="top">&nbsp;Exports as .zip file. </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approval</p> </td> 
      <td scope="col" valign="top"> <p>Step Approver<br>Approval Step<br>Approval<br>Approval Process<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Custom Data</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Expense Type</p> </td> 
      <td valign="top"> <p>Expense Type<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Hour Type</p> </td> 
      <td valign="top"> <p>Hour Type<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Team Member<br>Team<br>Preferences </td> 
      <td scope="col" valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>User</p> </td> 
      <td valign="top"> <p>User<br>Preferences</p> </td> 
      <td valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Exported Sheets of the Excel File</strong> </p> </th> 
      <th> <p>&nbsp;<strong>Export Format</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Portal Tab Section<br>Dashboard<br>Preferences<br></p> </td> 
      <td scope="col" valign="top">&nbsp;Exports as .zip file.</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Report</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
      <td scope="col" valign="top">Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Preferences</td> 
      <td scope="col" valign="top">&nbsp;Exports as .zip file. </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approval</p> </td> 
      <td scope="col" valign="top"> <p>Step Approver<br>Approval Step<br>Approval<br>Approval Process<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Custom Data</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Expense Type</p> </td> 
      <td valign="top"> <p>Expense Type<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Hour Type</p> </td> 
      <td valign="top"> <p>Hour Type<br>Preferences</p> </td> 
      <td scope="col" valign="top"> <p>Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Team Member<br>Team<br>Preferences </td> 
      <td scope="col" valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>User</p> </td> 
      <td valign="top"> <p>User<br>Preferences</p> </td> 
      <td valign="top"> <p>&nbsp;Exports as Excel file.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Recommended) Analyze the exported data to ensure that all the information you expect to see was exported.&nbsp;

   For large exports, Workfront works in the background to produce the Excel file and gives you a warning message about the delay. The kick-start file is emailed to you, when the download finishes.

   ![](assets/large-kick-start-file-warning-350x65.png)

