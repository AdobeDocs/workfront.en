---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Delegate work overview
description: When you plan to be out of the office for a short period of time, you can temporarily delegate your work to other users to ensure that your absence does not become a roadblock to work being completed. 
author: Lisa
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
---
# Delegate work overview

When you plan to be out of the office for a short period of time, you can temporarily delegate your work to other users to ensure that your absence does not become a roadblock to work being completed.

For example, if certain tasks are due before you return but you do not have the time to complete them before you leave, you can delegate your tasks to another user so they can complete them on time and not delay the completion of the project until after you return.

You can delegate the following objects in [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tasks assigned to you
* Issues assigned to you
* Project, task, issue, document approvals assigned to you.

This article contains general information about delegating tasks and issues.

For information about delegating project, task, issue, and document approvals, see [Delegate approval request](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

For information about how to delegate tasks and issues see [Delegate tasks and issues](../../manage-work/delegate-work/how-to-delegate-work.md).

## Delegate work overview

Consider the following when you delegate tasks and issues:

* Your [!DNL Workfront] or group administrator must enable the Delegation preferences in the [!UICONTROL Setup] area before you can delegate your work to others.

   For information, see [Configure system-wide task and issue preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* You can delegate tasks and issues only from the [!UICONTROL Home] area.
* Exceptions exist for the following license types:

   * You can delegate work to Reviewers or Requestors, although [!DNL Workfront] doesn't recommend it.
   * Reviewers can delegate work to others. They cannot view work items in their [!UICONTROL Home] area. They can view only approvals.
   * Requestors cannot delegate work to others. They cannot view work items in their [!UICONTROL Home] area
* You can only delegate the tasks and issues assigned to you. You cannot delegate tasks and issues that are assigned to other users, teams, or job roles.
* You can only delegate tasks and issues that are not completed before the delegation's start date.
* If a work item completes during the delegation time frame, the item remains in the Home area of the delegate and of the assignee for 2 weeks before [!DNL Workfront] automatically removes it.
* The users that you select as delegates receive the same  permissions as your permissions on the tasks and issues you delegate to them. The permissions must work within their access levels, and sometimes their access levels might be lower than yours.

>[!NOTE]
>
>  For items that are assigned after the delegation already started, it can take up to one hour after the item was assigned for [!DNL Workfront] to share the newly-assigned items with the delegate.

* If additional tasks and issues are assigned to you during the time you have selected to have your work delegated to other users, the new assigned work is automatically delegated to the same person for the time frame you selected if the task or issue dates are within that time frame.
* The same user can be selected as the delegate by multiple users.
* Delegated tasks and issues do not display in resource management tools, like the [!UICONTROL Workload Balancer] or the [!UICONTROL Resource Planner] for the delegated users.
* You can view delegated work and delegates names in several areas of [!DNL Workfront]. For more information, see the section "Locate delegated work and delegates information" in the article [Manage task and issue delegation](../delegate-work/how-to-delegate-work.md).


   >[!IMPORTANT]
   >
   >  If a user has only View access to tasks in their access level and you have Manage permissions on the tasks you delegate to them, they receive Manage permissions to the tasks you delegate to them. However, they will not be able to perform the same actions as you on the delegated tasks. They must request Edit access to Tasks from the system administrator to be able to update tasks in your absence.

* Stopping delegation does not remove the permissions given to the delegated users on the tasks and issues they have been delegated on.
* If a system or  disables the [!UICONTROL Allow users to delegate their tasks & issues] setting in the [!UICONTROL Setup] area, the currently delegated users are removed from the tasks and issues they have previously been delegated to. Their permissions to the tasks or issues are not removed.

## Differences and similarities between assignments and delegations

| Action | Assignments | Delegations |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| An assigned or delegated user can edit or delete the work item they are assigned or delegated to | Based on permissions and access level | Based on permissions and access level |
| An assigned or delegated user displays in the work item's header | Yes | Yes |
| The assigned or delegated tasks or issues display in the assignee's or delegate's Home area | Yes, until the item is completed | Yes, only for the time frame of the delegation |
| You can assign or delegate work to users from the Home area | Yes | Yes |
| You can assign or delegate work to users using the | Yes | No |
| You can assign or delegate work to users in a list, or from a work item's header | Yes | No |
| Any user can assign or delegate other users with work items that they are not associated with | Based on permissions and access level | No. Only the assignee can delegate their own items. |
| Planned, Actual, or Budgeted Hours for work assigned or delegated to a user display for that user in resource management tools | Yes | No |
