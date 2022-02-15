---
filename: view-all-updates-in-a-report
product-area: projects
navigation-topic: update-work-items-and-view-updates
---



# View all updates in a Note report {#view-all-updates-in-a-note-report}

The Updates `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area </MadCap:conditionalText>`of an object displays a maximum number of 200 updates by default.&nbsp;To see all the updates that any of the users have entered for an object, you can create a Note report that displays all the updates.




>[!NOTE]
>
>You can build a report to view updates on objects in Preview with the Journal entry report. For more information, see [Report on the Updates area](create-journal-entry-report.md). 





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level.<br>For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View</p> <p>Note: If you do not have View permission or higher to an object, information for that object does not display in the report.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a Note report {#create-a-note-report}

Creating a report for Notes for any object is identical, regardless of the object.


For example, to create a Note report for all the notes on a project:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1. Click  `Reports`.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> C</MadCap:conditionalText>`lick `New Report`, then choose  `Note`.

1. (Optional) Click `Views`, then `Add Column` to add the `Name` of the `Project` in the view of the report.&nbsp;

1. (Optional) Click `Groupings`, then `Add Grouping` to group by the `Project Name`, if you are reporting on multiple projects at the same time.  
   This ensures that the notes are grouped by their respective projects, making the report easier to read.&nbsp;

1. (Optional) Click `Filters,`then  `Add a Filter Rule`to filter for just one project, or specific projects.

1. (Conditional and optional) Set the `Project Name` as  `Equal` to the project name of the project you want to view updates for.&nbsp;&nbsp;  

1. Click `Save + Close`.  
   All the updates entered on the project by all users with permissions to at least View the project are displayed in the report.  



