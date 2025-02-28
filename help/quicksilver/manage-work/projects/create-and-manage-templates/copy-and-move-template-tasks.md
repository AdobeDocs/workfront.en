---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copy and move template tasks
description: You can copy or move a template task to the same template or to another template.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
---
# Copy and move template tasks

You can copy a template task from a template to another template, or you can move it either to another template or to another place in the same template. 

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
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
   <td> <p>Edit access to templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template and to the template task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for copying or moving template tasks

Consider the following when copying template tasks:

* The following information does not transfer to the copied task: 

   * Milestones

* You have a chance to select to copy some items associated with the template task to the copied task during the copying process. However, by default, the following objects do not transfer to the copied task:

   * User comments

* Custom forms are copied with the template task when you copy a template task. The information in the custom fields transfers to the new template task only when you select to copy Custom Data. 

* The following items transfer to the copied template task by default:

   * Subtasks

Consider the following when moving template tasks: 

* The following information transfers to the moved task, by default:

   * Custom forms and custom field information
   * Subtasks
   * User comments

* The following information does not transfer to the moved task: 

   * Milestones.

## Copy template tasks 

You can copy a single template task or you can copy several template tasks in bulk. 

1. Go to the template that contains the template task or template tasks that you want to copy.
1. Click **Template Tasks** in the left panel. 
1. Do one of the following:
    * Click the name of a template task to open it.
    * Select one or several template tasks in the list. 
1. (Conditional) Click the **More** menu ![More icon](assets/more-icon.png) at the top of the template task list or to the right of the template task name if you opened the task, then click **Copy to** or **Copy**, depending where you are accessing the Copy option from. 
    The Copy Template Task box opens.
    ![Copu template task box](assets/copy-template-task-box-unshimmed.png)
1. (Optional) Rename the template task in the **Template Task Name** field.

   >[!TIP]
   >
   >This field is dimmed and not editable when selecting to copy multiple template tasks in a list. You can hover over the Template Task Name field and a list of all selected template tasks displays.

1. Start typing the name of the **Destination Template** where you want to copy the template task in the **Select Destination Template** field, then select it when it displays in the list. 

    The current template name displays by default. If you want to copy the template task within the same template, leave this field unchanged. 

   >[!TIP]
   >
   >You can also start typing the Reference Number or enter the ID of the template. This might help you distinguish between templates with identical names. 

1. (Conditional) Click **request access** to request access to the destination template, if you don't have access to the selected template.
1. (Conditional) Continue to copy the template task to the selected destination template without requesting access if you have access to add template tasks to one of the template tasks on the destination template.

1. Click **Options** in the left panel, then deselect the template task attributes that you do not want to copy with the template task. All options are selected by default.

   >[!TIP]
   >
   >Deselecting **Select all** deselects all the options.

   Deselect from the following options to not transfer them to the copied template task. The following table describes what happens when the options are deselected: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Select all</td> 
      <td>Deselect this option to remove all information from the template task when copying it to its new location. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Constraint</td> 
      <td> <p>The template task constraint is set to As Soon As Possible or As Late As Possible based on the template Schedule Mode setting.</p> <p> When selected, the current constraint of the template task transfers to the copied template task. </p> 
      <p><b>NOTE</b> 
      
      When copying a template task with date-specific constraints to another template and the constraint dates of the template task are outside the dates of the new template, either the template task Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the templates are adjusted. 
      
      The following are examples of date-specific constraints:
      <ul>
      <li> Must Start On</li>
      <li> Must Finish On</li>
      <li> Start No Earlier Than</li>
      <li> Start No Later Than</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assignments</td> 
      <td> <p>All the assignments are removed from the template task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approval Process</td> 
      <td>All approval processes are removed from the template task.</td> 
     </tr> 

     <tr> 
      <td role="rowheader">All Predecessors</td> 
      <td> <p>This means that the dependencies will not carry over to the copied template tasks. </p> <p>When selected, the predecessors within the group of copied template tasks are preserved, others are deleted.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Custom Data</td> 
      <td> <p>The values for the custom fields are cleared and the custom forms are transferred to the copied template task. </p> <p>When selected, both the forms and the values for the custom fields transfer to the copied template task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financial Information</td> 
      <td>The financial information of the copied template task is removed and the Workfront updates the template task Cost Type to No Cost and the template task Revenue Type as Not Billable.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>The documents attached to the template task are not transferred to the copied template task. This includes versions, proofs, and linked documents.</p> <p><b>NOTE</b></p>
      
      <p>This does not include document approvals. Document approvals can never be copied when a template task is copied.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reminder Notifications</td> 
      <td>The template task reminders do not transfer to the copied template task. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expenses</td> 
      <td>The expenses logged on the template task do not transfer to the copied template task. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Optional) Click **Select Parent** in the left panel, then select the template task in the destination template that you want to become the parent of the copied template task.

   >[!TIP]
   >
   >When selecting to copy multiple template tasks in a list, all selected template tasks become the children of the selected parent and are added after the existing children tasks.

   Select a parent by doing one of the following:

   * In the template task list, select one of the parents in the template plan.
   * Click the search icon ![Search icon](assets/search-icon.png) and search for a parent template task by name.

   The template task should appear in the list.

