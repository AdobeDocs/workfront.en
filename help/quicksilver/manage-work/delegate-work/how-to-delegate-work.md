---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegate Tasks and Issues
description: You can temporarily delegate the work you are assigned to while you are out of the office. This article describes how to delegate task and issue assignments.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
---
# Delegate tasks and issues

<!-- Audited: 10/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

You can temporarily delegate the work you are assigned to while you are out of the office.

You can delegate task and issue assignments, or you can delegate approvals. This article describes how to delegate task and issue assignments.

For general information about delegating work, see [Delegate work overview](../../manage-work/delegate-work/delegate-work-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

>[!IMPORTANT]
>
>* The users that you select as delegates receive the same permissions as your permissions on the tasks and issues you delegate to them.
>* The permissions must work within their access levels, and sometimes their access levels might be lower than yours.
>
>   
>   For example, if a user has only View access to tasks in their access level and you have Manage permissions on the tasks you delegate to them, they receive Manage permissions to the tasks you delegate to them. However, they will not be able to perform the same actions as you on the delegated tasks. To be able to update tasks in your absence,they must request Edit access to Tasks from the system administrator.
>
>   
>   For information on how a system administrator can modify your access level, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* For items that are assigned after the delegation already started, it can take up to one hour after the item was assigned for [!DNL Workfront] to share the newly-assigned items with the delegate.


You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: Contributor or higher</p><p>Or</p><p>Current: Review or higher</p>

>[!NOTE]
>
>Although you can be assigned to work when you have a Request license, you cannot delegate your work to others. [!DNL Workfront] does not recommend assigning work to Review, Request, or Contributor users.

</tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the tasks or issues that you are assigned to</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Prerequisites

Before you can perform the activities described in this article, you must ensure the following:

* Your [!DNL Workfront] or group administrator enabled the [!UICONTROL **Allow users to delegate their tasks & issues**] setting in the [!UICONTROL Tasks & Issues Preferences] section in the [!UICONTROL Setup] area of your [!DNL Workfront] instance.

   For more information, see [Configure system-wide task and issue preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegate tasks and issues to another user

Before delegating work to others, we recommend that you reach out to them and inform them that they will be designated as delegates on your work items. Ask for their verbal approval before delegating work to ensure they have the time necessary to complete the work while you are out of the office.

For general information about delegating tasks and issues, see [Delegate tasks and issues overview](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

To delegate your tasks and issues to others:

1. Go to the [!UICONTROL **Home**] area.
1. Ensure you have the [!UICONTROL **My Work**], [!UICONTROL **My Tasks**], or [!UICONTROL **My Issues**] widgets added to your [!UICONTROL **Home**].

   For information, see [Add, edit, or remove widgets in Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)

1. Click [!UICONTROL **Delegate**] in the upper-left corner of the [!UICONTROL **My Work**], [!UICONTROL **My Tasks**], or [!UICONTROL **My Issues**] widgets.

   ![Delegate button](assets/delegate-button-on-my-work-widget.png)

1. Update the following:

   * [!UICONTROL **Delegate your tasks and issues to**]: Start typing the name of a user that you want your tasks and issues to be delegated to, then select it when it displays in the list. You can only select one user.

      The user that you select as a delegate receives the same  permissions as your permissions on the tasks and issues you delegate to them. 

   * [!UICONTROL **Start date**]: Select a date from the calendar when the delegation of your work items should start.

      >[!TIP]
      >
      >The Start date cannot be in the past.

   * [!UICONTROL **No end date**]: Select this option if you do not want to specify the end-date for your delegation.

   * [!UICONTROL **End date**]: Select a date from the calendar when the delegation should stop.

      >[!TIP]
      >
      >If you leave the End date field empty, and the No end date option is not selected, the delegation is set only for the current day.

      ![Delegate box expanded](assets/delegate-box-expanded-in-home.png)
      <!--check screen shot - submitted bug for casing-->

1. Click [!UICONTROL **Save**].

   The following things happen:

   * Your work is delegated to the specified user. Any incomplete tasks or issues that have dates within the time frame you selected (including newly assigned ones, after the delegation was enabled) are delegated.

      >[!TIP]
      >
      >   Completed work items that have dates within the time frame of the delegation are not delegated.


   * You receive a message at the bottom of the screen to confirm that you have enabled the delegation of your work to another user. The name of the delegate user displays in the confirmation message.

   * An indication that your tasks and issues are delegated to other users displays in most areas where you can see assignments in [!DNL Workfront]. For more information about what areas do not include delegates' names, see [Delegate work overview](delegate-work-overview.md).

   * The [!UICONTROL **Delegate**] button in the [!UICONTROL **Home**] area changes to [!UICONTROL **Edit delegation**] to indicate that there is a delegation in place.
      <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
      </MadCap:conditionalText>
      -->

      ![Edit delegation button](assets/edit-delegation-button-on-my-work-widget.png)

   * If your event notifications and your personal notifications are enabled, you also receive an email confirmation of your delegation.

   * The user you selected as your delegate receives an email about the delegation, if their event notifications are enabled.

      For information about enabling personal email notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Edit or stop delegation

You can let a delegation expire, if you selected an End Date, or you can manually stop it. You can also modify the time frame for the delegation, if the dates for the delegation changed.

1. Go to the [!UICONTROL **Home**] area, then click [!UICONTROL **Edit delegation**] in any of the following widgets: **My Work**, **My Tasks**, or **My Issues**.
1. In the [!UICONTROL Stop delegating tasks and issues] box, do one of the following:
   * Modify the [!UICONTROL **Start date**] or the [!UICONTROL **End date**]
   * Click [!UICONTROL **Stop delegation**]

   >[!TIP]
   >
   >    You can edit only the End date of a delegation if the delegation already started.

   ![Stop delegation button](assets/stop-delegation-box-new-home-tasks-and-issues.png)

1. (Conditional) click [!UICONTROL **Save**] to save the new delegation dates

   Or

   Click [!UICONTROL **Stop delegation**] in the confirmation box to confirm stopping the delegation.

   The delegation either updated the dates or it stopped and the delegated users have been removed from your tasks and issues. Their permissions to the tasks and issues remain in place.

## Locate delegated work and delegates information

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

When tasks and issues are delegated, there are several areas in [!DNL Workfront] where you can see the delegated work or who the delegates are.

* [Locate delegates in the Assignments box](#locate-delegates-in-the-assignments-box)
* [Locate delegated work in [!UICONTROL Home]](#locate-delegated-work-in-home)


### Locate delegates in the [!UICONTROL Assignments] box

When your system or group administrator enables work delegation in your system, the [!UICONTROL Assignments] box displays the following tabs everywhere you can access it:

* [!UICONTROL **Assignments**]: Users assigned to the task or issue display here.
* [!UICONTROL **Delegations**]: Users designated as delegates by the assignees on the task or issue display here.

You can access the [!UICONTROL Assignments] box in the following areas:

* The task or issue header

   The [!UICONTROL Assignments] field in the task or issue header changes to [!UICONTROL Assignments and delegations].

   ![Assignments and delegates panel in task header](assets/assignments-and-delegates-panel-in-task-header.png)

* The [!UICONTROL Workload Balancer] when manually assigning tasks or issues

   ![Assignments and delegations panel in Balancer](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> You cannot view delegates in the [!UICONTROL Assignments] section of a task or issue Edit box.

If a task or an issue is delegated and the [!UICONTROL Delegations] subtab is empty, one of the following scenarios might exist:

* You are not assigned to the task or issue.
* The task or issue dates are outside of the delegation time frame.

>[!TIP]
>
>The Planned or Actual Hours for delegated tasks and issues are not taken into account in resource management tools, like the [!UICONTROL Workload Balancer] or the [!DNL Resource Planner] for the delegated users. The hours remain associated only with the assigned user.

### Locate delegated work in [!UICONTROL Home]

1. Go to the [!UICONTROL **Home**] area in the [!UICONTROL **My Work**] widget. 
1. Click the filter drop-down menu and select one or more of the following options:
   * [!UICONTROL **Delegated**]: to view tasks and issues delegated to you or by you.
   * [!UICONTROL **Delegated to me**]: to view tasks and issues delegated to you by another user.
   * [!UICONTROL **Delegated by me**]: to view tasks and issues delegated by you to other users.

      ![Delegated tasks and issues filter](assets/delegated-tasks-and-issues-new-home-filter.png)

1. (Optional) Click the [!UICONTROL **Sort**] drop-down menu to sort the list by the following criteria:
   * [!UICONTROL Due Date]. This is the default sorting option.
   * [!UICONTROL Name]
   * [!UICONTROL Percent Complete]
   * [!UICONTROL Status]
1. (Optional) Expand the groupings drop-down menu in the upper-right of the [!UICONTROL **My Work**] widget, and group by one of the following criteria:
   * Nothing. This is the default grouping option.
   * [!UICONTROL Project]
   * [!UICONTROL Status]
   * [!UICONTROL Due Date]

1. To view either items you delegated or that have been delegated to you, view one of the following: 

   * For items that you delegated to others, find the delegate's name under the status of the task or issue, after [!UICONTROL **Delegated to**]. 

   * For items delegated to you, find the assignee's name under the status of the task or issue, after [!UICONTROL **Delegated to you by**].

      >[!TIP]
      >
      >    If the delegation is set to start at a date after today's date, the start date of the delegation also displays in the [!UICONTROL Work List]. The delegated items display in the grouping you select for the [!UICONTROL Work List], according to the type of the grouping. For example, if you group by [!UICONTROL Planned Completion Date], the delegated items display in the grouping that matches their planned completion dates.
