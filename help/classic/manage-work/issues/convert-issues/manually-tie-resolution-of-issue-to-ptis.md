---
filename: manually-tie-resolution-of-issue-to-ptis
product-area: projects
navigation-topic: convert-issues
title: Manually tie the resolution of an issue to other issues, tasks, or projects
description: You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue.
---

# Manually tie the resolution of an issue to other issues, tasks, or projects

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue.

>[!TIP]
>
>When you tie the resolution of an issue to the resolution of another object you can no longer manually edit the status of the original issue.

For more information about resolving and resolvable objects, see [Overview of Resolving and Resolvable Objects](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Access requirements

You must have the following:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues,&nbsp;Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must:

* Have an issue whose resolution you want to tie to the resolution of another issue, task, or project

* Have an additional issue, task, or project

## Tie the resolution of an issue to the resolution of a another issue, task, or project

1. Navigate to an issue whose resolution you want to tie to the resolution of another issue or a task or project.
1. Click the **Issue Details** tab. 
1. Click **Edit Overview**.
1. At the bottom of the form, click in the **Resolved By** field, and select from the following types of resolving objects: &nbsp;

   * **Project**
   * **Task**
   * **Issue**

1. The field for the resolving object displays. 
1. After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. 
1. Click **Save**&nbsp;.  
   The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5. This means that the original issue completes when the resolving object (the project, task, or issue you linked it to) is completed.

   >[!NOTE]
   >
   >One project, task, or issue may have multiple issues as Resolvable Objects.

&nbsp;
