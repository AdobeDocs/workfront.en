---
filename: create-and-modify-a-groups-templates
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and modify a group’s project templates
description: When you are viewing a group that you manage in the Groups area, you can view and work with project templates associated with the group and any of its subgroups.
---

# Create and modify a group’s project templates

When you are viewing a group that you manage in the Groups area, you can view and work with project templates associated with the group and any of its subgroups.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for `Workfront administrators` (for any group).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> <p>You must be a <span>group administrator</span> of the group or a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher on the templates you want to view and work with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your `Workfront administrator`.

## View, work with, and create templates for your group from the Groups area

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</li> 
 <li value="3">Click the name of the group for which you want to create or modify <span>templates</span>.</li> 
 <li value="4"> <p>In the left panel, click <span class="bold">Templates</span> to list the templates that are associated with the group and with any subgroups it might have.</p> <p>You must have View access to a template to see it in this list. For information about this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> </li> 
 <li value="5"> <p>Do any of the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Add a template</td> 
     <td> <p>Click <span class="bold">New Template</span>, then configure it using the available options. For information about these options, see <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Create a project template</a>.</p> <p>The template is automatically associated with the group.</p> <p>For information about how group preferences apply to new templates, see <a href="#how" class="MCXref xref">How preferences apply to templates and template tasks</a> in this article.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Edit one or more templates</td> 
     <td> <p>Select at least one template, click the Edit icon <img src="assets/edit-icon.png">, then use any of the available options to configure it. For information about these options, see <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</p> <p>The Edit icon is available only if you have Edit access to all of the templates you select. For information about this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Delete one or more templates</td> 
     <td> <p>Select at least one template, then click the Delete icon <img src="assets/delete.png">.</p> <p>This icon is available only if you have Edit access to all of the templates you select. For information about this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Share one or more templates</td> 
     <td> <p>Select at least one template, click the Share icon <img src="assets/share-icon.png">, then click one of the following options in the dropdown menu:</p> 
      <ul> 
       <li> <p><span class="bold">Template</span>: In the <span class="bold">Template Access</span> box that displays, add names to specify who you want to have access to the template itself.</p> <p>For more information, see the section <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Share a template</a> in the article <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Share project templates</a>.</p> </li> 
       <li><span class="bold">Project</span>: In the <span class="bold">Project Access</span> box that displays, add names to specify who you want to have access to the projects created from the template</li> 
      </ul> <p>The Share icon is available only if you have Share access to all of the templates you select. For information about this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Export the list of templates</td> 
     <td>Click <span class="bold">Export</span> <img src="assets/export.png">, then select the file format you want for the exported list.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

## How preferences apply to templates and template tasks

When you create a project template, the settings listed in the tables below are configured automatically by a correlating project or task preference.

>[!NOTE]
>
>Either a group-level or system-level project or task preference affects a project template, depending on whether you associated the template with a group when you created it. 
>
>If you did associate it with a group, the group-level preference takes effect. This occurs in the following scenarios:
>
>* You create the template from the Groups area, as explained in this article
>* You specify a group when creating the template using a Kickstart file
>* You specify a group when creating the template using the API
>
>If you didn't associate the new template with a group, the system-level preference takes effect. This occurs when in the scenarios below. (If you later assign a group to the template or template task, the group’s preferences don’t affect it.) 
>
>* You create the template from the Templates area
>* You don't specify a group when creating the template using a Kickstart file
>* You don't specify a group when creating the template using the API
>

* [Project template settings configured by project and task preferences](#project) 
* [Template task settings configured by task preferences](#template)

### Project template settings configured by project and task preferences

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Performance Index Method</p> </td> 
   <td> <p>Configured by the group-level project preference "Performance Index Method" if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Condition Type</p> </td> 
   <td> <p>Configured by the group-level project preference "Automatically set the project's Condition based on the Progress Status” if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schedule from</p> </td> 
   <td> <p>Configured by the group-level project preference "Schedule from” if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>User time off</p> </td> 
   <td> <p>Configured by the group-level project preference "User time off” if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Update type</p> </td> 
   <td> <p>Configured by the group-level project preference "Project timelines will be automatically re-calculated” if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Access section settings</p> </td> 
   <td> <p>Configured by the group-level task preferences in the "Access” section if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information about the project preferences listed in this table, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

For information about the task and issue preference, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* If you change the group that is associated with an existing project template, the template's settings remain the same.
>* If you move an existing template task to another template, the following settings remain unchanged in the template task, regardless of the group associated with the new template:>
>  * Duration Type
>  * Revenue Type
>  * Cost Type
>
>  However, the template task is affected by the setting "When someone is assigned to a task" on the new template. For more information, see the section [Access](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) in the article [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md). 
>
>* When an administrator saves a project as a template, all settings for the template are inherited from the project, including the group.
>
>  When an administrator converts a task or issue to a project using a template, all settings for the template are determined by what’s already saved on the template. 
>

### Template task settings configured by task preferences

When you create a template task, some of its settings are configured automatically by a correlating task preference. These settings are listed in the table below. 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Duration Type </p> </td> 
   <td> <p>Configured by the group-level task preference "Duration Type" if you associate the template with a group, or the same system-level task and issue preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Revenue Type</p> </td> 
   <td> <p>Configured by the group-level task preference "Revenue Type" if you associate the template with a group, or the same system-level task and issue preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cost Type </p> </td> 
   <td> <p> Configured by the group-level task preference "Cost Type" if you associate the template with a group, or the same system-level task and issue preference if you don't.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information about the task preferences listed in this table, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
