---
filename: create-report-reporting-activities
product-area: reporting
keywords: change,owner,shared,report,share,run,user,access,rights,entered,last,viewed,date,reporting,activities
navigation-topic: report-usage
title: Create a report on reporting activities
description: When you create a report about reports, you can identify specific report information, which can include if reports are assigned to deactivated users, if reports are set to run with access rights of a deactivated user, if users are accessing a report you plan to delete, and so forth.
---

# Create a report on reporting activities

When you create a report about reports, you can identify specific report information, which can include if reports are assigned to deactivated users, if reports are set to run with access rights of a deactivated user, if users are accessing a report you plan to delete, and so forth.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create the report about existing reports

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Reports</span>, then <span class="bold">New Report</span>.</p> </li> 
 <li value="3">In the <span class="bold">New Report</span> drop-down men, select <span class="bold">Report</span> to create a report on existing reports.</li> 
 <li value="4">In the <span class="bold">Columns (View)</span> tab, add the columns you want in your report.<br>Some of the following fields may be useful:<br>
  <table cellspacing="15">
   <col>
   <col>
   <thead>
    <tr>
     <th>Field</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr>
     <td><span class="bold">Run As User:&nbsp;Name</span></td>
     <td>This is the user specified in the <span class="bold">Run this report with the Access Rights of:</span> field on the report. If this user is deactivated, a report does not display for anyone the report is shared with.</td>
    </tr>
    <tr>
     <td><span class="bold">Shared With</span></td>
     <td>These are all the entities that the report is shared with.</td>
    </tr>
    <tr>
     <td><span class="bold">Entered By</span></td>
     <td>This is the owner of the report.</td>
    </tr>
    <tr>
     <td><span class="bold">Last Viewed Date</span></td>
     <td>This is the date and time the report was last viewed by a user.</td>
    </tr>
   </tbody>
  </table></li> 
 <li value="5"> <p>(Optional) To limit your list of reports to specific deactivated users:</p> 
  <ol> 
   <li value="1">Select the <span class="bold">Filters</span> tab, then click <span class="bold">Add a Filter Rule</span>.</li> 
   <li value="2">Add the filter <span class="bold">Run As User ID</span> > <span class="bold">Equal</span>.</li> 
   <li value="3">Type the name of the deactivated user you want to add to the filter, then click the name when it displays in the list.</li> 
   <li value="4">Repeat Step C until you have selected all deactivated users you want to include in the report.</li> 
  </ol> </li> 
 <li value="6"> <p>(Optional) To limit your list of reports to scheduled reports:</p> 
  <ol> 
   <li value="1">Select the <span class="bold">Filters</span> tab, then click <span class="bold">Add a Filter Rule</span>.</li> 
   <li value="2">Add the filter <span class="bold">Scheduled Report ID</span> > <span class="bold">Is Not Blank</span>.</li> 
  </ol> </li> 
 <li value="7"> <p>Click <span class="bold">Save + Close</span>, then type a name for the report, and click <span class="bold">Save Report</span>.</p> <p>Your report information displays.</p> </li> 
 <li value="8">(Optional) Export this report to Excel and save it on your computer.<br>For information on exporting a report, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Export data</a>.</li> 
</ol>

## Update the reports

After creating your report, you can update your reports as needed.

1. Go to the report you want to update.
1. Depending on the action you want to take, do one of the following:

  * Update the `Run this report with the Access Rights of:` field to an active user: For more information, see [Run and deliver a report with the access rights of another user](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).
  
  * Create a copy of the report: For more information, see [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
  * Delete a report:&nbsp;For more information, see the [Create an exact copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) section of the article [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
  
  * Share a report:&nbsp;For more information, see [Share a report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Conditional) If you copy the original reports, use the information from the report you created in [Create the report about existing reports](#create) to share the new copies with the same entities as the original reports.

