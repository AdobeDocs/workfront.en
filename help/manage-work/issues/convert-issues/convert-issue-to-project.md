---
filename: convert-issue-to-project
product-area: projects
navigation-topic: convert-issues
title: Convert an issue to a project in Adobe Workfront
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Convert an issue to a project in *Adobe Workfront*

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
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Edit access to Financial Data to update financial information for a projected converted from the issue</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>You obtain&nbsp;Manage permissions to the project after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Convert an issue to a project

You can convert an issue to a blank project or convert an issue to a project using a template.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<ol>
<li value="1"> <p>Go to a project and click&nbsp;Issues in the left panel. </p> <p>The list of issues displays. </p> </li>
<li value="2"> <p>Do one of the following:</p>
<ul>
<li> <p>To convert an issue to a blank project, click the name of an issue, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then click <span class="bold">Convert to a blank project</span>. </p> <draft-comment>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Or</p>
<p>Select the issue in the list of issue, click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> at the top of the list, then click <span class="bold">Convert to a blank project</span>. </p>
</div>
</draft-comment>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Or</p>
<p>Select the issue in the list of issue, click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> at the top of the list, then click <span class="bold">Convert to a blank project</span>. </p>
</div> <p>You must manually add tasks to the project or attach a template to the project after you convert the issue. </p> <p>Continue with Step 3e below.</p> </li>
<li> <p>To convert an issue to a project using a template, do one of the following:</p>
<ul>
<li> <p>Click the name of an issue, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> to the right of the issue name</p> <p>Or</p> </li>
<li> <p>Select the issue in the list of issues, in a report, or dashboard, click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> at the top of the list, then click <span class="bold">Convert to project from Template</span> and start typing the name of a template in the <span class="bold">Search Template</span> box, then click the name of the template when it displays in the list. Continue with Step 3.</p> </li>
</ul> <note type="tip">
If you have added templates to your Favorites list, you can hover over the
<span class="bold">Favorite templates</span> menu and click the template you want to use.
</note> <p>The New Project from Template box displays</p> <p> <img src="assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png" style="width: 350;height: 279;"> </p>
<div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
<span class="autonumber"><span><b>Tip: </b></span></span>
<p>If the issue is associated with an approval process or it is already associated with a resolving object, <em>Workfront</em> displays a warning at the top of the Convert to Project box to notify you that the approval will be removed or the resolving object will be overwritten during the conversion. For more information, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>.</p>
</div> </li>
</ul> </li>
<li value="3"> <p>(Conditional)&nbsp;If you selected to convert the issue to a project using a template, continue with the following steps: </p>
<ol>
<li value="1"> <p>Review template details on the right. </p> <p>The template details include the following:</p>
<ul>
<li> <p>Template duration</p> </li>
<li> <p>Template owner</p> </li>
<li> <p>The number of top-level tasks which includes the names of the top three tasks</p> </li>
<li> <p>The number of all tasks in the template</p> </li>
<li> <p>The names of the template custom forms</p> </li>
</ul> </li>
<li value="2"> <p>(Optional)&nbsp;Hover over the name of a template and click the Favorites icon <img src="assets/favorites-icon-small.png"> to mark it as a favorite for future use.</p> <note type="tip">
You can have up to 40
<em>Workfront</em> items marked as favorites. This includes templates and other items.
</note> </li>
<li value="3"> <p>Click <span class="bold">Use template</span> to select a template.</p> <p>The Convert to Project box opens.</p> <p> <img src="assets/convert-to-project-from-template-large-project-box-nwe-350x291.png" style="width: 350;height: 291;"> </p> </li>
<li value="4"> <p>If a field is already populated in the template, the field is pre-populated in the <span class="bold">Convert to project</span> box. You can edit the pre-populated values to better match your project. For more information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p>
<div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
<span class="autonumber"><span><b>Tip: </b></span></span>
<p>To update fields in the Finance section in the Convert to Project box you must have Edit access to Financial&nbsp;Data in your access level.&nbsp;If you have View access to Financial Data in your access level all financial information from the template transfers to the new project and you cannot edit it while you convert the issue. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a> and <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Sharing a template</a>. </p>
</div> </li>
<li value="5"> <p>(Optional and conditional) Click <span class="bold">Options</span>, then select from the options that are available:</p>
<ul>
<li> <p><span class="bold"><span class="bold">Keep the original issue and tie its resolution to the this project</span><br></span>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li>
</ul>
</note> </li>
</ul>
<ul>
<li> <p><span class="bold">Allow <User Name> to have access to this project</span> </p> <p>If unselected, the issue's Primary Contact has no access to the new task.</p> <note type="note">
<p>The options that are available here depend on how the <em>Workfront administrator</em> has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span>.</span></p>
</note> </li>
</ul> </li>
<li value="6"> <p>Click <span class="bold">Custom Forms</span> and do any of the following:</p>
<ul>
<li> <p>Review the custom forms attached to the template.&nbsp;They will transfer to the new project.</p> </li>
<li> <p>Ensure all required fields have valid information. </p> </li>
<li> <p>Rearrange the custom forms by clicking <img src="assets/drag-object-icon.png">, then dragging and dropping them in the correct place. </p> </li>
<li> <p>Click the <span class="bold">x icon</span> to the right of any form that you do not want to transfer to the project. </p> </li>
<li> <p>(Optional and conditional) If you want to transfer custom form information from the issue you are converting to the project, add the project custom form that contains the same fields whose information you want to transfer from the issue. For information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data to a larger work item</a>.</p> </li>
</ul> </li>
<li value="7"> <p>Click <span class="bold">Convert to project</span>.</p> <p>If you decided to delete the original issue, the issue is now a project. <br>Or<br>If you decided to keep the original issue, the issue is now linked to the new project and it will complete when the project completes. </p> <p>Some issue fields transfer to the project. Most fields defined in the template automatically transfer to the newly created project if you didn't change them in previous steps. For information, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>. </p> </li>
</ol> </li>
<li value="4"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
<li value="5"> <p>Click&nbsp;<span class="bold">Convert to project</span>. </p> <p>The issue is now converted to a project. </p> <p>In the Production environment, if you selected to convert the issue from a list, report, or dashboard, you are directed to the project's page.</p> </li>
<li class="preview" value="6"> <p>(Conditional and optional)&nbsp;In the Preview environment, click <span class="bold">Go to project</span> inside the Success notification in the upper-right corner of the page. This opens the project page. </p> </li>
</ol>
</div>
-->

