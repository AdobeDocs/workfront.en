---
filename: create-advanced-assignments
product-area: projects;user-management
navigation-topic: assign-tasks
title: Create advanced assignments
description: You can manage task or issue assignments by using Advanced Assignments.
---

# Create advanced assignments

You can manage task or issue assignments by using Advanced Assignments.

You can adjust the following assignment information when making advanced assignments:

* Assign users to the task or issue (this can be accomplished outside of an advanced assignment).
* Adjust and redistribute the number of hours each assignee is allocated.
* Determine which user should be designated as the owner of the task or issue.
* Specify which role each user is fulfilling when working on the task or issue.

>[!NOTE]
>
>When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Work</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Tasks and Issues</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to a the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Make advanced assignments

<ol> 
 <li value="1">Go to the project where you want to assign a task or an issue. </li> 
 <li value="2"> Click Tasks or Issues in the left panel, then click the name of a task or issue in the list. <note type="tip">
   You can make advanced assignments directly on the task or issue list if there are two or more people assigned. Click inside the 
   <span class="bold">Assignments</span> field on the same line as the task or issue, then click the 
   <span class="bold">People icon</span> to open the Advanced Assignments window. Skip to step 5 to continue creating advanced assignments.
   <br>
  </note> </li> 
 <li value="3"> Click Assign to in the Assignments field in the header of the task or issue. Or Click the name of the assignments if the task or issue is already assigned. </li> 
 <li value="4"> Click Advanced. </li> 
 <li value="5"> In the Search people, role and teams field, start typing the name of a user, role, or team then click the name when it appears in the drop-down list. <note type="note">
    If the user's name contains a special character, you must include the special character in the search field. 
  </note> </li> 
 <li value="6"> (Optional) Continue adding assignees in the Search people, role or teams box to add multiple resources to the task or issue. 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p> 
   <p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p> 
   <ul> 
    <li> <p><span>Reassign the work item to active resources.</span> </p> </li> 
    <li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li> 
   </ul> 
  </div> </li> 
 <li value="7"> <p>For each user in the <span class="bold">Assignee</span> column, specify the following information:</p> 
  <ul> Owner: Hover over the name of the assignee and click Make Primary in the Owner field if you want to mark the assignee as the Task Owner. A green checkbox indicates that the specified user is the Primary Contact of the task or issue. Adobe Workfront marks the first user or job role that you assign to a task or issue as the Owner or Primary Assignment. A team cannot be designated the Primary Owner of a task or issue. Important: Depending on how your Workfront administrator or group administrator set up your project preferences, Workfront might use the schedule of the task owner to calculate the timeline of the task when you have multiple users assigned to the task. For information about multiple task assignees, see the "Assign multiple users to a task" section in the article Assign tasks. 
   <li> <p> Allocations: When the Duration Type of a task is Simple, specify the number of hours each user or job role should be assigned to the task. The sum of all assigned hours for each user is equal to the number in the <span class="bold">Planned Hours</span> field at the bottom of the Allocations column. In all other cases, specify the percentage of time (or allocation)&nbsp;that you want the assignee to spend solving the task or issue. </p> 
    <div class="tips" data-mc-autonum="<b>Tips: </b>">
     <span class="autonumber"><span><b>Tips: </b></span></span> 
     <ul> 
      <li> <p><span>After you manually modify assignment allocations on tasks, the Planned Hours of the tasks might update accordingly. For more information, see the section "Update task Planned Hours when managing user allocations" in the article</span><a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Planned Hours overview</a>.</p> </li> 
      <li> <p>You cannot manually modify assignment allocations on issues. </p> </li> 
      <li> <p>You cannot manually modify allocations for teams assigned to tasks.</p> </li> 
     </ul> 
    </div> </li> 
   <li> <p><span class="bold">Assignee's Role:</span> Select the role the user should use when fulfilling this assignment. The Primary Role of the user displays by default. Click in the Assignee's Role box to select another role.When you assign the task or the issue to a role first, and then add a user who can fulfill that role as a second assignment, the list of suggested users is filtered for the users who can fulfill the roles already assigned to the task and issue.</p>  </li> Duration Type: This is only available for tasks. Click the name of the Duration Type and select a Duration Type from the drop-down menu. For information about Duration Types, see Overview of Task Duration and Duration Type. 
   <li> Duration: You can update this field for a task when you have Manage permissions to the task. For more information, see Overview of Task Duration and Duration Type. When bulk editing assignment information, a similar dialogue box appears to assign users, hours, allocation, and task owner. </li> 
   <li> Planned Hours: When the Duration Type is Calculated Assignment or Simple, update the number of Planned Hours. The allocation percentages or the hours for each resource are distributed evenly as a result. Workfront calculates the Planned Hours when the Duration Type is Calculated Work or Effort Driven. For more information, see Overview of Task Duration and Duration Type.  </li> 
  </ul> </li> 
 <li value="8"> Click Save. </li> 
</ol>

