---
filename: import-data-via-kickstarts
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Import data into Adobe Workfront via a Kick-Start template
description: Kick-Starts are specially formatted Excel workbooks that you can populate with data you want to import into Workfront. Adobe Workfront provides a Kick-Start template you can use to do this, as explained in Kick-Starts data importer.
---

# Import data into `Adobe Workfront` via a Kick-Start template

Kick-Starts are specially formatted Excel workbooks that you can populate with data you want to import into `Workfront`. `Adobe Workfront` provides a Kick-Start template you can use to do this, as explained in [Kick-Starts data importer](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

This process is broken up into 3 main tasks:

* First, you export a Kick-Start template as a spreadsheet file
* Second, you populate the spreadsheet with your data
* Finally, you import the populated spreadsheet into `Workfront`

Each of these procedures is outlined in the proper order in this article.

>[!IMPORTANT]
>
>If you use `Legacy Workfront Fusion` or `Workfront Fusion`, you must turn off your FLOs or scenarios before you can import data via Kick-Starts.
>
>For information on how to turn off FLOs in `Legacy Workfront Fusion`, see the `Legacy Workfront Fusion` [Getting Started](https://learn.fusion.workfront.com/quickstart-2019/) guide.
>
>For information on how to deactivate scenarios in `Workfront Fusion`, see [Activate or deactivate a scenario](../../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limitations

You can import large numbers of objects into `Workfront` using a Kick-Start template. However, consider the following limitations:

* Importing data this way doesn't update information on records that already exist in `Workfront`
* You can import only new records and their information
* Import no more than 2,000 records at a time to ensure that the import does not time out

## Export a Kick-Start template as a spreadsheet file

When you export a Kick-Start template you receive a blank Excel spreadsheet workbook. In subsequent procedures in this article, you will populate the workbook with your information and then import it back into `Workfront`.

To export a Kick-Start template:

<ol> 
 <li value="1"> <p>(Conditional) If you are using Workfront Fusion, turn off active FLOs or scenarios.</p> <p>For information on how to turn off FLOs in <span>Legacy Workfront Fusion</span>, see the <span>Legacy Workfront Fusion</span> <a href="https://learn.fusion.workfront.com/quickstart-2019/">Getting Started</a> guide. For information on how to deactivate scenarios in <span>Workfront Fusion</span>, see <a href="../../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md" class="MCXref xref">Activate or deactivate a scenario</a>.</p> </li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="3">Click <span class="bold">System</span> > <span class="bold">Export Data (Kick-Starts)</span>.</li> 
 <li value="4"> <p>Click <b>More Options</b>, then select the types of information that you want to include.</p> <p>Each option that you select represents a collection of multiple tabs in the exported spreadsheet. For example, if you select the Report option, all the necessary objects for creating a report will be included in the spreadsheet (views, filters, groupings, reports).</p> <p>You can use all of the object types listed below to import data into <span>Workfront</span>. (The only exception is the Access Levels option. The Access Levels data sheet in an export is provided for reference purposes—it allows you to assign an access level to a new user account by ID.)</p> <p>The template for each of the object types can be exported in the following file formats and contains the following sheets:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th> <p><span class="bold">Object</span> </p> </th> 
     <th> <p><span class="bold">Exports as</span> </p> </th> 
     <th> <p><span class="bold">Sheets in the exported spreadsheet</span> </p> </th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td scope="col"> <p>Dashboard</p> <p>All dashboards in the system are available to export. You can select up to 100 specific dashboards in a single export.</p> </td> 
     <td scope="col">Exports as ZIP file</td> 
     <td scope="col"> <p>Parameter</p> <p>Parameter Option</p> <p>Parameter Group</p> <p>Category Parameter</p> <p>Category</p> <p>Report</p> <p>Portal Tab Section</p> <p>Dashboard</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td scope="col"> <p>Report</p> <p>All reports in the system are available to export. You can select up to 100 specific reports in a single export.</p> </td> 
     <td scope="col">Exports as ZIP file </td> 
     <td scope="col"> <p scope="col">Parameter</p> <p scope="col">Parameter Option</p> <p scope="col">Parameter Group</p> <p scope="col">Category Parameter</p> <p scope="col">Category</p> <p scope="col">Report</p> <p scope="col">Preferences</p> </td> 
    </tr> 
    <tr> 
     <td scope="col"> <p>Approval</p> </td> 
     <td scope="col"> <p>Exports as Excel file</p> </td> 
     <td scope="col"> <p>Step Approver</p> <p>Approval Step</p> <p>Approval</p> <p>Approval Process</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td scope="col"> <p>Custom Data</p> </td> 
     <td scope="col"> <p>Exports as Excel file</p> </td> 
     <td scope="col"> <p>Parameter</p> <p>Parameter Option</p> <p>Parameter Group</p> <p>Category Parameter</p> <p>Category</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td scope="col"> <p>Expense Type</p> </td> 
     <td scope="col"> <p>Exports as Excel file</p> </td> 
     <td> <p>Expense Type</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td> <p>Hour Type</p> </td> 
     <td scope="col"> <p>Exports as Excel file</p> </td> 
     <td> <p>Hour Type</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td> <p>Team</p> </td> 
     <td scope="col"> <p>Exports as Excel file</p> </td> 
     <td> <p> Team Member</p> <p>Team</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td> <p>User</p> </td> 
     <td> <p>Exports as Excel file. To see the full list of options, click <span class="bold">More Options</span>.</p> </td> 
     <td> <p>User</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td>Access Level</td> 
     <td>Exports as Excel file</td> 
     <td> <p>Access Level</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td>Assignment</td> 
     <td>Exports as Excel file</td> 
     <td> <p>Assignment</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td>Company</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Company</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Email Template</td> 
     <td>Exports as Excel file</td> 
     <td> <p>Email Template</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Expense</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Expense'</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>External Page</td> 
     <td>Exports as Excel file</td> 
     <td> <p> External Page</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Filter</td> 
     <td>Exports as a ZIP file</td> 
     <td> <p> Filter</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Group</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Group</p> <p>Preferences&nbsp;</p> </td> 
    </tr> 
    <tr> 
     <td>Grouping</td> 
     <td>Exports as a ZIP file</td> 
     <td> <p> Grouping</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Hour</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Hour</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Issue</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Issue</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Job Role</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Job role</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Milestone Path</td> 
     <td> Exports as Excel file</td> 
     <td> <p> Milestone</p> <p>Milestone Path</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Note</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Note</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Portfolio</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Portfolio</p> <p>Preferences&nbsp;</p> </td> 
    </tr> 
    <tr> 
     <td>Project</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Queue</p> <p>Project</p> <p>Routing Rule</p> <p>Queue Topic</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Resource Estimate</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Resource Estimate</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Resource Pool</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Resource Pool</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Risk</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Risk</p> <p>Preferences&nbsp;</p> </td> 
    </tr> 
    <tr> 
     <td>Risk Type</td> 
     <td> Exports as Excel file</td> 
     <td> <p> Risk Type</p> <p>Preferences</p> </td> 
    </tr> 
    <tr> 
     <td>Scorecard</td> 
     <td>Exports as Excel file</td> 
     <td> <p>Scorecard Questions</p> <p>Scorecard Option</p> <p>Scorecard</p> <p>Preferences&nbsp;</p> </td> 
    </tr> 
    <tr> 
     <td>Task</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Task</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Template</td> 
     <td> Exports as Excel file</td> 
     <td> <p> Queue</p> <p>Template</p> <p>Routing Rule</p> <p>Queue Topic</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Template Assignment</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Template Assignment</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Template Task</td> 
     <td>Exports as Excel file</td> 
     <td> <p> Template Task</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>Timesheet</td> 
     <td> Exports as Excel file</td> 
     <td> <p> Timesheet Profile</p> <p>Timesheet</p> <p>Preferences </p> </td> 
    </tr> 
    <tr> 
     <td>View </td> 
     <td> <p>Exports as ZIP file</p> </td> 
     <td> <p> View</p> <p>Preferences&nbsp;</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <span class="bold">Download</span>.</li> 
 <li value="6">Continue with <a href="#populating-the-excel-template-with-your-data-and-uploading-to-workfront" class="MCXref xref">Populate the spreadsheet template with your data</a> to populate the template with your information.</li> 
</ol>

## Populate the spreadsheet template with your data

* [About the tabs (data sheets) included in the spreadsheet](#about) 
* [Import a record](#importing-a-record) 
* [Include dates](#including-dates) 
* [Use wildcards](#using-wildcards) 
* [Attribute name substitution for IDs](#understanding-attribute-name-substitution)

### About the tabs (data sheets) included in the spreadsheet

>[!TIP]
>
>To better understand how you will need to format the information in each column when you populate the Kick-Start template, consider doing a practice run by exporting a Kick-Start with existing `Workfront` data on the objects you are trying to import. For instructions, see [Export data from Adobe Workfront via Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

When you open a blank Kick-Starts template, a number of tabs (data sheets) are available. They depend on the objects that you selected for download. Each one represents an object in the application, such as project, tasks, hours, dashboard, and users:

![](assets/kick-start-spreadsheet-example-350x383.png)

When you open one of these tabs, row 2 displays the fields for each object that can be set during an import. In a column header, after the word "set," the name of the field displays as it appears in the database. These fields act as column headers.

>[!IMPORTANT]
>
>To avoid errors, make sure of the following:
>
>* Do not delete or modify these fields in any way. For example, don't change their order or their names.
>* Populate every field with a column header displayed in bold. These represent required fields.
>
>  However, if a required field contains a default value set in the system preferences, you don't have to populate it. 
>
>  For example, on the `PROJ Project` tab, the `setCondition` and `setConditionType` fields can be left empty, but the `setGroupID` and `setName` columns cannot.
>

### Import a record

Each row of the sheet corresponds to a unique object.

<ol> 
 <li value="1"> <p>Complete the cell in the <span class="bold">isNew</span> column:</p> 
  <ul> 
   <li> <p>If the object you are importing is new, type <span class="bold">TRUE</span> to import the data in the row.</p> </li> 
   <li> <p>If the object is already in <span>Workfront</span>, type <span class="bold">FALSE</span> to ignore the row.</p> </li> 
  </ul> </li> 
 <li value="2"> <p>Complete the cell in the <span class="bold">ID</span> column in one of the following ways:</p> 
  <ul> 
   <li>If the object you are importing is new (and you typed<span class="bold">TRUE</span> in the <span class="bold">isNew</span> column), specify any number for the ID. This number must be unique in the spreadsheet.</li> 
   <li> <p>If the object you are importing already exists in the <span>Workfront</span> system (and you typed<span class="bold"> FALSE</span> in the <span class="bold">isNew</span> column), the ID must be the alpha-numeric GUID that exists in <span>Workfront</span> for that object.</p> 
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span> 
     <p>For a project, the value displayed in the <span class="bold">setGroupID</span> column must one of the following:</p> 
     <ul> 
      <li>The GUID for an existing Group in your <span>Workfront</span> instance</li> 
      <li> <p>The value (number) in the ID column on the <span class="bold">GROUP Group</span> sheet if you are creating a new Group during the import</p> <p> <img src="assets/verysimplekickstartprojectimport-350x31.png" style="width: 350;height: 31;"> </p> </li> 
     </ul> 
    </div> </li> 
  </ul> </li> 
 <li value="3"> <p>Input values for the required fields and any other fields you want to populate during the import.</p> </li> 
 <li value="4"> <p>(Optional) To add custom data:</p> 
  <ul> 
   <li> Create a new column for each custom field that you want to include in the import process. </li> 
   <li> Name each new column for its corresponding custom field as follows: <span class="bold">DE:[Name of Custom Field as Appears in <span>Workfront</span>]</span>.</li> 
   <li>In the column <span class="bold">setCategoryID</span>, type the GUID of the existing custom form on which this custom field resides. This field is required when importing custom data.</li> 
   <li> <p>If you need to add multiple data values in the custom field, (such as radio buttons, check boxes, or lists) use the vertical bar custom data delimiter "|" listed in the Preferences tab to separate the values.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Type A|D under the DE: Departments column to populate department A and department D in your custom form.</p> </li> 
  </ul> </li> 
</ol>

### Include dates

`Workfront` can process most date formats. However, you must ensure that the date column in the spreadsheet is formatted as a date. The import will fail if the column is formatted as general, a number, or text.

>[!TIP]
>
>Most people find it easiest to use the MM/DD/YYYY format (for example: 07/10/2022).

`Workfront` also accepts time values as part of the date (for example: 07/10/2022 01:30 or 07/10/2022 1:00 PM).

If you omit a time in the date, `Workfront` does one of the following:

<ul> 
 <li> <p>Assumes 12:00 AM</p> </li> 
 <li> <p>If it is on an object that is associated with a schedule, the time defers to the earliest time that the schedule allows:</p> <p> <img src="assets/dateformats.png"> </p> </li> 
</ul>

>[!NOTE]
>
>When using a UNIX time stamp you must include three additional zeros at the end of the value.
>
>For example, if your time stamp is 7336899000, you would input 7336899000000 in the cell.

### Use wildcards

You can use the following wildcards when populating your Kick-Start template spreadsheet:

<table cellspacing="15" cellpadding="5"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><span class="bold">Wildcard</span> </p> </th> 
   <th> <p><span class="bold">Behavior</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>When used on a <span class="bold">setDate</span> field, this wildcard sets the date as midnight on the day when you import the Kick-Start.</p> <p>You can modify the wildcard using the standard syntax allowed with the wildcard on a filter.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you want a project to start on the Monday of the week it is imported on, regardless of the day you actually perform the import, you could use <span class="bold">$$TODAYbw</span>. This sets your project's planned start date as 12:00 AM on Sunday. Since the schedule for the project probably doesn't allow work at that time, it will start at 9:00 AM Monday morning.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>When used on a <span class="bold">setDate</span> field, this wildcard sets the date according to the moment when you create the record during the Kick-Start import.</p> <p>You can modify the wildcard using the standard syntax allowed with the wildcard on a filter.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you want a project to start 3 hours after it is imported, you could use <span class="bold">$$NOW+3h</span>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>When used on a <span class="bold">setAssignedToID</span> or other userID based field, this wildcard assigns the work or otherwise associates the record with the individual performing the import.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>This wildcard was added specifically for Kick-Start user imports. When a <span>Workfront</span> account is created, a user with the System Administrator access level is created. The username assigned to the default administrator can be used as a prefix when creating other users in the account.</p> <p>Because usernames must be unique across all customers, this is useful when you have several individuals with very common usernames such as John Smith, who might have a username "jsmith." By prepending the username assignment with the default administrator username, you guarantee that each username is unique (for example: <span class="bold">$$CUSTOMER.jsmith</span>).</p> <p>Tip: A more elegant way to ensure that usernames are unique system wide is to input the individual's email address in the <span class="bold">setUsername</span> field.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Attribute name substitution for IDs

Though it is a best practice to use IDs whenever possible, sometimes it's inconvenient to cross-reference IDs from one sheet to another when setting a `setAttributeID` value. You can reference values by name simply by changing the column header.

` `**Examples: **`` 

<ul> 
 <li> <p><span class="bold">(project import)</span> </p> <p>When importing projects,&nbsp;set the <span class="bold">setGroupID</span>&nbsp;of the projects by going to the <span class="bold">GROUP Group</span> sheet, making note of the respective Group IDs, and pasting them in the correct cells (<span class="bold">setGroupID</span> column) on the <span class="bold">PROJ Project</span> sheet. </p> <p>This is feasible when working with only a few groups and projects, but if you are working with several of each, it's not practical.</p> <p>To do the Attribute Name Substitution for the example described above, you change the <span class="bold">setGroupID</span> column header to <span class="bold">#setGroupID GROUP</span><span class="bold">name</span>. You can then reference each project's group by name.</p> <note type="note">
   The option to use Attribute Name Substitution is limited to references for existing records only. You cannot use name substitution for objects you are creating in the same import.
  </note> </li> 
 <li> <p><span class="bold">(user import)</span> </p> <p>When importing users,&nbsp;fill in the <span class="bold">setRoleID</span> from a list of roles on the <span class="bold">ROLE Role</span> tab. <br></p> <p>Some of the Role IDs are for records that already exist in the account, and others are being created during the import.</p> <p>For the new user&nbsp;records assigned to existing roles, you can use name substitution. For the new user&nbsp;records assigned to newly imported roles, you cannot. </p> <p>Here is how you can use both methods on the same import file:</p> 
  <ul> 
   <li>Add a column in the spreadsheet to the left of the <span class="bold">setRoleID</span> column.</li> 
   <li>Name the new column <span class="bold">#setRoleID ROLE name</span>.</li> 
   <li> <p>For role assignments to existing records, input the role names in the <span class="bold">#setRoleID ROLE name</span> column.</p> <p>For role assignments to new role records, input the ID you assigned on the ROLE Role sheet in the setRoleID.<br></p> <p> <img src="assets/setroleid-350x66.png" style="width: 350;height: 66;"> </p> </li> 
  </ul> </li> 
</ul>

## Import the spreadsheet data into `Workfront`

After you populate the Excel template with your data (as described in [Import data into Adobe Workfront via a Kick-Start template](#)), you can upload it's data into `Workfront`.

The Kick-Start import supports the following file types:

* XML-based Excel (&#42;.xlsx)
* Legacy Excel (&#42;.xls)
* Zipped (&#42;ZIP) xlsx or xls file

  A zipped file is necessary only when importing an Excel spreadsheet that references documents, avatars, or view, filter, or grouping property files.

  When using a zipped import file, the &#42;ZIP file must have the same name as the &#42;.xlsx or &#42;.xls file, and all contents must be at the same file structure level (no folders).

To import the template spreadsheet data into `Workfront`:

<ol> 
 <li value="1"> <p>(Conditional) If you are using Workfront Fusion, ensure that your FLOs or scenarios are turned off.</p> <p>For information on how to turn off FLOs in <span>Legacy Workfront Fusion</span>, see the <span>Legacy Workfront Fusion</span> <a href="https://learn.fusion.workfront.com/quickstart-2019/">Getting Started</a> guide.</p> <p>For information on how to deactivate scenarios in <span>Workfront Fusion</span>, see <a href="../../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md" class="MCXref xref">Activate or deactivate a scenario</a>.</p> </li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="3">Click <span class="bold">System</span> ><span class="bold"> Import Data (Kick-Starts)</span>.</li> 
 <li value="4">In the <span class="bold">Upload data with Kick-Start spreadsheet</span> section, click <span class="bold">Choose File</span>, then browse to and select the populated spreadsheet.</li> 
 <li value="5"> <p>Click <span class="bold">Upload.</span></p> <p>If the Excel file takes longer than 5 minutes to upload to <span>Workfront</span>, the application times out and the file cannot be uploaded.</p> <p>Try importing your data in smaller batches of objects. &nbsp;</p> </li> 
 <li value="6"> <p>(Conditional) If you are using Workfront Fusion, you can now turn on your FLOs or scenarios.</p> </li> 
</ol>