1. Select the radio button for the parent, after you have found it.

   If you do not select a parent template task, the template tasks are copied as main template tasks rather than subtasks and they are placed at the end of the template task list on the destination template. 

1. Click **Copy Template Task**.

   The copied template tasks are now on the specified template and are either subtasks to the selected parent template task, or the last template tasks on the template.


## Move template tasks 

You can move a template task either to another template task in the same template or to another template. You can move one template task or multiple template tasks, in bulk.

1. Go to the template that contains the template task or template tasks that you want to move.
1. Click **Template Tasks** in the left panel. 
1. Do one of the following:
    * Click the name of a template task to open it.
    * Select one or several template tasks in the list. 
1. (Conditional) Click the **More** menu ![More icon](assets/more-icon.png) at the top of the template task list or to the right of the template task name if you opened the task, then click **Move to** or **Move**, depending where you are accessing the Move option from. 
    The Move Template Task box opens.
    ![Move template task box](assets/move-template-task-box-unshimmed.png)

1. (Optional) Rename the template task in the **Template Task Name** field.

   >[!TIP]
   >
   >This field is dimmed and not editable when selecting to move multiple template tasks in a list. You can hover over the template task Name field and a list of all selected template tasks displays.

1. Start typing the name of the **Destination Template** where you want to move the template task in the **Select Destination Template** field, then select it when it displays in the list. 

   >[!TIP]
   >
   >You can also start typing the Reference Number or enter the ID of the template. This might help you distinguish between templates with identical names. 

1. (Conditional) Click **request access** to request access to the template, if you don't have access to the destination template.
1. (Conditional) Continue to move the template task to the selected destination template without requesting access if you have access to add template tasks to one of the template tasks on the destination template.

1. Click **Options** in the left panel, then deselect the template task attributes that you do not want to copy with the template task. All options are selected by default.

   >[!TIP]
   >
   >* The Options section is available only after you have selected a destination template. 
   >* Deselecting **Select all** deselects all the options.

   Deselect from the following options to not transfer the information to the moved template task. The following table describes what happens when the options are deselected: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Select all</td> 
      <td>Deselect this option to remove all information from the template task when moving it to its new location. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Constraint</td> 
      <td> <p>The template task constraint is set to As Soon As Possible or As Late As Possible based on the template Schedule Mode setting.</p> <p> When selected, the current constraint of the template task transfers to the moved template task. </p> 

      <p><b>NOTE</b> 
      
      When moving a template task with date-specific constraints to another template and the constraint dates of the template task are outside the dates of the new template, either the template task Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the templates are adjusted. 
      
      The following are examples of date-specific constraints:
      <ul>
      <li> Start On</li>
      <li> Must Finish On</li>
      <li> Start No Earlier Than</li>
      <li> Start No Later Than</li>
      </ul>


     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assignments</td> 
      <td> <p>All the assignments are removed from the template task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approval Process</td> 
      <td>All approval processes are removed from the template task.</td> 
     </tr> 

     <tr> 
      <td role="rowheader">All Predecessors</td> 
      <td> <p>This means that the dependencies will not carry over with the moved template tasks. </p> <p>When selected, the predecessors within the group of moved template tasks are preserved, others are deleted.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Custom Data</td> 
      <td> <p>The values for the custom fields are cleared and the custom forms are transferred with the moved template task. </p> <p>When selected, both the forms and the values for the custom fields transfer with the moved template task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financial Information</td> 
      <td>The financial information of the moved template task is removed and the Workfront updates the template task Cost Type to No Cost and the template task Revenue Type as Not Billable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>The documents attached to the template task are not transferred with the moved template task. This includes versions, proofs, and linked documents.</p> 
      
      <p><b>NOTE</b></p>
      
      <ul><li>
      <p>This does not include document approvals. Document approvals can never be moved when a template task is moved.</p> </li>
      <li>If you opt to not have the documents moved with the template task, the documents are deleted and placed in the Recycle Bin for 30 days. An administrator can restore them and they will be restored on the moved template task. 
      
      If the template task is deleted after it's moved, the restored documents will be placed in the Documents area of the user page of the administrator who restores them. </li> </ul>
      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reminder Notifications</td> 
      <td>The template task reminders do not transfer to the moved template task. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expenses</td> 
      <td>The expenses logged on the template task do not transfer with the moved template task. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Optional) Click **Select Parent** in the left panel, then select the template task in the destination template that you want to become the parent of the moved template task.

   >[!TIP]
   >
   >When selecting to move multiple template tasks in a list, all selected template tasks become the children of the selected parent and are added after the existing children tasks.

   Select a parent by doing one of the following:

   * In the template task list, select one of the parents in the template plan.
   * Click the search icon ![Search icon](assets/search-icon.png) and search for a parent template task by name.

   The template task should appear in the list.

1. Select the radio button for the parent, after you have found it.

   If you do not select a parent template task, the template tasks are moved as main template tasks rather than subtasks and they are placed at the end of the template task list on the destination template. 

1. Click **Move Template Task**. 

   The moved template tasks are now on the specified template and are either subtasks to the selected parent template task, or the last template tasks on the template.
