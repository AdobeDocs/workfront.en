---
filename: edit-an-approval-process
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
---



# Edit an approval process {#edit-an-approval-process}

If you are an *`Adobe Workfront administrator`*, or you have administrative access to approval processes, you can see and edit all approval processes in the system.


If you are a *`group administrator`*, you can see and edit the approval processes associated with the group or groups you manage.


For information about creating approval processes, see [Create an approval process](create-approval-processes.md).


>[!NOTE]
>
>
>
>
>* When you edit a global approval process that is already in use, your changes affect all objects throughout the system that are already associated with it.
>*  If you add a new approver to the current stage on an approval process that has already started on an object, the process for that object resets and the approvers have to start over.
>
>
>  However, if you make the following changes in an approval process that has already started on an object, that process continues without interruption:
>
>    
>    
>    * Add a stage beyond the current stage
>    * Add an additional approver before the current stage
>    
>    
>
>
>






## Access requirements {#access-requirements}

You must have the following:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Administrative access to Approval Processes if you are not a System Administrator</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Edit an existing approval process {#edit-an-existing-approval-process}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Processes` > `Approvals`.

1. Click the `Project Approvals`, `Task Approvals`, or `Issue Approvals` tab, depending on the type of approval process you want to edit.

1.  Click the name of the approval process you want to edit.
1.  Specify the following information in the box that displays:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Approval process name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a descriptive name for the approval process. Users see this name when applying the approval process to an object, as described in <a href="associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Type a description of the approval process. This displays in the <span class="bold">Approvals</span> section in the <span class="bold">Setup</span> area next to the name of the approval process.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Is Active</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select this check box if you want other users to be able to attach the approval process to projects, tasks, and issues that they create. </p> <p>This option is enabled by default.</p> <p>Tip: Marking an approval process as inactive is useful when your organization no longer needs to use it, but you want to preserve historical information about its use.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">This approval process can be used by </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>If you want the approval process available for projects, tasks, issues, and templates belonging only to a particular group, start typing the name of the group, then select the name when it appears:</p> 
    <ul> 
     <li>If you are a system administrator or you have administrative access to approval processes, you can see any group in the system when you type its name. <span class="bold">All groups</span> is selected by default. </li> 
     <li>If you are a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>, you can see any group you manage when you type its name. The <span class="bold">All Groups</span> option is not available.</li> 
    </ul> <p>This option is not available for single-use approval processes.</p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>When you make changes to the group-specific approval process, the existing approval processes that have already been associated with work items might change. For information about these changes, see <a href="how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>.</p> <p>For information about listing and managing your group’s approval processes from your group’s page, see <a href="create-and-modify-groups-approval-processes.md" class="MCXref xref">Group-level approval processes</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Configure a path for the approval process using the following options.


   A path is where you specify what needs to happen in the approval process. You create stages in a path to indicate who needs to do the approval work and in what order.

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Start Approval Process when the status is set to</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the status that will trigger the approval process on work items. When someone updates a work item to this status, its approval process begins.<br>The same status cannot be selected for multiple approval process paths.<br></p> <p>The statuses available are based on what is selected under the option <span class="bold">This approval can be used by</span> (explained in the table above):</p> 
    <ul> 
     <li> If All groups is selected, only system-wide locked statuses are available</li> 
     <li> <p>If a specific group is selected, only the statuses available for that group are available</p> </li> 
    </ul> <p>For information about how approval process work with statuses, see the section <a href="approval-process-in-workfront.md#how2" class="MCXref xref">How approval processes rely on statuses</a> in the article <a href="approval-process-in-workfront.md" class="MCXref xref">Approval process overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Stage Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">(Optional) Type a name describing the first stage of the path. If you do not specify a stage name, the default name is <span class="bold">Stage 1</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Approvers</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Begin typing the name of the user, team, or job role that you want to designate as an approver for this stage, then click the name when it appears in the drop-down list. You can add only active users, <span>job roles</span>, and teams. </p> <p>Note: Adding a user, team, or role as an approver does not automatically give them permissions to the object associated with that approval. They receive permissions to the object when the approval step is triggered. Otherwise, the objects must be shared with them before they can make an approval decision. </p> <p>You can also designate an individual as an approver by specifying the individual's role. For example, you can assign a Project Owner, Project Sponsor, Portfolio Owner, Program Owner, or Manager as an approver. These options automatically appear when you begin typing.</p> <p>Important: When you assign an approval to the Project Sponsor and no one is designated as the sponsor of a project, the approval is assigned to the Project Owner, by default. If no one is designated as the owner of the project, the approval is assigned to the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. <br></p> <p> <img src="assets/approval-create-addusers-350x528.png" alt="approval_create_addusers.png" style="width: 350;height: 528;"> <br> </p> <p>You can repeat this process to add multiple approvers to the stage. A single stage can include a combination of users, teams, and job roles as approvers. There is no limit to the number of approvers you can add to a stage.</p> <p>Important:  <p>When you assign job roles as approvers, all users associated with that job role that are also on the project team can see the pending approval process in their Approvals area. As soon as one of the users approves or rejects the item, the approval process is no longer listed on their Approvals area.<br></p> <p>When you assign a team as an approver, all users in that team can see the pending approval process in their Approvals area. As soon as one of the users on the team approves or rejects the item, the approval process is no longer listed on the Approvals area.<br></p> <p>For more information about the project team, see <a href="project-team-overview.md" class="MCXref xref">Project Team overview</a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Only one decision required</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Displays only if you add multiple approvers to the stage) Select this option if any one of the approvers on the stage can approve or reject the work item during this stage. This action allows the work item to leave the stage. </p> <p>When this option is not selected, all of the identified approvers must approve or reject the stage (in any order) before the item leaves the stage. If any one of the approvers rejects the stage, the process interrupts and starts over so that the required changes can be made. Then the approvers can approve or reject the stage once again.<br></p> <p>When a team is designated as an approver, any member of the team can grant or reject a stage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Add Stage</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">(Optional) Add another a stage to the path, using the options explained in the three rows above. You can add as many stages to the path as you need.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">If Rejected</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select the action you want to take if the work item is rejected at any stage of the path:</p> 
    <ul> 
     <li><span class="bold">Create an issue</span>: (Available only for project and task approval processes) An issue is created in the project or task where the approval process is running. The default assigned resource on the task, or the owner of the project is assigned to the issue. By default, the name of the issue created is <span class="bold">Approval Rejected (&lt;Project or Task Name&gt;)</span>. This is a Rejection Issue, entered under the task or the project, depending on the approval process where the rejection happened.</li> 
     <li> <p><span class="bold">Set Status to</span>: Choose one of the following:</p> 
      <ul> 
       <li><span class="bold">Previous status</span>: The rejected project, task, or issue reverts to the status prior to the status that activates the approval process.</li> 
       <li> <p>Any other status in the list: The rejected object moves to the status you choose, such as On Hold. You can choose one of the default statuses or a custom statuses you added to your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system.</p> 
        <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
         <span class="autonumber"><span><b>Tip: </b></span></span> 
         <p>If you select a status associated with an approval process as the rejection status, the rejected object moves to the selected status bypassing the approval process for the rejection status.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Example: </b></span></span> 
          <p> For example, if you select On Hold for the rejection status and the On&nbsp;Hold status is associated with an approval process, the rejected object is placed in the On&nbsp;Hold status without requiring the approval. </p> 
         </div> 
        </div> <p>For a system-wide approval process, only system-wide locked statuses are available.</p> <p>For a group-specific approval process, all group statuses are available. This includes any custom statuses that the <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> created specifically for the group, as well as any system-wide statuses. </p> <p>For information about how approval process work with statuses, see the section <a href="approval-process-in-workfront.md#how2" class="MCXref xref">How approval processes rely on statuses</a> in the article <a href="approval-process-in-workfront.md" class="MCXref xref">Approval process overview</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1. (Optional) Click `Add Path` to add another path to the approval process, referring to the list of options in the previous step. 
1. The new path must be associated with another status. The path triggers when the item is updated to show this status. You cannot have two paths for the same status.
1. Click `Save`.
1.  (Optional) Do any of the following:

    
    
    * Associate the approval process with specific projects, tasks, or issues throughout your system, as described in [Associate a new or existing approval process with work](associate-approval-with-work.md).
    *  Outside of *`Workfront`*, notify users that the approval process is available for them to associate with their projects, tasks, or issues, as described in [Associate a new or existing approval process with work](associate-approval-with-work.md).
    *  Create another approval process that is triggered if this approval process is rejected and the item takes on another status. This gives you a way to link approval processes together.
    
    



