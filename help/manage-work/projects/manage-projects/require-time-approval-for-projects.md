---
filename: require-time-approval-for-projects
product-area: projects
navigation-topic: manage-projects
---



# Require time to be approved for a project {#require-time-to-be-approved-for-a-project}

You can configure the project to require that the hours logged against the project are approved by the Project Owner. When configured in this way, hours must be first approved by the Project Owner before they can be eligible to be used on a billing record.   
For more information about billing records, see the article [Create billing records](create-billing-records.md).


>[!NOTE]
>
>Enabling this option does not remove a timesheet approver's ability to approve time on the timesheet. If the Project Owner doesn't approve or reject time, a timesheet approver can&nbsp;still approve the time on a timesheet. &nbsp;




## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects or higher</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>View permissions to the project or higher</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Additional access</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours.&nbsp;In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Require time to be approved for a project {#require-time-to-be-approved-for-a-project-1}

To require project manager approval for hours on the project:



1. Go to the project where you want to require approval for hours.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">More</span> icon  <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <span class="bold">Edit</span>.</MadCap:conditionalText>`  
   The Edit Project dialog box displays.

1.  In the `Project Settings` section, select `Require time to be approved for this project`. 
1. Click `Save`.  
   Now when time is logged and approved, those hours become locked and cannot be altered by the user who entered them on the project or the timesheet. Only a *`Workfront administrator`* can adjust the time recorded.





## Approve and reject time on a&nbsp;project {#approve-and-reject-time-on-a-project}

As a project manager, you can approve or reject hours that are logged for tasks, issues, or the project. 


Approving the hours at the project level does not have any impact on the timesheet of any of the users who logged the hours. For example, the hours in the project may be approved by the project manager, but the timesheet is still yet to be approved by the manager of the user or the timesheet approver.&nbsp; 


If you set up a project to require approval on the hours logged, the project manager must approve the hours in order for them to be available to be included in a billing record for the project. For more information about creating billing records, see the article [Create billing records](create-billing-records.md).


To approve or reject hours on a project: 



1. Go to the project.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Hours</span> area in the left panel.&nbsp;This might be located under the  <span class="bold">Show More</span> area. </MadCap:conditionalText>`  

1. The hours logged for issues, tasks, and the project display and should have a status of `Submitted`.  
   Click the box to the left of the hour entries to select the hours you want to approve.

1. Click `Approve`.  
   The status of the hours changes to `Approved`.  
   If you later reject the approved hours, the status of the hours changes to `Not Approved`.  
   When you include the approved hours in a billing record, the status of the hours changes to `Billed and Approved`. Hours added to a billing record cannot be deleted. For more information about creating billing records, see the article [Create billing records](create-billing-records.md)

1. (Optional) Click `Reject` to reject the time entries on the project.  
   The status of the hours changes to `Rejected`.



