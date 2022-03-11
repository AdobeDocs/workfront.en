---
filename: create-financial-data-reports-unique-exchange-rates
product-area: reporting
navigation-topic: create-and-manage-reports
title: Create financial data reports with unique exchange rates
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Create financial data reports with unique exchange rates

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

If multiple exchange rates have been configured in Adobe Workfront, you can set financial values in reports and lists to display in a currency other than the default currency.

>[!IMPORTANT]
>
>If you select a currency other than the default currency in a View, you no longer see the links `Add More Tasks` and `Add More Issues` at the bottom of a project list.

For information about how to change the default currency for a given project, see [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md).

If there are projects with a single currency in the report, the sums in groupings are also displayed in the system default currency.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you can view alternate currencies as described in this section, the Workfront administrator must first enable and configure multiple currencies in the Setup area of Workfront. For information, see [Set up exchange rates](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Apply financial values to a report

To convert financial values between currencies when working with reports:

<ol> 
 <li value="1"> <p>Go to the report where you want to convert financial values to a different currency.</p> </li> 
 <li value="2"> <p>Click the <span class="bold">View</span> drop-down list, click <span class="bold">Change Currency</span>, then select one of the following currencies that you want to display financial values in:</p> 
  <ul> 
   <li> <p>Project's Original&nbsp;Currency</p> </li> 
   <li> <p>Any of the other currencies</p> <note type="tip">
     You can choose only currencies previously selected in Setup. 
    </note> </li> 
  </ul> <p>Using this option allows you to quickly convert financial values in a report between rate values.</p> <p>  </p>  <!--
   Tip: You can also select the Change Currency option to convert financial values in other lists.
  --> </li> 
</ol>

## Display the Default Currency across multiple projects with different currencies

When you customize the currency at the project level and you want to display information from all the projects in the same report, the following scenarios exist:

* If you create a report that brings financial information from two or more projects that have different currencies applied, by default the grouping summary reflects the system's default currency as selected by the Workfront administrator.
* If you create a report for two or more projects that have the same currency, but they differ from that of the system's default currency, then the sums in the groupings are displayed using the system default currency.
* If you create a report for two or more projects that have job role assignments associated with an currency override, Workfront converts the financial information from the job role's overridden currency rates to either the currency of the project (when you select Project's Original Currency in the view), or to any different currency you select when viewing the report. For information about overriding the currency of a job role, see [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

To display two projects with custom currencies in a report:

1. Create two projects with different currencies applied.

1. Log hours on both projects.

   For more information about logging time, see [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Click the Main Menu icon , then click Reporting. 
1. Click `New Report`, then `Project Report`.
1. In the `Columns (View)` tab, add an `Actual Cost` column and summarize it by `Sum`.

   For information on how to create a column, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In the `Groupings` tab, apply a `Planned Completion Date` grouping.

   For information on how to create a grouping, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. In the `Filters` tab, add a filter for `Project Name` and select the two projects with the different currencies.

   For information on how to create a filter, see [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Click `Save + Close`.

   The total of the `Actual Cost` is displayed in the Grouping using the system default currency, regardless of the currency of the projects in the report.

   If the two projects have different currencies from one another, the system default currency also displays in the Grouping of the report.

## Display the Project Currency in a report at the project level

If a grouping is applied on a task or hour list within a project, the sums in the grouping are displayed in the project's currency.

<ol> 
 <li value="1"> <p>Create a project with a custom currency, different than the system default currency.</p> </li> 
 <li value="2"> <p>Go to the project and ensure that it includes hours that have been logged for tasks.</p> <p>For more information about logging time, see <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> <note type="note">
    The tasks should be assigned to users or job roles with Rate per Hour cost rates.
  </note> </li> 
 <li value="3"> <p> Click Tasks. </p> </li> 
 <li value="4"> <p>Expand the <span class="bold">View</span> drop-down menu and select <span class="bold">New View</span>.</p> </li> 
 <li value="5"> <p>Add <span class="bold">Actual Cost</span> in the new View as a new column, and summarize it by <span class="bold">Sum</span>.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Done</span>, then click <span class="bold">Save View</span>.</p> </li> 
 <li value="7"> <p>Expand the <span class="bold">Grouping</span> drop-down menu and select <span class="bold">New Grouping</span>.</p> </li> 
 <li value="8"> <p>Add <span class="bold">Actual Completion Date</span> in the new grouping as a new field, then click <span class="bold">Save Grouping</span>.</p> <p>The <span class="bold">Actual Cost</span> column summarizes in the new Grouping and displays the total in the currency of the project.</p> </li> 
</ol>

## Edit reports with unique currencies

The financial fields in a report are not editable until you change the report setting to show the original currency for projects.

To in-line edit a financial field in a report:

<ol> 
 <li value="1"> <p>Navigate to a report.</p> <note type="note">
   If the default currency does not display for a list in any other area, you can edit the View to display the default currency.
   <br>For information on how to change the currency in a View, see the section in this article 
   <a href="#applying-financial-values-to-a-report" class="MCXref xref">Apply financial values to a report</a>.
  </note> </li> 
 <li value="2"> <p>Click <span class="bold">Report Actions</span>, then select <span class="bold">Edit</span>.</p> </li> 
 <li value="3"> <p>Click <span class="bold">Report Settings</span>.</p> </li> 
 <li value="4"> <p>Click the <span class="bold">Default Currency</span> drop-down, then select <span class="bold">Project's Original Currency</span>.</p> <p>  </p> </li> 
 <li value="5"> <p>Click <span class="bold">Done</span>.</p> </li> 
</ol>