<ol> 
 <li value="1"> <p>Go to a project and click&nbsp;Issues in the left panel. </p> <p>The list of issues displays. </p> </li> 
 <li value="2"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>To convert an issue to a blank project, click the name of an issue, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then click <span class="bold">Convert to a blank project</span>. </p> 
    <div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <p>Or</p> 
     <p>Select the issue in the list of issue, click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> at the top of the list, then click <span class="bold">Convert to a blank project</span>. </p> 
    </div> <p>You must manually add tasks to the project or attach a template to the project after you convert the issue. </p> <p>Continue with Step 3e below.</p> </li> 
   <li> <p>To convert an issue to a project using a template, do one of the following:</p> 
    <ul> 
     <li> <p>Click the name of an issue, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> to the right of the issue name</p> <p>Or</p> </li> 
     <li> <p>Select the issue in the list of issues, in a report, or dashboard, click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> at the top of the list, then click <span class="bold">Convert to project from Template</span> and start typing the name of a template in the <span class="bold">Search Template</span> box, then click the name of the template when it displays in the list. Continue with Step 3.</p> </li> 
    </ul> <note type="tip">
     If you have added templates to your Favorites list, you can hover over the 
     <span class="bold">Favorite templates</span> menu and click the template you want to use. 
    </note> <p>The New Project from Template box displays</p> <p> <img src="assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png" style="width: 350;height: 279;"> </p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span> 
     <p>If the issue is associated with an approval process or it is already associated with a resolving object, <em>Workfront</em> displays a warning at the top of the Convert to Project box to notify you that the approval will be removed or the resolving object will be overwritten during the conversion. For more information, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>.</p> 
    </div> </li> 
  </ul> </li> 
 <li value="3"> <p>(Conditional)&nbsp;If you selected to convert the issue to a project using a template, continue with the following steps: </p> 
  <ol> 
   <li value="1"> <p>Review template details on the right. </p> <p>The template details include the following:</p> 
    <ul> 
     <li> <p>Template duration</p> </li> 
     <li> <p>Template owner</p> </li> 
     <li> <p>The number of top-level tasks which includes the names of the top three tasks</p> </li> 
     <li> <p>The number of all tasks in the template</p> </li> 
     <li> <p>The names of the template custom forms</p> </li> 
    </ul> </li> 
   <li value="2"> <p>(Optional)&nbsp;Hover over the name of a template and click the Favorites icon <img src="assets/favorites-icon-small.png"> to mark it as a favorite for future use.</p> <note type="tip">
     You can have up to 40 
     <em>Workfront</em> items marked as favorites. This includes templates and other items.
    </note> </li> 
   <li value="3"> <p>Click <span class="bold">Use template</span> to select a template.</p> <p>The Convert to Project box opens.</p> <p> <img src="assets/convert-to-project-from-template-large-project-box-nwe-350x291.png" style="width: 350;height: 291;"> </p> </li> 
   <li value="4"> <p>If a field is already populated in the template, the field is pre-populated in the <span class="bold">Convert to project</span> box. You can edit the pre-populated values to better match your project. For more information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span> 
     <p>To update fields in the Finance section in the Convert to Project box you must have Edit access to Financial&nbsp;Data in your access level.&nbsp;If you have View access to Financial Data in your access level all financial information from the template transfers to the new project and you cannot edit it while you convert the issue. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a> and <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Sharing a template</a>. </p> 
    </div> </li> 
   <li value="5"> <p>(Optional and conditional) Click <span class="bold">Options</span>, then select from the options that are available:</p> 
    <ul> 
     <li> <p><span class="bold"><span class="bold">Keep the original issue and tie its resolution to the this project</span><br></span>When deselected, the original issue is deleted.</p> <note type="note"> 
       <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li> 
       </ul> 
      </note> </li> 
    </ul> 
    <ul> 
     <li> <p><span class="bold">Allow <User Name> to have access to this project</span> </p> <p>If unselected, the issue's Primary Contact has no access to the new task.</p> <note type="note"> 
       <p>The options that are available here depend on how the <em>Workfront administrator</em> has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> 
       <p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span>.</span></p> 
      </note> </li> 
    </ul> </li> 
   <li value="6"> <p>Click <span class="bold">Custom Forms</span> and do any of the following:</p> 
    <ul> 
     <li> <p>Review the custom forms attached to the template.&nbsp;They will transfer to the new project.</p> </li> 
     <li> <p>Ensure all required fields have valid information. </p> </li> 
     <li> <p>Rearrange the custom forms by clicking <img src="assets/drag-object-icon.png">, then dragging and dropping them in the correct place. </p> </li> 
     <li> <p>Click the <span class="bold">x icon</span> to the right of any form that you do not want to transfer to the project. </p> </li> 
     <li> <p>(Optional and conditional) If you want to transfer custom form information from the issue you are converting to the project, add the project custom form that contains the same fields whose information you want to transfer from the issue. For information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data to a larger work item</a>.</p> </li> 
    </ul> </li> 
   <li value="7"> <p>Click <span class="bold">Convert to project</span>.</p> <p>If you decided to delete the original issue, the issue is now a project. <br>Or<br>If you decided to keep the original issue, the issue is now linked to the new project and it will complete when the project completes. </p> <p>Some issue fields transfer to the project. Most fields defined in the template automatically transfer to the newly created project if you didn't change them in previous steps. For information, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>. </p> </li> 
  </ol> </li> 
 <li value="4"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li> 
 <li value="5"> <p>Click&nbsp;<span class="bold">Convert to project</span>. </p> <p>The issue is now converted to a project. </p> <p>In the Production environment, if you selected to convert the issue from a list, report, or dashboard, you are directed to the project's page.</p> </li> 
 <li class="preview" value="6"> <p>(Conditional and optional)&nbsp;In the Preview environment, click <span class="bold">Go to project</span> inside the Success notification in the upper-right corner of the page. This opens the project page. </p> </li> 
</ol>

