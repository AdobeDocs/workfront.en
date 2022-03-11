---
filename: convert-issue-to-project
product-area: projects
navigation-topic: convert-issues
title: Convert an issue to a project in Adobe Workfront
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Convert an issue to a project in Adobe Workfront

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

If more work needs to be done to complete an issue after the issue is submitted, you can convert the issue to a project.

You can convert an issue to a new project or you can convert it to a project using a template.&nbsp;This article describes both ways for converting issues to projects.

For general information about converting issues, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Access requirements

You must have the following access to perform the steps in this article:

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
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Edit access to Financial Data to update financial information for a projected converted from the issue</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>You obtain&nbsp;Manage permissions to the project after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Convert an issue to a project

You can convert an issue to a blank project or convert an issue to a project using a template.
Go to a project and click Issues in the left panel. The list of issues displays. Do one of the following: To convert an issue to a blank project, click the name of an issue, then click the More menu to the right of the issue name, then click Convert to a blank project. Or Select the issue in the list of issue, click the More menu at the top of the list, then click Convert to a blank project. You must manually add tasks to the project or attach a template to the project after you convert the issue. Continue with Step 3e below. To convert an issue to a project using a template, do one of the following: Click the name of an issue, then click the More menu to the right of the issue name Or Select the issue in the list of issues, in a report, or dashboard, click the More menu at the top of the list, then click Convert to project from Template and start typing the name of a template in the Search Template box, then click the name of the template when it displays in the list. Continue with Step 3. Tip: If you have added templates to your Favorites list, you can hover over the Favorite templates menu and click the template you want to use. The New Project from Template box displays Tip: If the issue is associated with an approval process or it is already associated with a resolving object, Workfront displays a warning at the top of the Convert to Project box to notify you that the approval will be removed or the resolving object will be overwritten during the conversion. For more information, see Overview of converting issues in Adobe Workfront. (Conditional) If you selected to convert the issue to a project using a template, continue with the following steps: Review template details on the right. The template details include the following: Template duration Template owner The number of top-level tasks which includes the names of the top three tasks The number of all tasks in the template The names of the template custom forms (Optional) Hover over the name of a template and click the Favorites icon to mark it as a favorite for future use. Tip: You can have up to 40 Workfront items marked as favorites. This includes templates and other items. Click Use template to select a template. The Convert to Project box opens. If a field is already populated in the template, the field is pre-populated in the Convert to project box. You can edit the pre-populated values to better match your project. For more information, see Edit projects. Tip: To update fields in the Finance section in the Convert to Project box you must have Edit access to Financial Data in your access level. If you have View access to Financial Data in your access level all financial information from the template transfers to the new project and you cannot edit it while you convert the issue. For information, see Grant access to financial data and Sharing a template. (Optional and conditional) Click Options, then select from the options that are available: Keep the original issue and tie its resolution to the this project When deselected, the original issue is deleted. Note: Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see: Grant access to issues Share an issue in Adobe Workfront Allow <User Name> to have access to this project If unselected, the issue's Primary Contact has no access to the new task. Note: The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see Configure system-wide task and issue preferences. Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see Configure task and issue preferences for a group. Click Custom Forms and do any of the following: Review the custom forms attached to the template. They will transfer to the new project. Ensure all required fields have valid information. Rearrange the custom forms by clicking , then dragging and dropping them in the correct place. Click the x icon to the right of any form that you do not want to transfer to the project. (Optional and conditional) If you want to transfer custom form information from the issue you are converting to the project, add the project custom form that contains the same fields whose information you want to transfer from the issue. For information, see Transfer custom form data to a larger work item. Click Convert to project. If you decided to delete the original issue, the issue is now a project. Or If you decided to keep the original issue, the issue is now linked to the new project and it will complete when the project completes. Some issue fields transfer to the project. Most fields defined in the template automatically transfer to the newly created project if you didn't change them in previous steps. For information, see Overview of converting issues in Adobe Workfront. (Optional) Set any further project details (project owner, project dates) and tasks as necessary. Click Convert to project. The issue is now converted to a project. In the Production environment, if you selected to convert the issue from a list, report, or dashboard, you are directed to the project's page. (Conditional and optional) In the Preview environment, click Go to project inside the Success notification in the upper-right corner of the page. This opens the project page. 