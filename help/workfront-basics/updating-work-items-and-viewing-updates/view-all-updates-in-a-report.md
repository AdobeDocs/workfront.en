---
filename: view-all-updates-in-a-report
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: View all updates in a Note report
description: The Updates area of an object displays a maximum number of 200 updates by default. To see all the updates that any of the users have entered for an object, you can create a Note report that displays all the updates.
---

# View all updates in a Note report

The Updates 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
area
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area </MadCap:conditionalText>`of an object displays a maximum number of 200 updates by default.&nbsp;To see all the updates that any of the users have entered for an object, you can create a Note report that displays all the updates.

>[!NOTE]
>
>You can build a report to view updates on objects in Preview with the Journal entry report. For more information, see [Report on the Updates area](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level.<br>For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p> <p>Note: If you do not have View permission or higher to an object, information for that object does not display in the report.</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create a Note report

Creating a report for Notes for any object is identical, regardless of the object.

For example, to create a Note report for all the notes on a project:

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Reports</span>.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Reports</span>.</li> 
 <li value="3"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    C
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   C
  </MadCap:conditionalText>lick <span class="bold">New Report</span>, then choose&nbsp;<span class="bold">Note</span>.</li> 
 <li value="4">(Optional) Click <span class="bold">Views</span>, then <span class="bold">Add Column</span> to add the <span class="bold">Name</span> of the <span class="bold">Project</span> in the view of the report.&nbsp;</li> 
 <li value="5">(Optional) Click <span class="bold">Groupings</span>, then <span class="bold">Add Grouping</span> to group by the <span class="bold">Project Name</span>, if you are reporting on multiple projects at the same time.<br>This ensures that the notes are grouped by their respective projects, making the report easier to read.&nbsp;</li> 
 <li value="6">(Optional) Click <span class="bold">Filters, </span>then&nbsp;<span class="bold">Add a Filter Rule </span>to filter for just one project, or specific projects.</li> 
 <li value="7">(Conditional and optional) Set the <span class="bold">Project&nbsp;Name</span> as&nbsp;<span class="bold">Equal</span> to the project name of the project you want to view updates for.&nbsp;&nbsp;<br></li> 
 <li value="8">Click <span class="bold">Save + Close</span>.<br>All the updates entered on the project by all users with permissions to at least View the project are displayed in the report.<br></li> 
</ol>

