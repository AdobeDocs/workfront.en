---
filename: updates-tab-overview
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
---



# Updates tab overview {#updates-tab-overview}

The Updates tab shows up to 200 of the most recent updates made within the past 90 days.&nbsp;You can reply to updates on the following objects:

<table style="width: 100%;"> 
 <col style="width: 259px;"> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Projects</li> 
     <li>Portfolios</li> 
     <li>Programs</li> 
     <li>Templates</li> 
     <li>Template Tasks</li> 
     <li>Tasks</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Issues</li> 
     <li>Iterations</li> 
     <li>Stories</li> 
     <li>Users</li> 
     <li>Documents</li> 
     <li>Timesheets</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Updates that also appear on higher-rank objects {#updates-that-also-appear-on-higher-rank-objects}

As shown in the following table, replies made to updates on certain objects also appear on the Updates tab of higher-ranked objects. 


For example, when you add an update to a task, the update appears on the Updates tab for the task and on the Updates tab for the project containing the task.

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Object where the original update was added</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Higher-ranked object where the original update also appears</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Project</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Project</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Program, Portfolio</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Document </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Object where document is attached, Project </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Program</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Portfolio</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Team</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Timesheet</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">User, Team</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Template Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Template</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Story</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Iteration, Team</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Iteration</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Team</td> 
  </tr> 
 </tbody> 
</table>



>[!NOTE]
>
>Replies added to system updates do not roll up to the parent object. Only direct replies on a child object and replies added to existing updates roll up to parent objects.


For informatics about the object hierarchy in *`Adobe Workfront`*, see [Understand objects in Adobe Workfront](understand-objects.md).


## Limitations of the Updates tab for users and teams {#limitations-of-the-updates-tab-for-users-and-teams}

You cannot make updates on teams. The Updates tab for teams is&nbsp;populated by updates entered on the following objects:



* Users
* Timesheets
* Stories
* Iterations


On the Updates tab for&nbsp;users and teams, you can view the updates that have been entered in the past 90 days.&nbsp;


If you want to see all the updates made on a user or a team, beyond the 90-day limit, you can build a report for notes. The report should not have a time filter that displays all updates made for users or teams. For more information, see [Create a custom report](create-custom-report.md).


## View system updates on work items with the Journal Entry report {#view-system-updates-on-work-items-with-the-journal-entry-report}

The Journal Entry report surfaces system updates from the Updates area of projects, tasks, and issues.


The report allows you to see:



*  How many status changes occurred
*  When a task or issue was deleted
*  How values in important custom fields changed over the course of a project
*  What important dates changed over the course of a project
*  If priority changed over the course of a project
*  If the owner of a project changed


For more information, see [Report on the Updates area](create-journal-entry-report.md).
