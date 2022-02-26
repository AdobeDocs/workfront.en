---
filename: assign-issues
product-area: projects
navigation-topic: manage-issues
title: Assign issues
description: You can assign issues to users, roles, and teams to indicate who is responsible for completing the issues. For general information about assigning issues, see Modify issue assignments overview.
---

# Assign issues

You can assign issues to users, roles, and teams to indicate who is responsible for completing the issues. For general information about assigning issues, see [Modify issue assignments overview](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

` `**Tip: **`` You can assign multiple users or job roles, and you can assign only one team. `You can assign only active users, `job roles`, and teams.`

`If a user, `job role`, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:`

* `Reassign the work item to active resources.` 
* `Associate the users in a deactivated team with an active team and reassign the work item to the active team.`

In addition to this article, we recommend that you read the following articles for more information about assigning issues:

* [Modify issue assignments overview](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md) 
* [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md) 
* [Edit user assignments for multiple issues](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md) 
* [Create advanced assignments](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) 
* [Make smart assignments](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md) 
* [Smart assignments overview](../../../manage-work/tasks/assign-tasks/smart-assignments.md) 
* [Overview of assigning work in the Adobe Workfront Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

You can assign an issue to one or multiple resources at the individual issue level, or you can assign multiple resources to multiple issues at one time.

Assigning issues and tasks is similar in&nbsp;*Adobe Workfront*. For general information about assigning tasks, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying&nbsp;the issue with the ability to&nbsp;Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations for multiple assignments to job roles, teams, and users

Consider the following when assigning multiple resources to a work item:

* Users can have more than one job role associated with their profile. For information about associating users with job roles, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Tasks or issues are usually first assigned to one or multiple job roles or to a team. When projects are ready to start, they might need to also be assigned to users.   
  If a task or an issue is assigned to one or multiple roles and then you also assign a user, *Adobe Workfront* decides which job role to associate with the additional user (if any)&nbsp;according to the following rules:

  * If there is only one job role assigned and it matches the user's Primary Role, then the task or issue is assigned only to the user fulfilling their&nbsp;Primary Role. 
  * If there are multiple roles assigned and at least one of the roles matches the user's secondary roles, then the task or issue is assigned to the user fulfilling one of their Other Roles — which *Workfront* selects at random if there are multiple matches — as well as any additional roles that are assigned.
  * If there is one or more job roles assigned and there are no matches to the user's roles, then the task or issue is assigned to both&nbsp;the role or roles as well as to the user.

* If a task or an issue is assigned to a team and you also assign a user, the task or issue remains assigned to both the team and the user.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Remove"></a> </h2>
<h2>Considerations about removing assignments from issues</h2>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Edit user assignments for multiple issues</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

##

## Considerations about removing assignments from issues

You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.

For more information about removing assignments from issues in bulk, see [Edit user assignments for multiple issues](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md).

Consider the following when removing assignments from issues:

* When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.
* When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources.

## Assign a single issue

<ol> 
 <li value="1">Go to an issue that you want to assign.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Assign to</span> in the upper-right corner of the issue header, in the <span class="bold">Assignments</span> area</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Assign to</span> in the upper-right corner of the issue header, in the <span class="bold">Assignments</span> area</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the name of the current assignments, if the issue is already assigned. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the name of the current assignments, if the issue is already assigned. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-assign-to-button-in-header-350x77.png" style="width: 350;height: 77;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-assign-to-button-in-header-350x77.png" style="width: 350;height: 77;"> </p> </li> 
 <li value="3"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>Start typing the name of a user, role, or team that you want to assign, then click it when it appears on the list.</p> <p> <draft-comment>
      <img src="assets/nwe-assignments-expanded-in-task-header-350x259.png" style="width: 350;height: 259;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     </draft-comment><img src="assets/nwe-assignments-expanded-in-task-header-350x259.png" style="width: 350;height: 259;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Conditional) Click one of the names in the <span class="bold">Suggested Assignments</span> list </li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Conditional) Click one of the names in the <span class="bold">Suggested Assignments</span> list </li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Assign to me</span> to assign it to yourself</li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Assign to me</span> to assign it to yourself</li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <span class="bold">Advanced</span> </p> <p>Creating advanced assignments is similar for tasks and issues. For information about how to make advanced assignments, see <a href="../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md" class="MCXref xref">Create advanced assignments</a>.</p> </li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <span class="bold">Advanced</span> </p> <p>Creating advanced assignments is similar for tasks and issues. For information about how to make advanced assignments, see <a href="../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md" class="MCXref xref">Create advanced assignments</a>.</p> </li> 
  </ul> </li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Save</span> to complete assigning the issue. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Save</span> to complete assigning the issue. </p> </li> 
 <li value="5"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional)&nbsp;Click the <span class="bold">X&nbsp;icon</span> next to the name of the assignments in the Assignments area on the header of the issue to remove an assignment.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional)&nbsp;Click the <span class="bold">X&nbsp;icon</span> next to the name of the assignments in the Assignments area on the header of the issue to remove an assignment.</p> </li> 
