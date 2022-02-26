---
filename: share-a-template
title: Share a template
product-area: templates
navigation-topic: grant-and-request-access-to-objects
title: Sharing a template
description: As an Adobe Workfront administrator, you can grant users access to view or edit templates when you assign their access level. A user must have a Plan license to have access to Edit templates.
---

# Sharing a template

As an *Adobe Workfront administrator*, you can grant users access to view or edit templates when you assign their access level. A user must have a Plan license to have access to Edit templates.

For more information about granting access to templates, see [Grant access to templates](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Along with the access level that you grant, a user can also receive permissions to View or Manage specific templates from other users who share them .

>[!NOTE]
>
>Permission levels work within Access levels. For example, a user cannot receive permissions to Manage a template, if their access level only allows them to View templates.

Permissions are specific to one item in *Workfront* and define what actions one can take on that item.

## Considerations when sharing a template

<ul> 
 <li>In addition to the considerations below, also see <a href="../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects in Adobe Workfront</a>.</li> 
 <li>The creator of a template, as well as the Template Owner have Manage permissions to the template, by default. For information about designating a user as the Template Owner, see <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</li> 
 <li> <p>You can share the following when sharing a template:</p> 
  <ul> 
   <li> <p>The template</p> <p>For more information about how to share a template, see <a href="../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Share project templates</a>.</p> <p>You can grant the following permissions to a template:</p> 
    <ul> 
     <li> <p>View</p> <p> <img src="assets/view-on-template-262x221.png" style="width: 262;height: 221;"> </p> </li> 
     <li> <p>Manage</p> <p> <img src="assets/manage-on-template-225x280.png" style="width: 225;height: 280;"> </p> </li> 
    </ul> </li> 
   <li> <p>The future projects which are created using the template. You can give the same levels of permissions to projects created from a template as you would an individual project.&nbsp;</p> <p>For information about how to share a project from a template at the template level, see <a href="../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Share project templates</a>. </p> </li> 
  </ul> </li> 
 <li> <p>When you share a template or a project which is created from the template, users inherit the same permissions to all the children objects associated with the template or the project, by default.</p> <p>For more information about the hierarchy of objects in <em>Workfront</em>, see&nbsp;<a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> </li> 
 <li> <p>When you share a template, all the template tasks and documents, as well as the issues on the future project created from the template inherit the same permissions, unless otherwise specified.</p> <p>For information about managing the access to template tasks and issues on the project based on a user's permissions to the project, see the <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md#access" class="MCXref xref">Access</a> section in the article <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</p> </li> 
 <p>The <em>Workfront administrator</em> can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> 
</ul>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Share"></a>Share a template</h2>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <span class="bold">Template Actions</span>, then <span class="bold">Template Sharing</span>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <span class="bold">Share Template</span>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <span class="bold">Give template access to</span> or <span class="bold">Edit template access for</span> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><span class="bold">View it</span>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><span class="bold">Manage it</span>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <span class="bold">Advanced Settings</span> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <span class="bold">Save</span>.</li>
</ol>
<h2><a name="sharing-project"></a>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <span class="bold">Template Actions</span>, then <span class="bold">Project Sharing</span>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <span class="bold">Share Project</span>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <span class="bold">Give project access to</span> or <span class="bold">Edit template access for</span> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><span class="bold">No access</span>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><span class="bold">View</span>: Users with these permissions can view projects created from the template.</li>
<li><span class="bold">Contribute</span>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><span class="bold">Manage</span>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <span class="bold">Advanced Settings</span> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <span class="bold">Save</span>.</li>
</ol>
</div>
-->

## Share a template

<ol> 
 <li value="1"> <p>Go to the template you want to share with other entities, click <span class="bold">Template Actions</span>, then <span class="bold">Template Sharing</span>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <span class="bold">Share Template</span>.</p> <note type="note">
    If you select multiple templates, you cannot view who already has permissions to the individual templates.
  </note> </li> 
 <li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <span class="bold">Give template access to</span> or <span class="bold">Edit template access for</span> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
   You can share an object only with active users, teams, 
   <span>roles,</span> or companies.
  </note> </li> 
 <li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
  <ul>
   <li><p><span class="bold">View it</span>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
   <li><span class="bold">Manage it</span>: Users with these permissions are able to edit or delete the template.</li>
  </ul></li> 
 <li value="4">(Optional) Click <span class="bold">Advanced Settings</span> to fine-tune your settings for each level of permissions.</li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

## Share a project at the template level

You can share the future projects that are created using a template with users at the template level.

<ol> 
 <li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <span class="bold">Template Actions</span>, then <span class="bold">Project Sharing</span>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <span class="bold">Share Project</span>.</p> <note type="note">
    If you select multiple templates, you cannot view who already has project permissions to the individual templates.
  </note> </li> 
 <li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <span class="bold">Give project access to</span> or <span class="bold">Edit template access for</span> fields.</p> <note type="tip">
   You can share an object only with active users, teams, 
   <span>roles,</span> or companies.
  </note> </li> 
 <li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
  <ul>
   <li><span class="bold">No access</span>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
   <li><span class="bold">View</span>: Users with these permissions can view projects created from the template.</li>
   <li><span class="bold">Contribute</span>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
   <li><span class="bold">Manage</span>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
  </ul></li> 
 <li value="4">(Optional) Click <span class="bold">Advanced Settings</span> to fine-tune your settings for each level of permissions. </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

## Advanced Settings for template sharing

The following table displays what permissions you can grant users when allowing them to View or Manage a template. For the instructions on sharing a template, see the section [Share a template](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) in the article [Share project templates](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table cellspacing="15"> 
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
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td> <p>Add Documents</p> <p>Tip: Sometimes people add documents to a project template thinking that they’re adding them to a project. You can prevent this for your recipients by disabling this setting.</p> </td> 
    <td>&nbsp;</td> 
    <td>✓</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td> <p>Add Documents</p> <p>Tip: Sometimes people add documents to a project template thinking that they’re adding them to a project. You can prevent this for your recipients by disabling this setting.</p> </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

To understand the permissions you are granting users to projects that are created from a template, see [Share a project in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
