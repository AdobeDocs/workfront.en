---
filename: edit-an-approval-process
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Edit an approval process
description: If you are an Adobe Workfront administrator, or you have administrative access to approval processes, you can see and edit all approval processes in the system.
---

# Edit an approval process

If you are an Adobe Workfront administrator, or you have administrative access to approval processes, you can see and edit all approval processes in the system.

If you are a group administrator, you can see and edit the approval processes associated with the group or groups you manage.

For information about creating approval processes, see [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* When you edit a global approval process that is already in use, your changes affect all objects throughout the system that are already associated with it.
>* If you add a new approver to the current stage on an approval process that has already started on an object, the process for that object resets and the approvers have to start over.
>
>  However, if you make the following changes in an approval process that has already started on an object, that process continues without interruption:
>
>   * Add a stage beyond the current stage
>   * Add an additional approver before the current stage
>

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Approval Processes if you are not a System Administrator</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Edit an existing approval process

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. (Conditional) If you are editing a system-level approval process, click **Processes** > **Approvals** in the left panel.

   Or

   If you are editing a group-level approval process, do the following:

   1. In the left panel, click **Groups** ![](assets/groups-icon.png).
   
   1. Click the name of the group for which you want to list or manage group approval processes.
   1. In the left panel, click **Approvals**. You might need to click&nbsp;**Show More** first.

1. Click the **Project Approvals**, **Task Approvals**, or **Issue Approvals** tab, depending on the type of approval process you want to edit.

1. Click the name of the approval process you want to edit.
1. Specify the following information in the box that displays:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Approval process name</td> 
      <td>Type a descriptive name for the approval process. Users see this name when applying the approval process to an object, as described in <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type a description of the approval process. This displays in the <strong>Approvals</strong> section in the <strong>Setup</strong> area next to the name of the approval process.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong> </td> 
      <td> <p>Select this check box if you want other users to be able to attach the approval process to projects, tasks, and issues that they create. </p> <p>This option is enabled by default.</p> <p>Tip: Marking an approval process as inactive is useful when your organization no longer needs to use it, but you want to preserve historical information about its use.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">This approval process can be used by </td> 
      <td> <p>If you want the approval process available for projects, tasks, issues, and templates belonging only to a particular group, start typing the name of the group, then select the name when it appears:</p> 
       <ul> 
        <li>If you are a system administrator or you have administrative access to approval processes, you can see any group in the system when you type its name. <strong>All groups</strong> is selected by default. </li> 
        <li>If you are a group administrator, you can see any group you manage when you type its name. The <strong>All Groups</strong> option is not available.</li> 
       </ul> <p>This option is not available for single-use approval processes.</p> <p>Warning: When you make changes to the group-specific approval process, the existing approval processes that have already been associated with work items might change. For information about these changes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>.</p> <p>For information about listing and managing your group’s approval processes from your group’s page, see Create and modify a group’s approval processes in the new Adobe Workfront experience. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configure a path for the approval process using the following options.
1. A path is where you specify what needs to happen in the approval process. You create stages in a path to indicate who needs to do the approval work and in what order.
1. ```<col>``` ```<col>``` ```<tbody>  <tr>   <td role="rowheader">Start Approval Process when the status is set to</td>   <td> <p>Select the status that will trigger the approval process on work items. When someone updates a work item to this status, its approval process begins. </p> <p>The same status cannot be selected for multiple approval process paths.<br></p> <p>The statuses available are based on what is selected under the option <strong>This approval can be used by</strong> (explained in the table above):</p>    <ul>     <li> If All groups is selected, only system-wide locked statuses are available</li>     <li> <p>If a specific group is selected, only the statuses available for that group are available</p> </li>    </ul> <p>For information about how approval process work with statuses, see the section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">How approval processes rely on statuses</a> in the article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Approval process overview</a>.</p> </td>  </tr>  <tr>   <td role="rowheader">Stage Name</td>   <td>(Optional) Type a name describing the first stage of the path. If you do not specify a stage name, the default name is <strong>Stage 1</strong>.</td>  </tr>  <tr>   <td role="rowheader">Approvers</td>   <td> <p>Begin typing the name of the user, team, or job role that you want to designate as an approver for this stage, then click the name when it appears in the drop-down list. You can add only active users, <span>job roles</span>, and teams. </p> <note type="note">    Adding a user, team, or role as an approver does not automatically give them permissions to the object associated with that approval. They receive permissions to the object when the approval step is triggered. Otherwise, the objects must be shared with them before they can make an approval decision.    </note> <p>You can also designate an individual as an approver by specifying the individual's role. For example, you can assign a Project Owner, Project Sponsor, Portfolio Owner, Program Owner, or Manager as an approver. These options automatically appear when you begin typing.</p> <note type="important">     <ul>      <li> <p>When you assign an approval to the Project Sponsor and no one is designated as the sponsor of a project, the approval is reassigned to the Project Owner. If no one is designated as the owner of the project, the approval is assigned to the Workfront administrator. <br></p> </li>     </ul>     <ul>      <li> <p>When you assign an approval to a role and the <strong>Approver not required to be on the project team (for approval processes that include a role)</strong> is disabled but there are no roles in the project team that match the role on the approval, the approval is reassigned to the Project Owner. For information about approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>.</p> </li>     </ul>     <ul>      <li> <p>When you assign an approval to the Project Owner and no one is designated as the owner of a project, the approval is reassigned to the main Workfront administrator as indicated in the Customer Info section in the Setup area. For information, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configure basic information for your system</a>.&nbsp;&nbsp;<br></p> </li>     </ul>     <p> <img src="assets/approval-create-addusers.png" alt="approval_create_addusers.png"> </p>    </note> <p>You can repeat this process to add multiple approvers to the stage. A single stage can include a combination of users, teams, and job roles as approvers. There is no limit to the number of approvers you can add to a stage.</p> <note type="important">     <p>When you assign job roles as approvers, all users associated with that job role that are also on the project team can see the pending approval process in their Approvals area. As soon as one of the users approves or rejects the item, the approval process is no longer listed on their Approvals area.<br></p>     <p>When you assign a team as an approver, all users in that team can see the pending approval process in their Approvals area. As soon as one of the users on the team approves or rejects the item, the approval process is no longer listed on the Approvals area.<br></p>     <p>For more information about the project team, see <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Project Team overview</a>.</p>    </note> </td>  </tr>  <tr>   <td role="rowheader">Only one decision required</td>   <td> <p>(Displays only if you add multiple approvers to the stage) Select this option if any one of the approvers on the stage can approve or reject the work item during this stage. This action allows the work item to leave the stage. </p> <p>When this option is not selected, all of the identified approvers must approve or reject the stage (in any order) before the item leaves the stage. If any one of the approvers rejects the stage, the process interrupts and starts over so that the required changes can be made. Then the approvers can approve or reject the stage once again.</p> <p>When a team is designated as an approver, any member of the team can grant or reject a stage.</p> </td>  </tr>  <tr>   <td role="rowheader">Add Stage</td>   <td>(Optional) Add another a stage to the path, using the options explained in the three rows above. You can add as many stages to the path as you need.</td>  </tr>  <tr>   <td role="rowheader"> <p role="rowheader"><strong>If Rejected</strong> </p> </td>   <td> <p>Select the action you want to take if the work item is rejected at any stage of the path:</p>    <ul>     <li><strong>Create an Issue</strong>: (Available only for project and task approval processes) An issue is created in the project or task where the approval process is running. The default assigned resource on the task, or the owner of the project is assigned to the issue. By default, the name of the issue created is <strong>Approval Rejected (<Project or Task Name>)</strong>. This is a Rejection Issue, entered under the task or the project, depending on the approval process where the rejection happened.</li>     <li> <p><strong>Set Status to</strong>: Choose one of the following:</p>      <ul>       <li><strong>Previous Status</strong>: The rejected project, task, or issue reverts to the status prior to the status that activates the approval process.</li>       <li> <p>Any other status in the list: The rejected object moves to the status you choose, such as On Hold. You can choose one of the default statuses or a custom statuses you added to your Workfront system.</p> <note type="tip">         <p>If you select a status associated with an approval process as the rejection status, the rejected object moves to the selected status bypassing the approval process for the rejection status.</p>         <p> For example, if you select On Hold for the rejection status and the On&nbsp;Hold status is associated with an approval process, the rejected object is placed in the On&nbsp;Hold status without requiring the approval. </p>        </note> <p>For a system-wide approval process, only system-wide locked statuses are available.</p> <p>For a group-specific approval process, all group statuses are available. This includes any custom statuses that the group administrator created specifically for the group, as well as any system-wide statuses. </p> <p>For information about how approval process work with statuses, see the section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">How approval processes rely on statuses</a> in the article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Approval process overview</a>.</p> </li>      </ul> </li>    </ul> </td>  </tr> </tbody>``` 

1. (Optional) Click **Add Path** to add another path to the approval process, referring to the list of options in the previous step. 
1. The new path must be associated with another status. The path triggers when the item is updated to show this status. You cannot have two paths for the same status.
1. Click **Save**.
1. (Optional) Do any of the following:

   * Associate the approval process with specific projects, tasks, or issues throughout your system, as described in [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Outside of Workfront, notify users that the approval process is available for them to associate with their projects, tasks, or issues, as described in [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Create another approval process that is triggered if this approval process is rejected and the item takes on another status. This gives you a way to link approval processes together.

