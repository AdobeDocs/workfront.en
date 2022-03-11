---
filename: project-actual-start-date
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overview of the project Actual Start Date
description: Projects, tasks, and issues have an Actual Start Date in Adobe Workfront. For tasks, and issues, this is the date when they have been marked as In Progress. For projects, this is the date when the first task on the project is marked as In Progress or has been completed.
---

# Overview of the project Actual Start Date

Projects, tasks, and issues have an&nbsp;Actual Start&nbsp;Date in&nbsp;Adobe Workfront. For tasks, and issues, this is the date when they have been marked as In Progress. For projects, this is the date when the first task on the project is marked as In Progress or has been completed.

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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations about Actual&nbsp;Start&nbsp;Dates in&nbsp;Workfront

* The Actual Start Date is located in the Details section of projects, tasks, and issues.&nbsp;
* The Actual&nbsp;Start Date of a project, task, or issue is not populated when these items are created. 
* The Actual&nbsp;Start&nbsp;Date is populated when work actually starts on the project, task, or issue. 
* The Actual&nbsp;Start Date does not display on the Project Details tab if the work on the project has not started yet.

  The Actual Start&nbsp;Date displays blank on the Task and&nbsp;Issue Details tabs if the work has not yet started on them. 

* You can manually modify the Actual&nbsp;Start&nbsp;Date of a task or an issue, but you cannot modify the Actual&nbsp;Start&nbsp;Date of a project.

## Considerations about Actual Start&nbsp;Dates for projects

<ul> 
 <li>Workfront automatically sets the Actual&nbsp;Date of a project when any of the following occur:
  <ul>
   <li>A task assignee changes the status of a task from <i>New</i> to any other status that does not equate <i>New</i>.</li>
   <li><p>A task assignee changes the Percent Complete of a task.</p><note type="important">
     The Project&nbsp;Actual Start&nbsp;Date does not populate when the project is marked as Current.&nbsp;Actual work must start on the tasks of the project before the Actual&nbsp;Start&nbsp;Date of the project populates. 
    </note><p>In these cases, the Actual Start Date of the project is set to the date and time when these actions occurred for the earliest task on the project. This indicates that the project actually started on this date and time. </p></li>
  </ul></li> 
</ul>

## Locate the Actual Start&nbsp;Date of a project

You can locate the Actual&nbsp;Start&nbsp;Date of a project in the following areas:

* In the Details section of a Project.
* In a project report or view, when you add the Actual&nbsp;Start&nbsp;Date for the object Project in the report.

  For information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

To locate the Actual Start&nbsp;Date in the Details section of the project:

1. Click the Main Menu icon in the upper-right corner of Workfront, then click Projects. 
1. Click the project you want to view the Actual Start Date for.
1. Click Project Details in the left panel, then go to the Overview section. The Actual Start Date displays along other project dates .

&nbsp;
