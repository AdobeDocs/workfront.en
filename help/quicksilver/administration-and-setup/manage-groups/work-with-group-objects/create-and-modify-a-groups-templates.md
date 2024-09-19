---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and Modify a Group's Project Templates
description: When you are viewing a group that you manage in the Groups area, you can view and work with project templates associated with the group and any of its subgroups.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
---
# Create and modify a group's project templates

When you are viewing a group that you manage in the Groups area, you can view and work with project templates associated with the group and any of its subgroups.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher on the templates you want to view and work with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## View, work with, and create templates for your group from the Groups area

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the group for which you want to create or modify templates.
1. In the left panel, click **Templates** to list the templates that are associated with the group and with any subgroups it might have.

   You must have View access to a template to see it in this list. For information about this access, see [Grant access to templates](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Add a template</td> 
      <td> <p>Click <strong>New Template</strong>, then configure it using the available options. For information about these options, see <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Create a project template</a>.</p> <p>The template is automatically associated with the group.</p> <p>For information about how group preferences apply to new templates, see <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">How preferences apply to templates and template tasks</a> in this article.</p> </td> 
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
        <li> <p><strong>Template</strong>: In the <strong>Template Access</strong> box that displays, add names to specify who you want to have access to the template itself.</p> <p>For more information, see the section <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Share a template</a> in the article <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Share project templates</a>.</p> </li> 
        <li><strong>Project</strong>: In the <strong>Project Access</strong> box that displays, add names to specify who you want to have access to the projects created from the template</li> 
       </ul> <p>The Share icon is available only if you have Share access to all of the templates you select. For information about this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Export the list of templates</td> 
      <td>Click <strong>Export</strong> <img src="assets/export.png">, then select the file format you want for the exported list.</td> 
     </tr> 
    </tbody> 
   </table>

## How preferences apply to templates and template tasks {#how-preferences-apply-to-templates-and-template-tasks}

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
>If you didn't associate the new template with a group, the system-level preference takes effect. This occurs when in the scenarios below. (If you later assign a group to the template or template task, the group's preferences don't affect it.) 
>
>* You create the template from the Templates area
>* You don't specify a group when creating the template using a Kickstart file
>* You don't specify a group when creating the template using the API
>

* [Project template settings configured by project and task preferences](#project-template-settings-configured-by-project-and-task-preferences) 
* [Template task settings configured by task preferences](#template-task-settings-configured-by-task-preferences)

### Project template settings configured by project and task preferences {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Performance Index Method</p> </td> 
   <td> <p>Configured by the group-level project preference "Performance Index Method" if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Condition Type</p> </td> 
   <td> <p>Configured by the group-level project preference "Automatically set the project's Condition based on the Progress Status" if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schedule from</p> </td> 
   <td> <p>Configured by the group-level project preference "Schedule from" if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>User time off</p> </td> 
   <td> <p>Configured by the group-level project preference "User time off" if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Update type</p> </td> 
   <td> <p>Configured by the group-level project preference "Project timelines will be automatically re-calculated" if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Access section settings</p> </td> 
   <td> <p>Configured by the group-level task preferences in the "Access" section if you associate the new template with a group, or the same system-level project preference if you don't.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information about the project preferences listed in this table, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

For information about the task and issue preference, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* If you change the group that is associated with an existing project template, the template's settings remain the same.
>* If you move an existing template task to another template, the following settings remain unchanged in the template task, regardless of the group associated with the new template:>
>   * Duration Type
>   * Revenue Type
>   * Cost Type
>
>  However, the template task is affected by the setting "When someone is assigned to a task" on the new template. For more information, see the section [Access](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) in the article [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md). 
>
>* When an administrator saves a project as a template, all settings for the template are inherited from the project, including the group.
>
>  When an administrator converts a task or issue to a project using a template, all settings for the template are determined by what's already saved on the template. 
>

### Template task settings configured by task preferences {#template-task-settings-configured-by-task-preferences}

When you create a template task, some of its settings are configured automatically by a correlating task preference. These settings are listed in the table below. 

<table style="table-layout:auto"> 
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