</ol>

## Assign an issue in a list

You can assign issues in a list or a report when any of the assignments fields are visible in the list's view. This is faster way to assign issues.

Depending on which field is visible in the view you can assign the following entities to the issue: 

| `Assign To`  |Assign one user  |
|---|---|
| `Assigned`  |Assign one user |
| `Assignments`  |Assign users, job roles, or a team.  |

To assign issues in a list:

<ol> 
 <li value="1"> <p>Go to a list of issues that has the Assigned To, Assigned, or Assignments fields in the view.</p> </li> 
 <li value="2"> <p>To assign issues do one of the following:</p> 
  <ul> 
   <li> <p>Click inside the <span class="bold">Assigned To</span> or <span class="bold">Assigned</span> fields and start typing the name of an active user that you want to assign to the issue, then click it when it displays in the list.</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/assigned-to-field-task-list-nwe.png"> </img> </p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/assigned-to-field-task-list-nwe.png"> </img> </p> </li> 
   <li> <p>Click inside the <span class="bold">Assignments</span> field and start typing the name of an <span>active</span> user, <span>job role</span>, or <span>active</span> team that you want to assign to the issue, then click it when it displays in the list.</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/assignments-field-task-list-nwe.png"> </img> </p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/assignments-field-task-list-nwe.png"> </img> </p> </li> 
  </ul> </li> 
 <li value="3"> <p>(Conditional) When visible in the Assignments field, click the <span class="bold">People icon</span> <span>
    <draft-comment>
     <img src="assets/teams.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/teams.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></span> in the upper-right corner of the assignments box to open the Advanced Assignments box and create advanced assignments. For more information, see <a href="../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md" class="MCXref xref">Create advanced assignments</a>. </p> <note type="tip">
   You cannot make advanced assignments from the Assigned To or Assigned fields.
  </note> </li> 
 <li value="4"> <p>After adding your assignees to the issue, press Enter or click anywhere on the page to save your changes. </p> </li> 
</ol>

## Assign issues in bulk

<ol> 
 <li value="1">Go to a list of issues that you want to assign in bulk. </li> 
 <li value="2"> Select several issues in the list. </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit icon</span> <img src="assets/qs-edit-icon.png">. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit icon</span> <img src="assets/qs-edit-icon.png">. </p> <p>The <span class="bold">Edit Issues</span> dialog box opens.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Assignments</span> area, select the <span class="bold">Assignee</span> box, then start typing the name of a user, job role, or team that you want to assign to all the issues. </p> <note type="important">
   If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 
  </note> </li> 
 <li value="5">(Optional) Select the radio button in the <span class="bold">Issue Owner</span> column to indicate which resource is the primary assignee or the Owner of the issue, when you assign more than one resource to the issue. This is not available for teams. </li> 
 <li value="6">(Optional) Select a role that the user should fulfill on the issue from the <span class="bold">Pick a role</span> drop-down menu in the <span class="bold">Assignee's Role</span> column when you assign users to issues. If you do not select a role, <em>Workfront</em> automatically selects the user's Primary&nbsp;Role. </li> 
 <li value="7">(Optional) If you want to remove existing assignees from all issues do one of the following:
  <ol>
   <li value="1">Start typing the name of a user, role, or team you want to remove from the issue, then select it when it appears on the list and click <span class="bold">Remove Assignee</span> to add additional assignees to remove. </li>
   <li value="2">Click&nbsp;<span class="bold">Remove All&nbsp;Existing Assignees</span> to remove all assignees from all selected issues.</li>
  </ol></li> 
 <li value="8">Click&nbsp;<span class="bold">Save Changes</span>.</li> 
 <li value="9">(Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the <span class="bold">X icon</span> next to the name of an assignee to remove it from the issue. </li> 
</ol>

