---
filename: convert-issue-to-task
product-area: projects
navigation-topic: convert-issues
title: Convert an issue to a task in Adobe Workfront
description: If more work needs to be done to complete an issue after the issue is submitted, you can convert the issue to a task.
---

# Convert an issue to a task in  `Adobe Workfront`

If more work needs to be done to complete an issue after the issue is submitted, you can convert the issue to a task.

For general information about converting issues, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain&nbsp;Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Convert an issue to a task

<ol> 
 <li value="1"> Go to a project and click Issues in the left panel. </li> 
 <li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li> 
 <li value="3"> <p> Click the More menu on the issue, then Convert to Task. </p> <p>  </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>"> <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>If the issue is associated with an approval process or it is already associated with a resolving object, <span>Workfront</span> displays a warning at the top of the Convert to Project box to notify you that the approval will be removed or the resolving object will be overwritten during the conversion. For more information, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>.</p> 
  </div> </li> 
 <li value="4"> <p>Name the task.</p> </li> 
 <li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li> 
 <li value="6"> <p>In the <span class="bold">Project</span> box, start typing the name of the project where you want to put the new task, then press <span class="bold">Enter</span> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li> 
 <li value="7"> <p>(Optional and conditional) Under <span class="bold">Options</span>, select any of the following options. </p> <p>The <span>Workfront administrator</span> or <span>group administrator</span> must enable these preferences before they are visible during the conversion of issues: </p> 
  <ul> 
   <li> <p><span class="bold">Keep the original issue and tie its resolution to the this task</span> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">  
     <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
     <ul> 
      <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
      <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li> 
     </ul> 
    </note> </li> 
   <li> <p><span class="bold">Allow <User Name> to have access to this task</span> </p> <p>If unselected, the issue's Primary Contact has no access to the new task.</p> </li> 
   <li> <p><span class="bold">Keep the planned completion date of the issue</span> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li> 
  </ul> <note type="note">  
   <div> 
    <p>The options that display here depend on how the <span>Workfront administrator</span> configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> 
    <p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p> 
   </div> 
  </note> </li> 
 <li value="8"> <p> (Optional) Attach custom forms. </p> <p>If you want to transfer custom form information from the issue you are converting to the project, add the project custom form that contains the same fields whose information you want to transfer from the issue. </p> <p>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data to a larger work item</a>. <br></p> </li> 
 <li value="9">  </li> 
 <li value="10"> <p>Click <span class="bold">Save Changes</span> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#viewing-original-issue-information" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li> 
 <li value="11"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li> 
</ol>

## View original issue information on projects and tasks

You can view the original issue information in project and task lists and reports `or in the Project Details area`. For information about building reports, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

The following table illustrates which&nbsp;issue fields are visible from the converted projects and tasks. 

| Issue fields |Project or task field |Project list or report |Project Details area |Task list or report |Task Details area |
|---|---|---|---|---|---|
| Issue Name |Converted Issue Name |✔ |✔ |✔ |✔ |
| Primary Contact | `Converted Issue` Originator Name |✔ | `✔`  |✔ |&nbsp; |
| Entry Date |Converted Issue Entry&nbsp;Date |✔ |&nbsp; |✔ |&nbsp; |

` `**Warning: **``If the Primary&nbsp;Contact of an issue changes or if the issue becomes unlinked from the project or task after the issue has been converted, the Converted Issue Originator Name does not update and it displays the original&nbsp;Primary&nbsp;Contact of the issue at the time the issue was converted. 
