---
title: Overview of Project Condition and Condition Type
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: The project Condition is a visual representation of how the project is progressing. It is a reportable variable determined by the relationship between the planned, projected, and estimated dates of the project.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
---
# Overview of Project Condition and Condition Type

<!-- Audited: 12/2023 -->

The project Condition is a visual representation of how the project is progressing. It is a reportable variable determined by the relationship between the planned, projected, and estimated dates of the project.

## Project Condition overview

Consider the following in understanding the Condition of a project:

* As the project owner, you can decide whether the Condition of a project is set manually or automatically. The Condition of a project can be set in the following ways:

   * Manually by users who have access to Manage the project and when the Condition Type of the project is set to Manual.
   * Automatically by Adobe Workfront, when the Condition Type of the project is set to Progress Status. The Progress Status of the project is determined by the progress of the tasks on the project. For information about the Progress Status of the project, see [Project Progress Status overview](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  For information about how to update the Condition Type of the project, see [Set the Condition Type of a project](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* When allowing Workfront to estimate the Condition of the project automatically, we recommend that you use predecessors on your tasks so that the task progress reflects in the actual progress and the Progress Status of the project.
* As a project owner, you can change the project to use a Manual Condition Type instead of using the Progress Status by changing the Condition Type from Progress Status to Manual.

  >[!NOTE]
  >
  >Projects that are in any of the following statuses are always marked as On Target, no matter what the dates of the tasks and their progress are:  
  >
  >* Idea
  >* Requested
  >* Approved
  >* Rejected 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## How Workfront updates Project Condition based on Progress Status

When the Condition Type of the project is set to Manual, you can determine what the Condition of the project is independently from the Progress Status of the project.

However, we recommend that you set the Condition Type of the project to Progress Status so that you can have a clear indication of what the true progress of the project is, based on the progress of your tasks. For information about how Workfront calculates the Progress Status of projects, see [Project Progress Status overview](../../../manage-work/projects/planning-a-project/project-progress-status.md).

In this case, the values for the Project Condition can be:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Project Condition</strong></td> 
   <td><strong>Project Progress Status</strong></td> 
   <td><strong>Workfront Condition Indicator</strong></td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>On Target</td> 
   <td>When Progress Status of the project of On Time, the Condition of the project is <strong>On Target</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>At Risk</td> 
   <td>When the Progress Status of the project is <strong>Behind</strong> or <strong>At Risk</strong>, then the Condition of the project is <strong>At Risk</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>In Trouble</td> 
   <td>When the Progress Status of the project is <strong>Late</strong>, then the Condition of the project is <strong>In Trouble</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Conditions can be customized for your environment, so you may find more than three options for Condition in your environment. The names of the Conditions might be different than the ones listed above. For information about customizing Conditions in , see the article [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Report on Project Condition, Project Condition Update, and Last Condition Note

In the view of a project report, you can show the following fields related to the Condition of the project:

* **Project Condition:** Shows the current Condition of the project. 
* **Project Condition Update**: Shows the most recent update that the project owner has provided in the update stream of the project, along with the new Condition.   
  Comments made on Condition updates are not displayed in the **Condition Update** column; only the main update is displayed. 

* **Last Condition Note**: Displays the update last entered on an object by the owner of the object. This field is helpful to display the owner's most recent activity or interaction on an object.   
  The **Last Condition Note** column is empty if the note text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.

For information about how to create a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
