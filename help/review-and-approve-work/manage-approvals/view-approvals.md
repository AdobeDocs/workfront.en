---
filename: view-approvals
product-area: projects
navigation-topic: approvals
---



# View approvals  {#view-approvals}

Approval processes provide the flexibility to create multi-step approvals for projects, tasks, and issues. Approval processes are defined by *`Adobe Workfront`* administrators to provide consistency throughout the system. 


For information about creating approval processes, see [Create an approval process](create-approval-processes.md). 


For information about associating approvals with work in *`Workfront`*, see [Associate a new or existing approval process with work](associate-approval-with-work.md). 



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to the objects associated with approvals</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View or higher permissions to the objects associated with approvals</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.



## Locate approvals in *`Adobe Workfront`* {#locate-approvals-in-adobe-workfront}

You can view or manage approvals from several areas of *`Workfront`*. For information about how to manage approvals in various areas, see [Approving work](approving-work.md). 


You can view or manage approvals from the following areas:



*  In the Home area  
  All projects, tasks,&nbsp;issues, timesheets,&nbsp;documents, and access awaiting your approval are displayed in the Home area when you select to view All or Approvals.


  Approvals that you submitted yourself also display in the Home area, in the Approvals I've Submitted section of the Work List.   
  Approvals&nbsp;are removed from the Home area when the associated&nbsp;project, task, or issue&nbsp;is marked&nbsp;Resolved, On Hold, Closed, or Canceled. 


  For information about using Home, see [Get started with Home](get-started-with-home.md). 

*  In the header of a project, task, issue, document, or proof 
*  In the Approvals tab&nbsp;in a project, task, or issue
*  In a report


  >[!NOTE]
  >
  >You cannot make a decision on an approval from a report.


  You can create a report that contains approval information.


  For information about how to create a report, see [Create a custom report](create-custom-report.md).





##  



## View the approval status of an object {#view-the-approval-status-of-an-object}

You can view the approval status of an object in the following `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> sections </MadCap:conditionalText>`of the object:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Updates </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Displays all approval statuses when they occur. Approval statuses are displayed in line with other statuses displayed on the <span class="bold" style="font-weight: normal;">Updates</span> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
     </MadCap:conditionalText>in the object history.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Approvals</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Displays more detailed information about the approval process, such as each phase of the approval process and whether approvers have given their approval.</p> </td> 
  </tr> 
 </tbody> 
</table>




* [Use the Updates area to view an approval status](#using-the-updates-tab-to-view-approval-status) 
* [Use the Approvals area to view an approval status](#using-the-approvals-tab-to-view-approval-status) 




### Use the Updates area to view&nbsp;an approval status {#use-the-updates-area-to-view-an-approval-status}

When an approval is initiated on a project, task, or issue, a status is displayed on the `Updates` tab in the object history,&nbsp;indicating the approval status. A new status is displayed&nbsp;any time the object transitions through the approval process. This includes the following events:



* An approval process is initiated on an&nbsp;object (The approval process is initiated when the status is changed)
* The object is&nbsp;rejected
* The object&nbsp;is approved&nbsp;


If an approval is applied to a task, the approval updates are shown on the Updates tab of the task, not on the Updates tab of the project where the task resides.


### Use the Approvals area to view an approval status {#use-the-approvals-area-to-view-an-approval-status}

You can gain visibility into where a task or issue that you are working on currently is in&nbsp;the approval&nbsp;process. You can see the following information:



* The phase of the approval process
* Which approvers have already approved it
* Which approvers have not yet approved it


To see the current state of where a task or issue is in the approval process:



1. Go to the project, task, or issue that the approval is associated with.
1. In the left panel, click `Approvals`.  
   The Approvals tab displays&nbsp;the full information about all past approval paths and steps. You can see exactly who has made the approval if the approval was set for the team or job role.



