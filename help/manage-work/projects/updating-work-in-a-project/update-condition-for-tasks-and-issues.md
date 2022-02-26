---
filename: update-condition-for-tasks-and-issues
product-area: projects
navigation-topic: update-work-in-a-project
title: Update Condition for tasks and issues
description: The Condition of a task or issue is a flag placed on it to indicate how it's going. This is different than the Status of the work item, which indicates the current stage of the development of the item.
---

# Update Condition for tasks and issues

The Condition of a task or issue is a flag placed on it to indicate how it's going. This is different than the Status of the work item, which indicates the current stage of the development of the item.

You can set the Condition of a task or an issue either automatically or manually.

The *Adobe Workfront administrator* can create custom Conditions for your environment, as described in [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access) section of this article.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on tasks and issues </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Automatically update the Condition by updating the status

When you are assigned a task or issue and you click `Work On It` `, Start Task or Start Issue,` or update its status, the Condition of the task or issue automatically changes to the default Condition associated with `Going Smoothly`.

For information about using a custom Condition as a default Condition, see the articles ` [Set a custom condition as the default for tasks and issues](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)` and [Set a custom condition as the default for projects](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

For information about changing the task status, see [Update task status](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

For information about changing the issue status, see [Update issue status](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

For information about setting the Work On It button to a Start Task or Start Issue button, see [Replace the Work On It button with a Start button](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Manually update the Condition

You must be assigned to a task or the issue or have Manage permissions to it to be able to set the Condition on it.

Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* You can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them.
* You can update the Condition only in a list of tasks or issues if you are not assigned to them, but have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue.

To manually set the Condition of a task or an issue:

<ol> 
 <li value="1"> <p>Go to a task or issue assigned to you for which you want to set the Condition.</p> <p>Or</p> <p>Go to a list of tasks or issues that you have Manage permissions to, but are not assigned to you. </p> </li> 
 <li value="2">Change the Condition of the issue or task as follows:
  <ul>
   <li><p> If you are assigned to the task or issue and have Manage permissions to it, on the <span class="bold">Updates</span> tab, click <span class="bold">Start a new update</span>, select the <span class="bold">Condition</span> that best reflects how the task is going, type your reason for changing the Condition in the <span class="bold">Start a new update</span> area (optional) , then click <span class="bold">Update</span>.</p><p>
     <draft-comment>
      <img src="assets/change-condition-update-comment-350x141.png" style="width: 350;height: 141;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     </draft-comment><img src="assets/change-condition-update-comment-350x141.png" style="width: 350;height: 141;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
   <li><p> If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <span class="bold">Condition</span> column to any view you use in a task or issue list, then set the <span class="bold">Condition</span> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p><note type="note">
     <span>Conditions can be customized for your environment, so you</span>
     <span data-mc-edit-date="2019-06-18T10:07:04.7449325-04:00" data-mc-editor="alinawilson" data-mc-comment="Remove draft with 19.3 and add link to COurtney's article??" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-06-18T10:06:50.3739957-04:00">may</span>
     <span> find more than three options for Condition in your environment. The names of the Conditions might be different than the ones listed above. For information about customizing Conditions in <em>Workfront</em>, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md" class="MCXref xref">Create or edit a custom condition</a>.</span>
    </note><p>For information about the additional functionality that is available when updating a work item, see <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</p></li>
  </ul></li> 
</ol>

