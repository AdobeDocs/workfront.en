---
product-area: projects
navigation-topic: manage-issues
title: Delete issues
description: You can delete issues or requests in Adobe Workfront if you have the correct access and permissions to do so.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
---
# Delete issues

<!--Audited: 01/2024-->

You can delete issues or requests in Adobe Workfront if you have the correct access and permissions to do so.

>[!TIP]
>
>"Issues" and "requests" are used interchangeably in Workfront. You can record issues on both projects and tasks to indicate unforeseen work that needs to be addressed. You can also submit requests which are recorded as issues on a project designated as a Request Queue.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Contributor or higher</p>
   <p>Current: Request or higher</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p>  <p>For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>Contribute or higher permissions on the project or task</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator. For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Considerations for deleting issues

* Your Workfront administrator or a group administrator must enable deleting issues in a project that has a status of Complete in your Project Preferences area. For information about setting up project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).   

* If the issue has logged hours, the Workfront administrator or a group administrator must allow the deletion of these issues by configuring the Task & Issue Preferences in your Workfront instance. This also applies when you try to delete projects that have issues with hours logged on them.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  For more information about enabling the deletion of issues where hours are logged, see the "Deletion" section in [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## The impact of deleting issues

When you delete an issue, you impact other objects linked to the issue.

The following objects attached to an issue are also deleted when you delete an issue:

* Documents

  You cannot delete an issue that has a document which has been checked out attached to it. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

* Notes
* Approvals

Depending on how your Workfront or group administrator configures the Project, Task, or Issue Deletion Preferences in the **Timesheet & Hour Preferences** of your Workfront instance, hours logged for the issues are handled in one of the following ways when deleting an issue:

* Move to the project and will not be restored on the issue, if the issue is later restored.
* Be deleted and will be restored on the issue, if the issue is later restored.

  This also applies when you try to delete projects that have tasks with hours logged on them.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  For more information about configuring the deletion preferences for hours logged on issues, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* The users assigned to the issue or to the issue approval remain on the project team.  
  For more information about project teams, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Delete issues

* [Delete multiple issues in a project simultaneously](#delete-multiple-issues-in-a-project-simultaneously) 
* [Delete a single issue](#delete-a-single-issue)

### Delete multiple issues in a project simultaneously  {#delete-multiple-issues-in-a-project-simultaneously}

1. Go to the **Main menu**. 
1. Click **Projects**.  
1. Click the project name that contains the issues you want to delete.
1. Click **Issues** in the left panel. 
1. Select an issue, then click the **Delete** icon ![](assets/delete.png) at the top of the list. 

1. If the deletion is allowed, click **Yes, Delete it**.  
   Your Workfront administrator might not allow the deletion of issues where hours are logged.  
   For more information about the access and permissions needed to delete an issue, see [Delete issues](#access-and-permissions-needed).

### Delete a single issue {#delete-a-single-issue}

{{step1-to-projects}} 

1. Click the project name that contains the issue you want to delete.
1. Click **Issues** in the left panel.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Click the name of the issue you want to delete.
1. Click the **More** menu to the right of the issue name.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Click **Delete Issue**. 
1. If the deletion is allowed, click **Yes, Delete it**.  
   
   Your Workfront administrator might not allow the deletion of issues where hours are logged.  
   For more information about the access and permissions needed to delete an issue, see [Delete issues](#access-and-permissions-needed).

## Restore deleted issues

A Workfront or group administrator can restore issues within 30 days after they are deleted. For more information about restoring items in Workfront, see [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
