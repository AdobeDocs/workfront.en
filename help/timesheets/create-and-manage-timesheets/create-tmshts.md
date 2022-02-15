---
filename: create-tmshts
product-area: timesheets
navigation-topic: create-and-manage-timesheets
---



# Create a single-use timesheet {#create-a-single-use-timesheet}

You can manually create a single-use&nbsp;timesheet if you want a timesheet that is not recurring.&nbsp;When the end date of the timesheet is reached and you need more timesheets are needed, you must create new ones.


For information about creating a timesheet profile that generates recurring timesheets for your users without any further intervention from you (recommended), see [Create, edit, and assign timesheet profiles](create-timesheet-profiles.md).


>[!NOTE]
>
>
>
>
>*  Single-use timesheets cannot be created for groups. 
>*  When creating a single-use timesheet, you cannot specify&nbsp;specific general hour types to include in your timesheet. All general hour types that are activated in your system display in timesheets created manually. 
>
>
>  If you want to select only certain general hour types to display in your timesheets, use a timesheet profile.&nbsp;For more information about timesheet profiles, see [Create, edit, and assign timesheet profiles](create-timesheet-profiles.md).
>
>
>





## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have administrative access to timesheets. For more information, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a single-use timesheet {#create-a-single-use-timesheet-1}

To create a single-use timesheet:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1. Click `Timesheets`.
1. Click `All Timesheets` in the left panel.
1.  Click `New Timesheet`.
1.  Specify the following information:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Create timesheet for</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Start entering the name of the user for whom you are creating the timesheet, and click it when it appears&nbsp;in the list.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Start Date</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">This is the start date of the timesheet.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">End Date</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> This is the end date of the timesheet.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Approvers</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.<br>Start entering the names of the timesheet approvers and click them when they appear&nbsp;in the list.<br>You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <span class="bold">Closed</span> and it disappears from the timesheet approvals list of all the remaining approvers.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Can edit time</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <li> Select this option if you want to allow approvers to edit hours on the timesheet.&nbsp;</li> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">You can choose to hide the Overtime box on the timesheet. This option is disabled by default.</td> 
  </tr> 
 </tbody> 
</table>


1. Click `Create Timesheet`.




## When tasks and issues appear on users' timesheets {#when-tasks-and-issues-appear-on-users-timesheets}

A task or issue assigned to a user automatically appears on the timesheet of a user if the task or issue meets any of the following criteria:



* The user&nbsp;has logged hours on the task or issue
* The planned dates of the task or issue fall within the dates of timesheet
* The task or issue has an Actual Start Date (The task or issue status is In Progress)
* The task or issue is pinned to the timesheet
* The Planned Completion date falls within the date range of the timesheet and the status is In Progress


If the "Pre-populate timesheets..." preferences (located in the Timesheets & Hour preferences) are&nbsp;deselected, the timesheet shows issues and tasks which have a status of In Progress. For more information about the Timesheets & Hour preferences, see [Configure timesheet and hour preferences](timesheet-and-hour-preferences.md)
