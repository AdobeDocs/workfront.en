---
filename: create-edit-views
product-area: reporting
navigation-topic: reporting-elements
title: Create and edit views
description: You can customize the type of information you display on the screen using views. You can use several types of views in Adobe Workfront.
---

# Create and edit views

You can customize the type of information you display on the screen using views. You can use several types of views in&nbsp;*Adobe Workfront*.

This article describes how to create and edit standard views for lists and reports, and how to create Agile views. For more information, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to create a view in a report</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to create or edit a view in a report</p> <p>Manage permissions to a view to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create or customize a view

The process for creating or customizing a view differs depending on whether you are creating or customizing a standard view or an agile view.

* [Create or customize a standard view](#customizing-a-standard-view) 
* [Create or customize an Agile view](#customizing-an-agile-view)

### Create or customize a standard view

You can create a new standard view, or you can customize an existing standard view that you previously created.

<ol> 
 <li value="1">Click the<span class="bold"> View</span> drop-down menu on any list where you want to create or customize a view.</li> 
 <li value="2">(Optional) To customize an existing view, select the standard View you want to customize.<br>Standard Views are available on any type of list in <em>Workfront</em>, such as a report, project list, or task list.</li> 
 <li value="3">Click the <span class="bold">View</span> drop-down menu, then click <span class="bold">Customize View</span> or<span class="bold"> New View</span>.<br>The <span class="bold">Customize View</span> dialog box displays.<br></li> 
 <li value="4"> <p>In the <span class="bold">Column Preview</span> section, do any of the following:</p> 
  <ul> 
   <li>Modify the value of any column by clicking the column title and then selecting a new field.</li> 
   <li>Add a column by clicking <span class="bold">Add Column</span>, begin typing the name of the column that you want to add, then click it when it appears in the drop-down list.</li> 
   <li>Adjust the order that columns appear by dragging the column title to a new location. 
    <ul> 
     <li>(Optional) In the <span class="bold">Column Settings</span> area, click the <a name="summarize-this-column-by"></a><span class="bold">Summarize this column by</span> drop-down list, then select one of the available options for summarizing the information. When you choose this option, the information in your column is aggregated in the groupings of the report.<br>For date fields, you can summarize the values by the following options: 
      <ul> 
       <li>Maximum</li> 
       <li>Minimum</li> 
      </ul><p>For number and currency fields, you can summarize the values by the following options:</p> 
      <ul> 
       <li>Count</li> 
       <li>Sum</li> 
       <li>Average</li> 
       <li>Maximum</li> 
       <li>Minimum</li> 
      </ul> <note type="note">  
       <p>The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:</p> 
       <ul> 
        <li>All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.</li> 
        <li>Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.</li> 
        <li>Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.</li> 
       </ul> 
      </note><p>For more information about using groupings in a report, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p></li> 
     <li>(Optional) Click <span class="bold">Advanced Options</span> to specify the following information for the column:<p> 
       <table cellspacing="0"> 
        <col> 
        <col> 
        <thead> 
         <tr> 
          <th> </th> 
          <th> </th> 
         </tr> 
        </thead> 
        <tbody> 
         <tr> 
          <td role="rowheader"><span class="bold">Custom Column Label</span></td> 
          <td><p>Specify a custom label for the column. This label replaces the default label.</p></td> 
         </tr> 
         <tr> 
          <td role="rowheader"><span class="bold">Field Format</span></td> 
          <td>Select the format in which you want the values to be displayed for fields in the column.</td> 
         </tr> 
         <tr> 
          <td role="rowheader"><span class="bold">Show this column when on a Dashboard</span></td> 
          <td><p>Select this option to show this column on a dashboard, when the report is displayed side by side with another report. When this option is unselected, this column is not displayed when viewing the report on a dashboard where reports are displayed side by side.</p></td> 
         </tr> 
         <tr> 
          <td role="rowheader"><span class="bold">Column Rules</span></td> 
          <td><p>Click <span class="bold">Add a Rule for this Column</span> to define a rule for the column. After you add a rule, you can define field and text styles for how fields that match that rule are displayed. Click <span class="bold">Add Rule</span> after you have finished defining the rule.</p></td> 
         </tr> 
        </tbody> 
       </table></p><p>For more information about conditionally formatting views in reports, see the article <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p></li> 
    </ul></li> 
  </ul> </li> 
 <li value="5">(Conditional) If you clicked <span class="bold">Advanced Options</span>, click <span class="bold">Done</span>.</li> 
 <li value="6"> <p>Click <span class="bold">Save View</span> to create a new View or to replace the current View with your changes.<br>Or<br>Click <span class="bold">Save as New View</span> to save your changes as a new View.</p> <note type="tip">
   The 
   <span class="bold">Save as New View</span> is the only option available when you customize a built-in 
   <em>Workfront</em> view.
  </note> <p>Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.</p> </li> 
</ol>

### Create or customize an Agile view

You can create a new Agile view or customize an existing Agile view that you previously created.

>[!IMPORTANT]
>
>Agile views are available only when viewing a project.

For more information about Agile views, see the article [Manage a project in the Agile View](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

To create or customize an Agile view:

<ol> 
 <li value="1">Go to the list of tasks on a project.</li> 
 <li value="2">Click the <span class="bold">Agile</span> icon .<br></li> 
 <li value="3">(Conditional) To customize an existing Agile view:</li> 
 <ol> 
  <li value="1">Click the <span class="bold">View</span> drop-down menu, then select the Agile View you want to customize.<br>You cannot customize the default Agile view.</li> 
  <li value="2">Click the <span class="bold">View</span> drop-down menu again, then click <span class="bold">Customize View</span>.<br><img src="assets/view-agile-customize.png" alt=""></li> 
 </ol> 
 <li value="4">(Conditional) To create a new Agile view, click <span class="bold">New View</span>.<br>The <span class="bold">Customize Agile View</span> dialog box displays.<br></li> 
 <li value="5">In the <span class="bold">Customize Agile View</span> dialog box, specify a name for the Agile view.<br>We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.<br>This name is displayed in the <span class="bold">View</span> drop-down menu when selecting a view.</li> 
 <li value="6"> <p>Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the <em>Workfront administrator</em>, as described in <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> <p>Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.</p> <p>Users can move stories among these status columns on the Agile story board.<br>When defining status columns, you can do the following:</p> <p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> </th> 
      <th> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><span class="bold">Reorder status columns:</span> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Remove status columns:</span> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Add status columns:</span> </td> 
      <td>Click the <span class="bold">Plus</span> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</td> 
     </tr> 
    </tbody> 
   </table> </p> <p> </p> <p> </p> </li> 
 <li value="7"> <p>In the <span class="bold">Associate Card Color to</span> area, select from the following options: </p> <p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> </th> 
      <th> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><span class="bold">Story:</span> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Free Form:</span> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Priority:</span> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your <em>Workfront administrator</em> has configured custom priorities for your <em>Workfront</em> system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Task Owner:</span> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table> </p> </li> 
 <li value="8"> <p>In the <span class="bold">Agile</span> section, in the <span class="bold">Additional Fields</span> area, click <span class="bold">Add Field</span>, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)<br>Repeat this process to add up to 3 additional fields to the story cards.<br>When you add fields to story cards, fields are view-only and display only when the field is populated.</p> <p>By default, the following types of data is displayed on the story card:</p> 
  <ul> 
   <li>Story name with a link directly to the task</li> 
   <li>The project name with a link directly to the project<br>This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.</li> 
   <li>The task description</li> 
   <li>Current commitment</li> 
   <li>View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete</li> 
   <li>Assigned Users</li> 
  </ul> <p>You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.</p> </li> 
 <li value="9">Click <span class="bold">Save</span>.<br>Your access dictates how the View is saved. If you created the View originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the View impact users with whom the View has been shared.</li> 
</ol>

&nbsp;
