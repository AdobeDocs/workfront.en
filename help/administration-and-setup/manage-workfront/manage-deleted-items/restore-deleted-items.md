---
filename: restore-deleted-items
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restore deleted items
description: If you are a Workfront administrator, you can restore projects, tasks, issues, documents, and templates in Adobe Workfront if they have been deleted in the past 30 days. After 30 days, these items are permanently deleted and cannot be restored.
---

# Restore deleted items

If you are a Workfront administrator, you can restore projects, tasks, issues, documents, and templates in Adobe Workfront if they have been deleted in the past 30 days. After 30 days, these items are permanently deleted and cannot be restored.

When you restore an object, all of its child objects and fields are also restored. For example, if you restore a project, all tasks, issues, documents, hours, notes, assignments, and custom data in the project are also restored.

A group administrator can also restore these objects for a group they manage.

>[!IMPORTANT]
>
>* If you delete a report, dashboard, user, template, group, or team, it can’t be restored.
>* In a group, when someone other than the group administrator uploads a document directly to the Documents area of an object, only a Workfront administrator can restore the document.
>

## Access requirements

You must have the following to perform the steps in this article:

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
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## Information that is recovered when you restore a project, task, or issue

When you restore a project, task, or issue, the following associated information is recovered along with it:

* Comments and replies in the Updates area
* Approvals
* Assignments
* Custom Forms
* Queue setup
* Business cases, including scorecards, goals, and risks
* Project teams
* Dates
* Issues
* Tasks
* Subtasks
* Statuses
* Financial Information:

  * Billing records
  * Billing rates
  * Expenses

* Timeline information:

  * Predecessors
  * Task constraints
  * Duration type

* Baselines

  Task baselines are recovered when you restore their parent project or task, but not&nbsp;when you restore individually deleted tasks.

* Hours (and hour IDs)

  Whether hours are restored to the deleted item depends on the settings you chose when configuring preferences for timesheets and hours. For more information, see [Configure affect on hours when an object is deleted and restored](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* The URL of the&nbsp;item

  When restored, the URL of the item&nbsp;remains the same. If people have created browser bookmarks for the item, they&nbsp;remain valid.

* Access and permissions

  Users who had access to the item&nbsp;before it was deleted regain access after it is restored.

* Documents (including proofed documents)

  Consider the following when restoring documents and document versions:

  * Documents that were deleted individually can be restored individually.

    Documents that were deleted along with their parent project, task, or issue are recovered when you restore the parent, but you cannot restore them individually. 
  
  * All versions of a document or a document proof are restored when the document is restored.  
    Individual versions of a document or document proof that were deleted individually cannot be recovered.

## Information that is not recovered when you restore a project, task, or issue

When you restore a project, task, or issue, the following associated information is not recovered along with it:

* Likes
* Endorsements
* Intake Email Address in a request queue
* Favorites

  A project, task, or issue that you added to the Favorites menu before deleting it doesn't reappear on the Favorites menu after you restore it.

* Resolving objects

  A resolving object is a converted issue configured with the option `Keep the original issue and tie its resolution to this` < `project` or `task)`>. If you delete the parent project or task, the issue is no longer identified as a resolving object because there is no longer a link connecting it to the project or task. If you restore the parent, the link is not restored.

  For more information about how a Workfront administrator or group administrator configures issues to match the resolving object when converted, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) and [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  For more information about converting issues, see, [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restore items

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Recycle Bin` > `Recently Deleted`.
1. Click the `Projects`, `Tasks`, `Issues`, or `Documents` tab, depending on the type of item you want to restore.

   Items are sorted by the `Deletion Date` column by default.

1. Select up to 10 items that you want to restore.

   If you delete a child task, it displays in the list.

   If you delete a parent task, only the parent task shows in the list. But all child tasks are restored when you restore a parent task.

1. Click `Restore` to restore the selected items to their original location.
1. (Optional) To quickly view the restored item, follow the steps in [View restored items](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   For more information about what happens after you restore an item, see [What happens after you restore items](#what-happens-after-restoring-items) in this article.

## What happens after you restore items

* When you restore tasks and subtasks, they appear in the order they had prior to being deleted.

  However, if the order of other tasks changes while the task is deleted, the task might be restored to the bottom of the list of tasks or subtasks.

* After you restore an item:

  * A message displays to lets you know whether you were successful.

    You also receive an email notification. If you restored multiple items, the email lists them.
  
  * A comment displays in the Updates area of the project, task, or issue and in that of the parent object.

    This does not happen when you restore a document.

