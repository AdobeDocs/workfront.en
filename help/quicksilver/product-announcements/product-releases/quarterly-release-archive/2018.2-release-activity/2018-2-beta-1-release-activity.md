---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 1 release activity
description: This page describes all changes most recently available in the Preview environment with the 2018.2 Beta 1 release. The functionality was made available in the Preview environment on March 22, 2018. It will be made available in the Production environment in June 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
---
# 2018.2 Beta 1 release activity

This page describes all changes most recently available in the Preview environment with the 2018.2 Beta 1 release. The functionality was made available in the Preview environment on March 22, 2018. It will be made available in the Production environment in June 2018.

>[!IMPORTANT]
>
>Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2018.2, see [2018.2 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

The 2018.2 Beta 1 release contains the following enhancements:

* [Modify Task Dates in the Gantt Chart](#modify-task-dates-in-the-gantt-chart) 
* [Access the Project Gantt Chart from the Updates Tab](#access-the-project-gantt-chart-from-the-updates-tab) (Temporarily Removed) 

* [Various Links Re-Introduced to Documents on the Document List](#various-links-re-introduced-to-documents-on-the-document-list) 
* [User View Improvements in the Resource Planner](#user-view-improvements-in-the-resource-planner) 
* [New Project List Experience](#new-project-list-experience) 
* [New Look for Updates Tab](#new-look-for-updates-tab) 
* [Mobile Improvements](#mobile-improvements)

## Modify Task Dates in the Gantt Chart {#modify-task-dates-in-the-gantt-chart}

You can now drag the task bubble to change the Planned Start and Planned Completion Dates in the Gantt chart. With this change, you can apply what-if scenarios to your project without impacting the timeline.

Prior to this change, you could change task dates only in the task list or at the task level.

For more information, see [Update information in the task list Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Access the Project Gantt Chart from the Updates Tab {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>This functionality has been temporarily removed from the Preview environment.

You can now access the new project Gantt chart from the Updates tab. When a user changes the Commit Date of a task in a way that affects the project timeline, you can view the impact in the project Gantt chart.

Prior to this change, the Project Timeline link opened the Legacy Gantt Chart.

For more information, see [Commit Date overview](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

For more information, see [Portfolio Optimizer overview](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Various Links Re-Introduced to Documents on the Document List {#various-links-re-introduced-to-documents-on-the-document-list}

In the 18.1 release, various links were removed from documents on the document list and moved to other areas of the interface (some as a button next to the document name and some in a drop-down menu on the button). The following links are being re-introduced below the document name with this release, and are now available on individual documents within the document list:

* Generate Proof (available when a proof is not yet generated)
* Open Proof (available when a proof is generated)
* Document Details (available when a proof is not yet generated)
* Proof Details (available when a proof is generated)
* Print Summary

The following actions are not being re-introduced as links on the document within the document list:

* Share (still available as a button in the menu)
* Check Out / Check In (still available in the More drop-down menu in the menu)

For more information, see the following sections:

* &nbsp;in&nbsp;

## User View Improvements in the Resource Planner {#user-view-improvements-in-the-resource-planner}

The User View of the Resource Planner now contains the following improvements:

* The User View is now the default view, replacing the Project View.
* Improved filters which pull information from the entire database, rather than just the information on the screen.
* Full-screen mode.
* Performance is now faster and more efficient.

   * New limits for the number of users, projects, roles, and tasks you can display.
   * Lazy loading, for faster loading of users.

The following functionality has been temporarily disabled in the Resource Planner:

* Exporting the data from the Resource Planner when using the User View.

Prior to these improvements, you have reported that the Resource Planner was slow to load and that you had noticed incongruences in the data displayed. With these improvements, these should now be eliminated.

For more information about the areas of the Resource Planner, see [Resource Planner navigation overview](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## New Project List Experience {#new-project-list-experience}

A new experience is now available when viewing a list of projects. This experience includes increased performance and smoother and faster list navigation. Only the lists in the Projects tab of the Projects area of Workfront have been updated to this new experience.

For the most part, the changes are in the speed and efficiency of the list. The following visible changes have also been introduced:

* The list displays up to 2,000 items by default.

  Prior to this enhancement, the list displayed 100 items.

* Groupings are collapsed by default.

  Prior to this change, groupings were expanded by default.

* The area for selecting a row has expanded to the entire row.

The following features have been temporarily disabled in the specified lists of projects:

* Column resizing (This functionality was reintroduced in the 2018.2 Beta 5 release)
* Column reordering
* Status icon fields display as blank (This functionality was reintroduced in the 2018.2 Beta 5 release)
* The Gantt chart is not accessible (This functionality was reintroduced in the 2018.2 Beta 3 release.)

For more information about working in lists, see [Get started with lists in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## New Look for Updates Tab {#new-look-for-updates-tab}

>[!NOTE]
>
>For some users, the new Updates tab might not display in the Preview environment. Our development team is currently troubleshooting the issue and working to resolve the problem as soon as possible.

The look and feel of the Updates tab has changed to be more aligned with other areas of the interface. This change applies to projects, tasks, issues, and documents.

The following table shows the updates made to the Updates tab: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Task</strong> </p> </th> 
   <th> <p><strong>Previous user action</strong> </p> </th> 
   <th> <p><strong>New user action</strong> </p> </th> 
   <th> <p><strong>For more information, see…</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Logging time on a timesheet</p> </td> 
   <td> <p>Click the Log Time link</p> </td> 
   <td> <p>Click the Log Time Button</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtering out system updates on the Updates tab</p> </td> 
   <td> <p>Click the Filter System Updates link</p> </td> 
   <td> <p>Disable the Show Activity Log toggle</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Viewing system updates on the Updates tab</p> </td> 
   <td> <p>Click Show All Updates</p> </td> 
   <td> <p>Enable the Show Activity Log toggle</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tagging other users on an update or comment</p> </td> 
   <td> <p>Click the Include others on this update icon</p> </td> 
   <td> <p>Add users and teams in the Notify field</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allow only users within your company to view an object</p> </td> 
   <td> <p>Click the Lock icon</p> </td> 
   <td> <p>Enable the Private to My Company toggle</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allow users outside your company to view an object</p> </td> 
   <td> <p>Click the Lock icon</p> </td> 
   <td> <p>Disable the Private to My Company toggle</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add a reply or update to a comment or update</p> </td> 
   <td> <p>Click the Comment button</p> </td> 
   <td> <p>Click the Reply or Update button</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a> </p> <p>&nbsp;</p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Add an update to a document</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mobile Improvements {#mobile-improvements}

The mobile app contains the following enhancements:

* Links that are shared with you in other mobile applications now open in the Workfront mobile app.

  For more information about sharing links, see .

  This update will be released to iOS sometimes this week, and the Android update should follow shortly after.

* We have updated our support requirements for the iOS platform to support iPhone X.

  For more information about supported mobile devices and operating systems, see the .
