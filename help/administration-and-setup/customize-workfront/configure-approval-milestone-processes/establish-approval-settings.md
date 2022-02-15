---
filename: establish-approval-settings
title: Establish approval settings
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
---



# Configure global approval settings {#configure-global-approval-settings}

As an *`Adobe Workfront administrator`*, you can determine the global settings for approval processes in *`Workfront`*. These settings impact all work item approval processes in your system.


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>



## Configure global approval settings {#configure-global-approval-settings-1}




1. Log in to *`Workfront`* as a *`Workfront administrator`* . 

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `Processes` > `Approvals`.  

1. Click `Settings` in the upper-right corner of the Approvals page.  

1.  In the `Approval Settings` box that appears, specify the following information:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Add &lt;number&gt; Days to planned completion date to accommodate for approval processes</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the number of minutes, hours, days, weeks, or months to add time to the planned completion date of the task that needs approval. Select "Elapsed" minutes, hours, days, or weeks to add time that includes any weekends,&nbsp;holidays, and non-working hours&nbsp;that have been designated in the system work schedule calendar.</p> <p>For example, if a task is assigned on Friday and&nbsp;has a duration of 3 elapsed days, the task completion date is set for&nbsp;Monday (assuming that Saturday and Sunday is a weekend). If the task has a duration of 3 days (not elapsed), the&nbsp;task completion date is set for Wednesday.<br><p>Note: &nbsp;Enabling the addition of extra time to accommodate&nbsp;for approval on tasks will affect the timeline of the task and that of the project.</p></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Approver not required to be on the project team (for approval processes that include a role)</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select this if an approver is not required to be on the project team when an approval process includes a role. When assigning the approval decision to a job role, only the users who have a role associated with them on the project will see the approval. If you enable this setting, any user with that job role receives the approval request whether they are on the project team or not. For information about editing a user's project role, see <a href="manage-project-team.md" class="MCXref xref">Manage the Project Team</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Disable approval delegation</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select this option to disable the functionality for users in your system to delegate approvals to another user. When this option is selected, the option to delegate approvals is removed from <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, and any existing approval delegations are stopped.</p> <p>For more information about delegating approvals in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see<a href="delegate-approval-requests.md" class="MCXref xref">Delegate approval request</a> .</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Allow Editing the custom form when the project, task, or issue is in pending approval status</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select this option&nbsp;to&nbsp;allow users to edit the custom form of projects, tasks, and issues when in the Pending Approval status. This is the default setting.<br></p> <p>When this option is selected:</p> 
    <ul> 
     <li>All approvers (and any other users who have access to edit the custom form) can make changes to the custom form when the object is pending approval, regardless of the current approval path or approval step.</li> 
     <li>Changes that are made to the custom form during an approval process do not affect any approval decisions that were made prior to the change.</li> 
     <li> <p>Any changes made to the project, task, or issue are tracked in the same way, regardless of this setting. <br></p> <p>For example, if you added custom form fields to be tracked on the update stream, any changes to the form are tracked on the update stream on the object.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Allow users to recall newly created requests pending approval</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Select this option to configure whether users can recall an issue or a request pending approval for their first status.&nbsp;You can associate the first status of an issue or a request with an approval process by configuring requests queues. <br></p> <p>For more information about request queues, see <a href="create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.</p> <p>Do one of the following:</p> 
    <ul> 
     <li>Select this option to allow users to recall an approval for the first status of an issue or a request. In this case, they can see a <span class="bold">Recall</span> button on a new issue or request which is pending approval status. When they select to recall the issue, they will receive a warning that the issue will also be deleted. The issue is deleted after they have confirmed their recalling it.&nbsp;</li> 
     <li> <p>Deselect this option to prevent users from recalling an issue or a request whose first status is pending approval. They cannot see a <span class="bold">Recall</span> button on the new issue or request and the approval must be granted. This is the default option.</p> <p>For more information about reviewing items waiting for approval, see <a href="view-approvals.md" class="MCXref xref">View approvals </a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save Changes.`&nbsp;


