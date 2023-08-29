---
product-area: reporting
navigation-topic: using-built-in-reports
title: Built-in Status Icons in Views
description: You can add the built-in Status Icons field as a column in your views to enhance visibility into key points about your objects.
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
---
# Built-in Status Icons in Views

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

You can add the built-in Status Icons field as a column in your views to enhance visibility into key points about your objects. Using Status Icons, you can see at a glance when the following conditions exist:

* An object has documents attached
* An object is associated with an approval process
* An object has additional notes associated with it
* An expense is billable or reimbursable 
* A task is on a critical path
* A user belongs to a company, a team, or is located in a different time zone

Consider the following:

* Most of the indicators in the Status Icons field are quick links to the actual object or area of the object that they represent.

* If any of the items represented by the icons are missing from the object, the icon representing the missing item appears dimmed in the Status Icons column instead of a colored image.  

   ![task_status_icons.png](assets/task-status-icons.png)  

   For more information, see the [Overview of Status Icons and Flags](#overview-of-status-icons-and-flags) section in this article.  

* In some views, the **Status Icons** field is named **Flags** or **View Icons**.  
You cannot customize the look and feel of the icons that are included in the Status Icons field.

* You cannot edit the number of icons in the Status Icons field. 

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to Reports,&nbsp;Dashboards, Calendars to add columns to a report</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to an existing view</p> <p>Manage permissions to a report to add columns to it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add the Status Icons field to a view

Some built-in views and reports already have the Status Icons field included.

You cannot add the Status Icons field to all views.

To add the Status Icons field to a custom view that you build from scratch:

1. Go to a list of any of the following objects:

   * Tasks
   * Issues
   * Projects
   * Template Tasks
   * Templates
   * Expenses
   * Documents
   * Users  
     Only these objects have the **Status Icons** field available.  
     For information on object lists, see [Get started with lists in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. From the **View** drop-down menu, select **New View**.

1. Click **Add Column**.
1. In the **Show in this column** box, start typing any of the following field names, then select it when it appears in the list:

   * *Status Icons*
   * *Flags*
   * *View Icons *(only in Document views).

   The built-in icons are listed under any of these names.  
   A Template view contains both the **Status Icons** and the **Flags** fields. In this case, the two columns contain identical icons.   
   Document views contain a **View Icons** field.

1. Click **Save View**. 
1. (Optional) Specify a new name for your view, then click **Save View**.  
   This adds the **Status Icons** column to your View.
1. (Optional) Mouse over an icon to understand what it represents.
1. (Optional) Click an icon to go to the area of the object represented by it.  
   Not all icons are links to objects.  
   For a complete list of attributes for each icon, see the [Overview of Status Icons and Flags](#overview-of-status-icons-and-flags) section.

## Overview of Status Icons and Flags {#overview-of-status-icons-and-flags}

The following table lists all the Status Icons available in Workfront, the type of objects that can be associated with them, as well as what happens when you click them.

You must have permissions to at least View the objects in order to be able to click some of the following icons and access those objects. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Status Icon or Flag</strong> </th> 
   <th><strong>Description</strong> </th> 
   <th><strong>Object</strong> </th> 
   <th>On Click</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">or <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trouble.png" style="width: 29;height: 26;"> or <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> or <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Indicates that the Condition of the project is On Target (green), In Trouble (red), or At Risk (yellow).<br>For information about project Condition, see <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</td> 
   <td>Projects</td> 
   <td>Click to open the tasks list of the project. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Indicates that the object has notes (updates) in the Updates tab.</td> 
   <td> <p>Projects<br>Tasks<br>Issues<br>Templates<br>Template Tasks</p> </td> 
   <td> <p>Click to open the Updates tab of the object. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">or <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Indicates that the object has documents attached. </td> 
   <td> Projects<br>Tasks<br>Issues<br>Templates<br>Template Tasks </td> 
   <td>Click to open the Documents tab of the object. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">or <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Indicates that there are open issues on the project or the task.</td> 
   <td> Projects<br>Tasks </td> 
   <td>Click to open the object. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> or <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Indicates that there is an approval on the object.</td> 
   <td> Projects<br>Tasks<br>Issues<br>Templates<br>Template Tasks </td> 
   <td>Click to open the object. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>You can add an Expenses Icon column in your view to display this icon. This indicates that the project or the task has expenses associated with them.</p> </td> 
   <td> <p>Projects</p> <p>Tasks</p> </td> 
   <td>Click to open the Expenses tab of the project or the task. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Indicates that the Progress Status of a task is one of the following:</p> 
    <ul> 
     <li>On Time (green square)</li> 
     <li>Late (red circle)</li> 
     <li>At Risk (blue diamond)</li> 
     <li>Behind (yellow triangle)</li> 
    </ul> <p>For information about the Progress Status of tasks, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</p> </td> 
   <td>Tasks</td> 
   <td>Click to open the task. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> or <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Indicates that the task is currently on the Critical Path. <br>For information about tasks on a Critical Path of the project, see <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Overview of the project Critical Path</a>.</td> 
   <td>Tasks</td> 
   <td>Click to open the task.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Indicates that the task is associated with a milestone. Your system administrator can customize the color of the diamond in your environment.<br>For information about milestones, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</td> 
   <td>Tasks</td> 
   <td>Click to open the task. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Link to the source object of an issue. The source object of an issue is the object where the issue was logged. A task or a project can be source objects for issues. </td> 
   <td>Issues</td> 
   <td>Click to open the source object (task or project) of an issue. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Indicates that there is a resolving object which ultimately resolves the issue. In this case, you cannot complete the issue. It is completed when the resolving object completes. <br>For information about resolving objects, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</td> 
   <td>Issues</td> 
   <td>Click to open the resolving object of the issue. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>View a document.</td> 
   <td>Documents</td> 
   <td>Click to download the document.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Download a document.</td> 
   <td>Documents</td> 
   <td>Click to download the document.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Indicates the type of document.</td> 
   <td>Documents</td> 
   <td>Click to download the document.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belongs_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Indicates that the user is associated with a Company. </td> 
   <td>Users</td> 
   <td>Unavailable</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Indicates that the user is associated with a Team.</td> 
   <td>Users</td> 
   <td>Click to open the user profile.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Shortcut to the Allocation tab of the user. </td> 
   <td>Users</td> 
   <td>Click to open the Allocation tab of the user and learn to what work items the user is assigned.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Indicates that the user is in a different time zone than that of the system.</td> 
   <td>Users</td> 
   <td>Unavailable</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_expense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Indicates that an expense is billable.<br>For information about expenses, see <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Manage project expenses </a>.</td> 
   <td>Expenses</td> 
   <td>Unavailable</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="expense_reimbursable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> Indicates that an expense is reimbursable.<br>For information about expenses, see <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Manage project expenses </a>.</td> 
   <td>Expenses</td> 
   <td>Unavailable</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="reimbursed_expense_icon.png" style="width: 44;height: 43;"></td> 
   <td> Indicates that an expense has been reimbursed.<br>For information about expenses, see <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Manage project expenses </a>.</td> 
   <td>Expenses</td> 
   <td>Unavailable</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
