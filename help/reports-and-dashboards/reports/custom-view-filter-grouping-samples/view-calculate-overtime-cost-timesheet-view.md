---
filename: view-calculate-overtime-cost-timesheet-view
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: View: calculate overtime cost in a Timesheet View
description: Overtime is not calculated by default in Adobe Workfront, but you can create a Timesheet report that calculates overtime.
---

# View: calculate overtime cost in a Timesheet View

Overtime is not calculated by default in *Adobe Workfront*, but you can create a Timesheet report that calculates overtime.

If the user is associated with a Cost per Hour rate in their profile, you can also calculate the amount of cost for the overtime of that user.  
For information about associating users with Cost per Hour rates, see the article [Configure My Settings](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>The Overtime field that you can add to a Timesheet view in a list or a report displays the information found in the Overtime field of the timesheet. This information is updated manually by a user with access to modify the timesheet. For more information about the Overtime field in a timesheet, see the article [Understand the Timesheet layout](../../../timesheets/timesheets/timesheet-layout.md).

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

## Calculate overtime cost in a Timesheet View

To add a calculated Overtime column to a timesheet view:

<ol> 
 <li value="1"> <p>Go to a list of timesheets, or create a Timesheet Report.</p> <p>For information about creating reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Customize View</span> in a list of timesheets.</p> <p>Or</p> <p>Select the <span class="bold">Columns (View)</span> tab in a Timesheet report.</p> </li> 
 <li value="3"> <p>Click <span class="bold">Add Column</span>.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Switch to Text Mode</span>.</p> </li> 
 <li value="5"> <p>In the <span class="bold">Show in this column</span> area, click <span class="bold">Click to edit text</span>.</p> </li> 
 <li value="6"> <p>Copy and paste the following text mode code in the <span class="bold">Text mode</span> dialog box.</p><pre>displayname=Calculated Overtime Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre> <note type="note">
    This calculation assumes that the user usually works a 40-hour week.
  </note> </li> 
 <li value="7"> <p>Click <span class="bold">Save</span>, then name the new view and click <span class="bold">Save View</span> in a list of timesheets.</p> <p>Or</p> <p>Click <span class="bold">Save + Close</span> in a Timesheet report.</p> </li> 
 <li value="8"> <p>(Optional and conditional) if you are building a Timesheet report, specify a name for the report, then click <span class="bold">Save Report</span>.</p> <p>The cost of the overtime of each user is displayed in the <span class="bold">Calculated Overtime Cost</span> column.</p> <img src="assets/calculated-overtime-cost-in-timesheet-report-350x92.png" alt="calculated_overtime_cost_in_timesheet_report.png" style="width: 350;height: 92;"> </li> 
</ol>

