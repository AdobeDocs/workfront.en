---
filename: system-project-statuses
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
---



# System project statuses {#system-project-statuses}

*`Workfront`* has 9 built-in system project statuses.


The first 3 in the table below are required, which means that you can unlock, rename, and reorder them, but you cannot hide or delete them.


Changing a project status is typically a manual process. However, there are some scenarios outlined in the following list when a project status is changed automatically, depending on other factors that are happening in the system.


The following project statuses are provided with your *`Workfront`* instance:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 </col> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">System project status</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">This project status occurs when</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">What happens in this status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planning (required status)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>The project manager is planning the timeline of the project, the assignment of the tasks, and the approvals. The project manager sets this status on a project manually.</p> <p>Tip: We recommend that you set the default status for new projects in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to Planning. As a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>, you can change the default status for all your new projects in the Projects area of Project Preferences.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Users on the project team can see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project do not populate their Work List. Only approvals and accepted work items display in the Home Work List.</p> <p>No notifications are sent while a project has this status.</p> <p>We recommend that all the changes that can trigger an update to the timeline of the project, or any changes to tasks and issue assignments, are made while the project is in the Planning status. This minimizes the amount of notifications users receive.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Current (required status)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Users are working on it. The project manager should turn a project to Current to signal that it has started.</p> <p>This is the default status for new projects in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> <p>Tip: As a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>, you can change the default status for new projects in the Projects area of Project Preferences. For more information, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Users on the project team can see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project populate their Work List. They can start accepting work on tasks and issues and move them to their Working On list.</p> <p>Also, on a Current project, all notifications about timeline changes, assignments, actions needed, and approvals are sent to users on the project team.</p> <p>And the timeline of the project is calculated automatically by the system, if the Update Type of the project is set to Automatic, On Change, or Automatic and On Change.</p> <p>Tip: It's a good idea to keep project plan adjustments to a minimum when a project is in this status so that users don't receive too many notifications.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Complete (required status)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> The project is completed:</p> 
    <ul> 
     <li> <p>If the Completion Mode of the project is set to Manual, the project manager chooses this status manually to inform users on the project team to stop working on the project.</p> </li> 
    </ul> 
    <ul> 
     <li>If the Completion Mode of the project is set to Automatic, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> automatically marks a project as Complete when all the tasks and issues in the project are marked as Complete. </li> 
    </ul> <p>Important: You can mark a project as Complete only when all the tasks, issues, and approvals on the project are resolved.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><![CDATA[
           ]]>
    <ul>
     <li>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project do not populate their Work Requests or Working On lists.</li>
     <li>All the notifications related to the project, except for a status change notification, stop being sent to the users on the project team. </li>
     <li>The timeline of the project is not calculated anymore by the system.</li>
     <li>The project cannot be copied.</li>
    </ul><p>You can prevent users from performing additional actions when a project is marked as Complete. </p><p>For more information about how to restrict actions on projects that are marked as Complete, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Dead</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">The project has not finished yet, but due to roadblocks, or scope change, the project cannot continue to be worked on and has been abandoned. The project manager changes the status to Dead to alert the users on the project team that this project will never finish and they should not be working on it anymore.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project disappear from their Work List.</p> <p>Approval decisions cannot be granted to tasks or issues.</p> <p>Notifications about timeline changes, assignments, actions needed, approvals are not sent to users on the project team.</p> <p>The timeline of the project is not calculated automatically by the system, as the project is perceived as being completed.</p> <p>You can prevent users from performing certain actions when a project is marked as Dead. For more information about how to restrict actions on Dead projects, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">On Hold</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">The project has not finished yet, but due to some delays, the project needs to be temporarily suspended. The project manager chooses to use this status to alert users in the project team to stop working on the project, at the current time.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project disappear from their Work List. </p> <p>Approval decisions cannot be granted to tasks or issues.</p> <p>Notifications about timeline changes, assignments, actions needed, approvals are not sent to users on the project team.</p> <p> <p>Note:  When you place a project On Hold, the timeline of the project does not stop. The project can still show as At Risk or In Trouble even if no one is actively working on the project. Some manual adjustments of the dates of the remaining open tasks might be needed when turning the project back to Current again, so that the project can show updated progress.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requested</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">The project status is automatically marked as Requested by the system, when the business case on a project request has been completed and submitted for approval. For more information about requesting a project using a business case, see <a href="review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues on the project that are assigned to them do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Approved</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">The project status is automatically marked as Approved, when the business case on a project request has been approved. For more information about requesting a project using a business case, see <a href="review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Users on the project team can see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Rejected</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">The project status is automatically marked as Rejected, when the business case on a project request has been rejected. For more information about requesting a project using a business case, see <a href="review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Idea</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">The project status is automatically marked as Idea when you submit a project request. For more information about requesting a project using a business case, see <a href="review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The tasks and issues that are assigned to them on the project do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
 </tbody> 
</table>



>[!NOTE]
>
>The following project statuses cannot be changed to a Dead, On Hold, or Complete status:>
>
>
>* Requested
>* Idea
>* Approved
>* Rejected (or its equivalent)
>
>



