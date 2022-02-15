---
filename: task-finances-in-details
product-area: projects
navigation-topic: manage-tasks
---



# Manage task finances in the Task Details `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>` {#manage-task-finances-in-the-task-details-section}

You can view or edit the financial information of a task by accessing the Overview area of the Task&nbsp;Details `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`. There is a limited number of fields that you can view or edit in this area. For information about editing all financial information for a task see [Edit tasks](edit-tasks.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" style="width: 344px;"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects and Tasks</p> <p>View access to&nbsp;Financial&nbsp;Data or higher</p> <p>You must have Edit access to&nbsp;Financial Data to edit financial information on tasks</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View permissions to the task that include View Finance or higher</p> <p>You must have Manage permissions on the task that include Edit Finance to edit financial information on tasks</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Edit task finances in the Task Details section {#edit-task-finances-in-the-task-details-section}




1.  Go to a project where you want to view a task.


   >[!NOTE]
   >
   >To find a task, you can also search for it, and click the name to access the task. For more information on searching for objects in *`Workfront`*, see [Search Adobe Workfront](search-workfront.md).



1.  Click `Tasks` in the left panel. 
1. Click the name of a task that you want to view.
1. Click `Task Details`.
1.  (Optional) Click the `Collapse all` icon in the top right of the Task Details page. 


   ![](assets/collapse-all-icon-on-details-page.png)   



   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* or *`Group administrator`* sets up our Layout Template, the fields in the Task Details section might be rearranged or not display. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md).



1.  Click `Finance` to expand and view the financial information for the task. 


   Click the `Edit` icon ![](assets/edit-icon.png) in the upper-right corner of the Details section, then click  `Finance`. 

1.   Edit any field that is available for editing, by single-clicking the field or click `+Add` to add information to an empty field.
1.  Review or edit the following information `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> in the  <span class="bold">Finance</span> area</MadCap:conditionalText>`: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Cost Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the Cost Type for the task. This is going to determine how the cost of the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p>No Cost</p> </li> 
     <li> <p>Fixed Hourly </p> </li> 
     <li> <p> User Hourly </p> </li> 
     <li> <p> Role Hourly</p> </li> 
    </ul> <p>For more information about tracking costs, see <a href="track-costs.md" class="MCXref xref">Track costs</a> . Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> selects the default Cost Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> .</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Revenue Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Specify the Revenue Type for the task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p> Not Billable </p> </li> 
     <li> <p>User Hourly </p> </li> 
     <li> <p>Role Hourly </p> </li> 
     <li> <p>Fixed Hourly </p> </li> 
     <li> <p>User Hourly w/Cap </p> </li> 
     <li> <p>Role Hourly w/Cap </p> </li> 
     <li> <p>User Hourly Plus Fixed </p> </li> 
     <li> <p>Role Hourly Plus Fixed </p> </li> 
     <li> <p>Fixed Revenue </p> </li> 
    </ul> <p>For more information about tracking revenue, see<a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a> . </p> <p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> or <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> selects the default Revenue Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Planned Cost</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is a calculation that shows the cost of the task based on the planned hours, the cost type, and the hourly rate for users or job roles. For more information about tracking costs, see <a href="track-costs.md" class="MCXref xref">Track costs</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Actual&nbsp;Cost</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> This is a calculation that shows the cost of the task based on the actual hours, the cost type, and the hourly rate for users or job roles. For more information about tracking costs, see <a href="track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Planned Revenue</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is a calculation that shows the revenue associated with the task based on the planned hours, the revenue type, and the hourly rate for users or job roles. For more information about tracking costs, see <a href="track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Actual&nbsp;Revenue</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This is a calculation that shows the revenue associated with the task based on the actual hours, the revenue type, and the hourly rate for users or job roles. For more information about tracking costs, see <a href="track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">CPI/SPI/CSI</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>These are task performance metrics that show how your task is performing, at a given time. Their values are calculated based on the Performance Index Method of the project.<br>For more information see the following articles:</p> 
    <ul> 
     <li> <p><a href="calculate-cpi.md" class="MCXref xref">Calculate Cost Performance Index (CPI)</a> </p> </li> 
     <li> <p><a href="calculate-spi.md" class="MCXref xref">Calculate Schedule Performance Index (SPI) </a> </p> </li> 
     <li> <p> <p><a href="calculate-csi.md" class="MCXref xref">Calculate Cost Schedule Performance Index (CSI)</a> </p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Estimate at Completion (EAC)</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>This is a calculation that shows the total cost of your task, at completion. For more information about estimate at completion, see <a href="calculate-eac.md" class="MCXref xref">Calculate Estimate At Completion (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Conditional) If you are editing the fields in the Finance section, click `Save` `Changes`. 


