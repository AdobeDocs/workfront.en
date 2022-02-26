---
filename: edit-assignments-for-multiple-issues
product-area: projects
navigation-topic: manage-issues
title: Edit user assignments for multiple issues
description: You can simultaneously modify user assignments to multiple issues. For information about editing issues or assigning them one at a time, also see the following articles:
---

# Edit user assignments for multiple issues

You can simultaneously modify user assignments to multiple issues.&nbsp;For information about editing issues or assigning them one at a time, also see the following articles:

* [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md) 
* [Assign issues](../../../manage-work/issues/manage-issues/assign-issues.md)

For general information about assigning issues, see [Modify issue assignments overview](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>You must have at least Contribute permissions to an issue be able to make assignments to the issue.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> licenses*</td> 
   <td> <p><em>Request</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="When"></a>When to modify user assignments on issues</h2>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## When to modify user assignments on issues

You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:

* Users join or leave&nbsp;your team
* A user takes a vacation that extends beyond the issue&nbsp;due dates
* A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role

## Modify assignments for multiple issues

<ol> 
 <li value="1">Go to the issue list that contains the&nbsp;issues whose assignments you want to modify. </li> 
 <li value="2"> <p>(Optional) Create a filter to display only issues assigned to the assignee that you want to modify.</p> <p>For example, you can create a filter to display only issues with a specific role as the assignee.&nbsp;Then, you can&nbsp;replace the role with a specific user. Do the following:</p> 
  <ol> 
   <li value="1"> <p>Click the <span class="bold">Filter</span>&nbsp;drop-down list, then click <span class="bold">New Filter</span>.</p> <p>The New Filter dialog box displays. </p> </li> 
   <li value="2">Click <span class="bold">Add a Filter Rule.</span></li> 
   <li value="3"> <p>To filter for a specific role, expand <span class="bold">Assignment Roles,</span>&nbsp;then click <span class="bold">ID.</span></p> <p>Or</p> <p>To filter for a specific user, expand <span class="bold">Assignment Users,</span>&nbsp;then click <span class="bold">ID.</span></p> <note type="tip">
     Do not use 
     <span class="bold">Assigned to</span>&nbsp;because this field refers only to the Issue Owner and not to all assignees.
    </note> </li> 
   <li value="4">In the drop-down list, select <span class="bold">Equal</span> as the filter qualifier.</li> 
   <li value="5">Begin typing the name of the user or role that you want to filter for, then click the name when it appears in the drop-down list.</li> 
   <li value="6">Click <span class="bold">Save Filter.</span></li> 
  </ol> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select the issues for which you want to modify assignments, then click the <span class="bold">Edit</span> icon <img src="assets/qs-edit-icon.png">. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select the issues for which you want to modify assignments, then click the <span class="bold">Edit</span> icon <img src="assets/qs-edit-icon.png">. </p> <p>The <span class="bold">Edit Issues</span> displays. The items that are edited display in the upper-left corner of the page.</p> </li> 
 <li value="4"> <p>Go to the <span class="bold">Assignments</span> section, then select <span class="bold">Assignee</span>.</p> <p> <img src="assets/classic-assignmens-area-on-edit-box-350x119.png" style="width: 350;height: 119;"> </p> </li> 
 <li value="5">Do one of the following:
  <ol>
   <ul>
    <li>To add a new assignee: 
     <ol>
      <li value="1"><p>Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues. </p>
       <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
        <span class="autonumber"><span><b>Tip: </b></span></span>
        <p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
        <p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span></p>
        <ul>
         <li><p><span>Reassign the work item to active resources.</span></p></li>
         <li><p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span></p></li>
        </ul>
       </div><p>Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the <span class="bold">Assignee</span>&nbsp;column. If information is not common across the issues selected, no information displays.</p></li>
     </ol></li>
    <li>To remove individual assignees: 
     <ol>
      <li value="1"><p>Click the <span class="bold">X icon</span> next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.</p><p>Or</p><p>(Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click <span class="bold">Remove Assignee</span> and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.</p></li>
      <li value="2">Click&nbsp;<span class="bold">Remove Assignee</span> again to add another assignee to remove.</li>
     </ol></li>
    <li>To remove all existing assignees: 
     <ol>
      <li value="1"><p>Click <span class="bold">Remove All Existing Assignees</span>, then click <span class="bold">Yes, Delete All Assignees</span>.</p><p>This removes not only common assignees (assignees that are displayed in the edit&nbsp;dialog box), but also all assignees on all the selected issues.</p></li>
     </ol></li>
   </ul>
  </ol></li> 
 <li value="6"> <p>(Optional) Modify any of the following options for the assignees you selected to associate with the issues:</p> 
  <ul> 
   <li><span class="bold">Issue Owner:</span>&nbsp;Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, <em>Adobe Workfront</em> designates the first assignee as the Issue Owner. This is not available for team assignments. </li> 
   <li><span class="bold">Assignee's Role</span>: Select a role from the drop-down list. If left unselected, <em>Workfront</em> automatically selects the Primary Role of the user. </li> 
  </ul> </li> 
 <li value="7">Click <span class="bold">Save Changes</span>.</li> 
</ol>

