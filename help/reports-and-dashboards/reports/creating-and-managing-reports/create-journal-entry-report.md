

# Report on the Updates area

The Journal Entry report surfaces system updates from the Updates area of projects, tasks, issues, and other objects that were previously only available through the `Adobe Workfront` API. While this is an advanced report intended for specific use cases, the more digestible format makes it easier for you to report on project activity and system updates within `Workfront`.

>[!TIP]
>
>The Journal Entry report contains only system updates from the Updates area of objects. To report on comments left in the Updates area, you must use the Note report.  
>For more information on the Note report, see [View all updates in a Note report](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md).‍

The Journal Entry report can show:

* How many status changes occurred
* When a task or issue was deleted
* How values in important custom fields changed over the course of a project's life cycle
* What important dates changed over the course of a project's life cycle
* If the owner of a project changed

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the objects that contain the journal entries you display in the report</p> <p>You will obtain Manage permissions to the report after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

Before you begin, you must make sure:

* Any fields that you want to report on are tracked in `Workfront`. You can only report on data from the Updates area that is tracked.

  To learn how to add fields that you want `Workfront` to track, see [Configure system updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Any custom fields that you want to report on have the setting `Display field changes in update feeds` enabled.

  To learn how to enable this setting for a custom field, see the section [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Journal Entry report overview

Because the Journal Entry report queries system updates, it can return a significant number of results. For this reason, we recommend that you filter to specific objects—such as projects, programs, portfolios, groups, and so forth—when creating the report.

To learn more about the different object types in `Workfront`, see [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Because the Journal Entry report returns so much data, exporting and scheduled report delivery are not supported.

The default view for this report contains the following columns:

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Field</th> 
   <th>Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><span class="bold">Field Name</span> </td> 
   <td> <p><span style="font-weight: normal;">The name of the affected field. Depending on how you set up the report, this column could contain Status, Owner ID, Task Name, Planned Completion Date, or other fields.</span> </p> <p><span style="font-weight: normal;">When</span> <span class="bold">DE</span>:<span style="font-weight: normal;"> displays in this column, it indicates that the field listed is a custom field.</span></p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Change Type</span> </td> 
   <td> <p>The type of change made to the affected field. Depending on the filter rules that you set up and the actions taken by users, the following might appear in this field:</p> 
    <ul> 
     <li> <p>Add</p> </li> 
     <li> <p>Audit</p> </li> 
     <li> <p>Delete</p> </li> 
     <li> <p>Digest</p> </li> 
     <li> <p>Edit</p> </li> 
     <li> <p>Restore</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Top ObjCode</span> </td> 
   <td> <p>The highest parent object in the hierarchy.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Scope</span> </td> 
   <td> <p>The type of object that was changed.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Entry Date</span> </td> 
   <td> <p>The date that the field was changed.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Edited by Name</span> </td> 
   <td> <p>The user that changed the field.</p> </td> 
  </tr> 
 </tbody> 
</table>

To organize the information in this report, you can use the built-in grouping Project. The Project grouping gives you a primary grouping of Project Name and a secondary grouping of Entry Date. You can apply this existing grouping during report creation, or you can apply it when viewing the report.

To learn how to set up the views, filters, and groupings you want for your report, see the relevant section:

* [See what status changes occurred](#see) 
* [See when a task or issue was deleted](#see2) 
* [See how custom fields changed over the course of a project's life cycle](#see3) 
* [See how the Planned Completion Date changed over the course of a project's life cycle](#see4) 
* [See if the owner of a project changed](#see6)

## See what status changes occurred

You can set up the Journal Entry report to show:

* How many status changes were made on a project, task, or issue

* What the previous status was before the change
* Who changed the status
* When the status change took place

If you want to see the health of a project, you could also set up the report to show this same information using the project `Condition` field.

This information can be used to help with auditing and to illustrate how well you and your organization are planning.

>[!TIP]
>
>If you want to compare the difference in days between condition changes, you can use `Enhanced analytics`.  
>To learn more about `Enhanced analytics`, see [Enhanced analytics overview](../../../enhanced-analytics/enhanced-analytics-overview.md).

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Reports. 
 <li value="2"> <p>Click <span class="bold">New Report</span>, then select <span class="bold">Journal Entry</span>.</p> <p>  </p> <p>The report builder loads.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Columns (View)</span> tab, add the following columns:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Column</th> 
     <th>Explanation</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p style="font-weight: bold;">Field Name</p> </td> 
     <td> <p>The name of the affected field. In this case, <span class="bold">status</span> should display in this column.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Change Type</p> </td> 
     <td> <p>The type of change made to the affected field, such as <span class="bold">Add</span>, <span class="bold">Delete</span>, or <span class="bold">Edit</span>.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Edited by Name</p> </td> 
     <td> <p>The name of the user that updated the status.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Entry Date</p> </td> 
     <td> <p>The date that the status was changed.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Old Text Value</p> </td> 
     <td> <p>The key for the previous status. The following are the status keys for the default project statuses:</p> 
      <ul> 
       <li> <p> <span class="bold">CUR</span>: Current</p> </li> 
       <li> <p><span class="bold">DED</span>: Dead</p> </li> 
       <li> <p><span class="bold">ONH</span>: On Hold</p> </li> 
       <li> <p><span class="bold">PLN</span>: Planning</p> </li> 
       <li> <p><span class="bold">CPL</span>: Complete</p> </li> 
       <li> <p><span class="bold">REQ</span>: Requested</p> </li> 
       <li> <p><span class="bold">APR</span>: Approved</p> </li> 
       <li> <p><span class="bold">REJ</span>: Rejected</p> </li> 
       <li> <p><span class="bold">IDA</span>: Idea</p> </li> 
      </ul> <p>If your organization has set up custom statuses, other status keys might appear in this column. To learn what custom status is related to a status key, contact your <span>Workfront administrator</span> or <span>group administrator</span>.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">New Text Value</p> </td> 
     <td> <p>The key for the updated status.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
     <td> <p>The highest parent object for the field that had the status change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Scope</p> </td> 
     <td> <p>The type of object that had the status change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Issue Name<br>(Optional)</p> </td> 
     <td> <p>The name of the issue that had a status change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Task Name<br>(Optional)</p> </td> 
     <td> <p>The name of the task that had a status change.</p> </td> 
    </tr> 
   </tbody> 
  </table> <p>For more information on adding columns, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Filters</span> tab, click <span class="bold">Add filter rule</span>, then add the filter rule <span class="bold">Field Name</span> > <span class="bold">Equal</span> > <span class="bold">status</span>.</p> <p>  </p> <note type="tip">
   To report on condition changes, you can instead add the filter rule 
   <span class="bold">Field Name</span> > 
   <span class="bold">Equal</span> > 
   <span class="bold">Condition</span>.
  </note> <p>For more information on adding filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </li> 
 <li value="5"> <p>(Optional) To narrow the focus of the report and reduce load times, add a prompt.</p> <p>Or</p> <p>Create additional filter rules to include specific projects, tasks, or issues.</p> <note type="important">
   Creating a filter rule that uses the modifier 
   <span class="bold">Contains</span> can actually increase load times. For this reason, we recommend using a different modifier like 
   <span class="bold">Equal</span> when possible to filter for a specific project or higher-level object ID.
  </note> <p> To learn how to add a prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p> </li> 
 <li value="6"> <p>In the <span class="bold">Groupings</span> tab, click <span class="bold">Apply an Existing Grouping</span>, then select <span class="bold">Project</span>.</p> <p>For more information on adding groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save + Close</span>.</p> <p>Your new report loads.</p> </li> 
</ol>

## See when a task or issue was deleted

You can set up the Journal Entry report to show:

* What tasks or issues have been deleted
* Who deleted a task or issue

To see when a task or issue was deleted:

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Reports. 
 <li value="2"> <p>Click <span class="bold">New Report</span>, then select <span class="bold">Journal Entry</span>.</p> <p>  </p> <p>The report builder loads.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Columns (View)</span> tab, add the following columns:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Column</th> 
     <th>Explanation</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p style="font-weight: bold;">Scope</p> </td> 
     <td> <p>The type of object that was deleted.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Change Type</p> </td> 
     <td> <p>The type of change that happened. The <span class="bold">Delete</span> change displays in this column.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Entry Date</p> </td> 
     <td> <p>The date that the task or issue was deleted.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Edited by Name</p> </td> 
     <td> <p>The name of the user that deleted the task or issue.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Project Name</p> </td> 
     <td> <p>The name of the project that had tasks or issues deleted.</p> </td> 
    </tr> 
   </tbody> 
  </table> <p>For more information on adding columns, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Filters</span> tab, click <span class="bold">Add filter rule</span>, then add the following:</p> 
  <ul> 
   <li> <p><span class="bold">Change Type</span> > <span class="bold">Equal</span> > <span class="bold">Delete</span></p> </li> 
   <li> <p><span class="bold">Project ID</span> > <span class="bold">Equal</span> > <span class="bold"><project></span></p> <p><a href="../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png"></a> </p> </li> 
  </ul> <p>For more information on adding filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </li> 
 <li value="5"> <p>(Optional) To narrow the focus of the report and reduce load times, add a prompt.</p> <p>Or</p> <p>Create additional filter rules to include specific projects, tasks, or issues.</p> <note type="important">
   Creating a filter rule that uses the modifier 
   <span class="bold">Contains</span> can actually increase load times. For this reason, we recommend using a different modifier like 
   <span class="bold">Equal</span> when possible to filter for a specific project or higher-level object ID.
  </note> <p> To learn how to add a prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p> </li> 
 <li value="6"> <p>(Optional) In the <span class="bold">Groupings</span> tab, click <span class="bold">Apply an Existing Grouping</span>, then select <span class="bold">Project</span>.</p> <p>For more information on adding groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save + Close</span>.</p> <p>Your new report loads.</p> </li> 
</ol>

## See how custom fields changed over the course of a project's life cycle

You can track important field changes over the course of the project. To do this, you can set up the Journal Entry to track:

* If certain custom fields were added, updated, or edited
* When these changes happened
* Who made the changes

To see how custom fields changed over the course of a project's life cycle:

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Reports. 
 <li value="2"> <p>Click <span class="bold">New Report</span>, then select <span class="bold">Journal Entry</span>.</p> <p>  </p> <p>The report builder loads.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Columns (View)</span> tab, add the following columns:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Column</th> 
     <th>Explanation</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p style="font-weight: bold;">Field Name</p> </td> 
     <td> <p>The name of the custom field affected.</p> <p><span style="font-weight: normal;">When</span> <span class="bold">DE</span>:<span style="font-weight: normal;"> displays in this column, it indicates that the field listed is a custom field.</span></p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Change Type</p> </td> 
     <td> <p>The type of change made to the affected field, such as <span class="bold">Add</span>, <span class="bold">Delete</span>, or <span class="bold">Edit</span>.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Edited by Name</p> </td> 
     <td> <p>The name of the user that updated the custom field.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Entry Date</p> </td> 
     <td> <p>The date that the value in the custom field changed.</p> <p>You should sort by this field in descending order.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Old Number Value</p> </td> 
     <td> <p>The previous number value in the custom field.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">New Number Value</p> </td> 
     <td> <p>The current number value in the custom field.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Old Date Value</p> </td> 
     <td> <p>The previous date value in the custom field.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">New Date Value</p> </td> 
     <td> <p>The current date value in the custom field.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Old Text Value</p> </td> 
     <td> <p>The previous text value in the custom field.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">New Text Value</p> </td> 
     <td> <p>The current text value in the custom field.</p> <p>If the custom field is a typeahead field, the <span class="bold">New Text Value</span> column displays the object ID.</p> </td> 
    </tr> 
   </tbody> 
  </table> <p>For more information on adding columns, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Filters</span> tab, click <span class="bold">Add filter rule</span>, then add the following:</p> 
  <ul> 
   <li> <p><span class="bold">Journal Entry Field Name</span> > <span class="bold">Contains</span> > <span class="bold">DE</span></p> <note type="tip">
     To limit this report to specific custom fields, add the filter rule 
     <span class="bold">Journal Entry Field Name</span> > 
     <span class="bold">Equal</span> > 
     <span class="bold"><custom field></span>.
    </note> </li> 
   <li> <p><span class="bold">Project ID</span> > <span class="bold">Equal</span> > <span class="bold"><project></span></p> <p>  </p> </li> 
  </ul> <p>For more information on adding filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </li> 
 <li value="5"> <p>(Optional) To narrow the focus of the report and reduce load times, add a prompt.</p> <p>Or</p> <p>Create additional filter rules to include specific projects, tasks, or issues.</p> <note type="important">
   Creating a filter rule that uses the modifier 
   <span class="bold">Contains</span> can actually increase load times. For this reason, we recommend using a different modifier like 
   <span class="bold">Equal</span> when possible to filter for a specific project or higher-level object ID.
  </note> <p> To learn how to add a prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p> </li> 
 <li value="6"> <p>In the <span class="bold">Groupings</span> tab, click <span class="bold">Apply an Existing Grouping</span>, then select <span class="bold">Project</span>.</p> <p>For more information on adding groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save + Close</span>.</p> <p>Your new report loads.</p> </li> 
</ol>

## See how the Planned Completion Date changed over the course of a project's life cycle

You can set up the Journal Entry report to show how often the Planned Completion Date changes over the course of a project’s life.

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Reports. 
 <li value="2"> <p>Click <span class="bold">New Report</span>, then select <span class="bold">Journal Entry</span>.</p> <p>  </p> <p>The report builder loads.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Columns (View)</span> tab, add the following columns:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Column</th> 
     <th>Explanation</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p style="font-weight: bold;">Field Name</p> </td> 
     <td> <p>The name of the affected field.</p> <p><span style="font-weight: normal;">When</span> <span class="bold">DE</span>:<span style="font-weight: normal;"> displays in this column, it indicates that the field listed is a custom field.</span></p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Change Type</p> </td> 
     <td>The type of change that happened, such as <span class="bold">Add</span>, <span class="bold">Delete</span>, or <span class="bold">Edit</span>.</td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Edited by Name</p> </td> 
     <td> <p>The name of the user that updated the project's Planned Completion Date.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Entry Date</p> </td> 
     <td> <p>The date that the project's Planned Completion Date was changed.</p> <p>You should sort by this field in descending order.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
     <td> <p>The highest parent object for the field that had the Planned Completion Date change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Scope</p> </td> 
     <td> <p>The object that had the Planned Completion Date change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Old Date Value</p> </td> 
     <td> <p>The previous value for the Planned Completion Date.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">New Date Value</p> </td> 
     <td> <p>The current value for the Planned Completion Date.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Project Name</p> <p>(Optional)</p> </td> 
     <td> <p>Thhe name of the project that had the Planned Completion Date change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Task Name</p> <p>(Optional)</p> </td> 
     <td> <p>The name of the tasks in the project that had the Planned Completion Date change.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Issue Name</p> <p>(Optional)</p> </td> 
     <td>The name of the issues in the project that have the Planned Completion Date change.</td> 
    </tr> 
   </tbody> 
  </table> <p>For more information on adding columns, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Filters</span> tab, click <span class="bold">Add filter rule</span>, then add the following:</p> 
  <ul> 
   <li> <p><span class="bold">Field Name</span> > <span class="bold">Equal</span> > <span class="bold">Date</span></p> </li> 
   <li> <p><span class="bold">Project ID</span> > <span class="bold">Equal</span> > <span class="bold"><project></span></p> </li> 
  </ul> <p>  </p> <p>For more information on adding filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.<br></p> </li> 
 <li value="5"> <p>(Optional) To narrow the focus of the report and reduce load times, add a prompt.</p> <p>Or</p> <p>Create additional filter rules to include specific projects, tasks, or issues.</p> <note type="important">
   Creating a filter rule that uses the modifier 
   <span class="bold">Contains</span> can actually increase load times. For this reason, we recommend using a different modifier like 
   <span class="bold">Equal</span> when possible to filter for a specific project or higher-level object ID.
  </note> <p> To learn how to add a prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p> </li> 
 <li value="6"> <p>In the <span class="bold">Groupings</span> tab, click <span class="bold">Apply an Existing Grouping</span>, then select <span class="bold">Project</span>.</p> <p>For more information on adding groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save + Close</span>.</p> <p>Your new report loads.</p> </li> 
</ol>

## See if the owner of a project changed

You can set up the Journal Entry report to show how many times the project owner—or project manager—changes over the course of a project's life.

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Reports. 
 <li value="2"> <p>Click <span class="bold">New Report</span>, then select <span class="bold">Journal Entry</span>.</p> <p>  </p> <p>The report builder loads.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Columns (View)</span> tab, add the following columns:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Column</th> 
     <th>Explanation</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p style="font-weight: bold;">Field Name</p> </td> 
     <td>The name of the affected field. The <span class="bold">ownerID</span> displays in this column.</td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Change Type</p> </td> 
     <td> <p>The type of change that happened, such as <span class="bold">Add</span>, <span class="bold">Delete</span>, or <span class="bold">Edit</span>.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
     <td> <p>The highest parent object for the project that had the project owner updated.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Entry Date</p> </td> 
     <td>The date that the project owner was changed.<br>You should sort by this field in descending order.</td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Edited by Name</p> </td> 
     <td> <p>The name of the user that updated the project owner.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Additional Info 1</p> </td> 
     <td> <p>The current project owner on the project.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Additional Info 2</p> </td> 
     <td> <p>The previous project owner on the project.</p> </td> 
    </tr> 
    <tr> 
     <td> <p style="font-weight: bold;">Project Name</p> </td> 
     <td> <p>The project that had the Project Owner field updated.</p> </td> 
    </tr> 
   </tbody> 
  </table> <p>For more information on adding columns, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Filters</span> tab, click <span class="bold">Add filter rule</span>, then add the following:</p> 
  <ul> 
   <li> <p><span class="bold">Field Name</span> > <span class="bold">Equal</span> > <span class="bold">ownerID</span></p> </li> 
   <li> <p><span class="bold">Project ID</span> > <span class="bold">Equal</span> > <span class="bold"><project name></span></p> <p>  </p> </li> 
  </ul> <p>For more information on adding filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </li> 
 <li value="5"> <p>(Optional) To narrow the focus of the report and reduce load times, add a prompt.</p> <p>Or</p> <p>Create additional filter rules to include specific projects, tasks, or issues.</p> <note type="important">
   Creating a filter rule that uses the modifier 
   <span class="bold">Contains</span> can actually increase load times. For this reason, we recommend using a different modifier like 
   <span class="bold">Equal</span> when possible to filter for a specific project or higher-level object ID.
  </note> <p> To learn how to add a prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p> </li> 
 <li value="6"> <p>(Optional) In the <span class="bold">Groupings</span> tab, click <span class="bold">Apply an Existing Grouping</span>, then select <span class="bold">Project</span>.</p> <p>For more information on adding groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save + Close</span>.</p> <p>Your new report loads.</p> </li> 
</ol>

