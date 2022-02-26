---
filename: reorder-group-statuses-from-groups-area
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Reorder group statuses
description: s mAs a group administrator, you can change the order of project, task, and issue statuses for a group you manage.
---

# Reorder group statuses

s mAs a 

<!--
<span data-mc-conditions="SnippetConditions-wf-groups.groups"><em>group administrator</em></span>
-->

`*group administrator*`, you can change the order of project, task, and issue statuses for 

<!--
<span data-mc-conditions="SnippetConditions-wf-groups.groups">a group you manage</span>
-->

`a group you manage`.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/statuses-350x116.png" style="width: 350;height: 116;"> </p>
-->

![](assets/statuses-350x116.png)

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *Workfront administrators* (for any group).

>[!NOTE]
>
>* >
>  <!-->
>  <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">>
>  A>
>  <em>Workfront administrator</em> can reorder>
>  </MadCap:conditionalText>>
>  -->
>  `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> A  <em>Workfront administrator</em> can reorder</MadCap:conditionalText>` the statuses at the system level>
>  <!-->
>  <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">>
>  . This>
>  </MadCap:conditionalText>>
>  -->
>  `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> . This</MadCap:conditionalText>` does not affect the order of statuses within groups. 
>
>  However, the statuses within a newly created top-level group inherit the order of the system-level statuses. (A new subgroup inherits the order of the statuses in the group one level up.)
>
>* You can reorder locked statuses. For information about locked statuses, see >
>  <!-->
>  <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref" data-mc-conditions="SnippetConditions-wf-groups.groups">Create or edit a group status</a>>
>  -->
>  [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a>* </td> 
   <td> <p>Any</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
    <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank"><em>Adobe Workfront</em> license</a>*</td> 
    <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank"><em>Adobe Workfront</em> license</a>*</td> 
   <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *Workfront administrator*.

## Default order of statuses

By default, statuses display in the following order:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Project</th> 
   <th width="33.33%">Task</th> 
   <th width="33.33%">Issue</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Current</li> 
     <li>Dead</li> 
     <li> On Hold </li> 
     <li> Planning </li> 
     <li> Complete </li> 
     <li> Requested </li> 
     <li> Approved </li> 
     <li> Rejected </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Complete</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Reopened</li> 
     <li>Awaiting Feedback</li> 
     <li>On Hold</li> 
     <li>Cannot Duplicate</li> 
     <li>Closed</li> 
     <li>Resolved</li> 
     <li>Verified Complete</li> 
     <li>Won't Resolve</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Reorder statuses for tasks and projects<draft-comment>
<span data-mc-conditions="SnippetConditions-wf-groups.groups"> in a group</span>
</draft-comment><span data-mc-conditions="SnippetConditions-wf-groups.groups"> in a group</span></h2>
<ol>
<li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> <draft-comment>
<li value="2" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Groups</span>, then click the name of the group.</li>
</draft-comment>
<li value="2" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Groups</span>, then click the name of the group.</li> <draft-comment>
<li value="3" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Statuses</span>.</li>
</draft-comment>
<li value="3" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Statuses</span>.</li>
<li value="4">Above the Statuses list that displays, click the <span class="bold">Projects</span> or <span class="bold">Tasks</span> tab.</li>
<li value="5"> <p>Drag and drop the statuses in the order you want.</p> <p>The new status order is saved automatically.</p> </li>
<li value="6">To test the new status order, go to a task or project<draft-comment>
<span data-mc-conditions="SnippetConditions-wf-groups.groups"> associated with the group</span>
</draft-comment><span data-mc-conditions="SnippetConditions-wf-groups.groups"> associated with the group</span>, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.</li>
</ol>
</div>
-->

## Reorder statuses for tasks and projects `in a group`

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Groups</span>, then click the name of the group.</li> 
 <li value="3" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Statuses</span>.</li> 
 <li value="4">Above the Statuses list that displays, click the <span class="bold">Projects</span> or <span class="bold">Tasks</span> tab.</li> 
 <li value="5"> <p>Drag and drop the statuses in the order you want.</p> <p>The new status order is saved automatically.</p> </li> 
 <li value="6">To test the new status order, go to a task or project<span data-mc-conditions="SnippetConditions-wf-groups.groups"> associated with the group</span>, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.</li> 
</ol>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Reorder statuses for issues</h2>
<ol>
<li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> <draft-comment>
<li value="2" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Groups</span>, then click the name of the group.</li>
</draft-comment>
<li value="2" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Groups</span>, then click the name of the group.</li> <draft-comment>
<li value="3" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Statuses</span>.</li>
</draft-comment>
<li value="3" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Statuses</span>.</li>
<li value="4">Click the <span class="bold">Issues</span> tab.</li>
<li value="5"> <p> (Optional) Select an issue type (<span class="bold">Bug Report</span>, <span class="bold">Change Order</span>, <span class="bold">Issue</span>, or <span class="bold">Request</span>).</p> <note type="note">
<ul>
<li> You cannot customize the order of statuses for the Master List.</li>
<li>We recommend that you order of statuses for each issue type the same way. For more information about issue types, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md" class="MCXref xref">Configure request types</a>.</li>
</ul>
</note> </li>
<li value="6"> <p>Drag and drop the statuses in the order you want.</p> <p>The new status order is saved automatically.</p> </li>
<li value="7">To test the new status order, go to an issue<draft-comment>
<span data-mc-conditions="SnippetConditions-wf-groups.groups"> associated with the group</span>
</draft-comment><span data-mc-conditions="SnippetConditions-wf-groups.groups"> associated with the group</span>, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.</li>
</ol>
</div>
-->

## Reorder statuses for issues

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Groups</span>, then click the name of the group.</li> 
 <li value="3" data-mc-conditions="SnippetConditions-wf-groups.groups">In the left panel, click <span class="bold">Statuses</span>.</li> 
 <li value="4">Click the <span class="bold">Issues</span> tab.</li> 
 <li value="5"> <p> (Optional) Select an issue type (<span class="bold">Bug Report</span>, <span class="bold">Change Order</span>, <span class="bold">Issue</span>, or <span class="bold">Request</span>).</p> <note type="note"> 
   <ul> 
    <li> You cannot customize the order of statuses for the Master List.</li> 
    <li>We recommend that you order of statuses for each issue type the same way. For more information about issue types, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md" class="MCXref xref">Configure request types</a>.</li> 
   </ul> 
  </note> </li> 
 <li value="6"> <p>Drag and drop the statuses in the order you want.</p> <p>The new status order is saved automatically.</p> </li> 
 <li value="7">To test the new status order, go to an issue<span data-mc-conditions="SnippetConditions-wf-groups.groups"> associated with the group</span>, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.</li> 
</ol>

