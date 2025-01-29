---
title: Sharing a template
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: As an Adobe Workfront administrator, you can grant users access to view or edit templates when you assign their access level. A user must have a Plan license to have access to Edit templates.
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
---
# Share a template

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>

As an Adobe Workfront administrator, you can grant users access to view or edit templates when you assign their access level. A user must have a Plan license to have access to Edit templates.

For more information about granting access to templates, see [Grant access to templates](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Along with the access level that you grant, a user can also receive permissions to View or Manage specific templates from other users who share them .

>[!NOTE]
>
>Permission levels work within Access levels. For example, a user cannot receive permissions to Manage a template, if their access level only allows them to View templates.

Permissions are specific to one item in Workfront and define what actions one can take on that item.

## Considerations when sharing a template

* In addition to the considerations below, also see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* The creator of a template, as well as the Template Owner have Manage permissions to the template, by default. For information about designating a user as the Template Owner, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* You can share the following when sharing a template:

   * The template

     For more information about how to share a template, see [Share project templates](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

     You can grant the following permissions to a template:

      * View
      * Manage

        ![](assets/view-on-template-262x221.png) ![](assets/manage-on-template-225x280.png)

      <span class="preview">In preview:
      ![](assets/template-permissions.png)
    </span>

   * The future projects which are created using the template. You can give the same levels of permissions to projects created from a template as you would an individual project.&nbsp;

     For information about how to share a project from a template at the template level, see [Share project templates](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* When you share a template or a project which is created from the template, users inherit the same permissions to all the children objects associated with the template or the project, by default.

  For more information about the hierarchy of objects in Workfront, see&nbsp; [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* When you share a template, all the template tasks and documents, as well as the issues on the future project created from the template inherit the same permissions, unless otherwise specified.

  For information about managing the access to template tasks and issues on the project based on a user's permissions to the project, see the [Access](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) section in the article [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* The Workfront administrator can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* You cannot share template tasks, individually. Sharing a template shares the template tasks as well. Sharing the project from the template also shares the future project tasks. 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Advanced Settings for template sharing

The following table displays what permissions you can grant users when allowing them to View or Manage a template. For the instructions on sharing a template, see the section [Share a template](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) in the article [Share project templates](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Actions</th> 
   <th>Manage</th> 
   <th>View</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Copy</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Edit Template Details</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>View Template</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Share</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Share System-wide</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Add Documents</p> <p>Tip: Sometimes people add documents to a project template thinking that they're adding them to a project. You can prevent this for your recipients by disabling this setting.</p> </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

To understand the permissions you are granting users to projects that are created from a template, see [Share a project in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
