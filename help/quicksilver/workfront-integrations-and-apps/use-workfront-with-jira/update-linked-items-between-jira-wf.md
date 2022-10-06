---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Update linked items between [!DNL Jira] and [!DNL Adobe Workfront]
description: When you link [!DNL Jira] issues to [!DNL Adobe Workfront] tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
---
# Update linked items between [!DNL Jira] and [!DNL Adobe Workfront]

When you link [!DNL Jira] issues to [!DNL Adobe Workfront] tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application. 

For more information about linking items between [!DNL Workfront] and [!DNL Jira], see [Link items between Adobe Workfront and Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

As you are setting up [!DNL Workfront] for [!DNL Jira], as a [!DNL Jira] system administrator, you can configure certain fields from one application to synchronize with fields from linked items in the other application.

For more information about synchronizing fields between linked [!DNL Jira] and [!DNL Workfront] items, see [Configure [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licenses overview</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in [!DNL Jira] and [!DNL Workfront] to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a [!DNL Workfront] administrator. For information on [!DNL Workfront] administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Prerequisites

Before you can link items between [!DNL Workfront] and [!DNL Jira], you must

* Install [!DNL Workfront for Jira].

   For instructions on installing [!DNL Workfront for Jira], see [Install [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configure [!DNL Workfront for Jira].

   For instructions on configuring [!DNL Workfront for Jira], see [Configure [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Link items between [!DNL Workfront] and [!DNL Jira].

   For instructions, see [Link items between [!DNL Adobe Workfront] and [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Update linked items in [!DNL Workfront]

If you work primarily in [!DNL Workfront], you can update your work items in [!DNL Workfront] and their counterparts in [!DNL Jira] also update. This update happens through the integration of [!DNL Workfront] for [!DNL Jira] which does not require you to have a [!DNL Jira] license. 

As long as your [!DNL Workfront] administrator has configured [!DNL Workfront for Jira] to synchronize the fields between linked items, certain fields that you update in [!DNL Workfront] also update for the linked [!DNL Jira] issue. For more information about updating items in [!DNL Workfront], see [Edit issues](../../manage-work/issues/manage-issues/edit-issues.md) and [Edit tasks](../../manage-work/tasks/manage-tasks/edit-tasks.md).

The following list shows which [!DNL Workfront] fields synchronize with [!DNL Jira] fields on linked items: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Updated [!DNL Workfront] field</strong> </th> 
   <th><strong>Synchronized [!DNL Jira] field/ update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>A comment about the Name change is added to the <strong>[!DNL Workfront]</strong> tab of the [!DNL Jira] issue. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>A comment about the updated Description is added to the <strong>[!DNL Workfront]</strong> tab of the [!DNL Jira] issue.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Note: Documents which are linked to [!DNL Workfront] items from an external server are not transferred to [!DNL Jira] issues. Only documents uploaded directly to [!DNL Workfront] items are also updated to the linked [!DNL Jira] issues. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>A comment about the uploaded attachments is added to the <strong>[!DNL Workfront]</strong> tab of the [!DNL Jira] issue.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>A comment about the [!UICONTROL Due Date] having changed is added to the [!DNL Workfront] tab of the [!DNL Jira] issue. </p> <p>Note: You must enable <strong>[!UICONTROL Due Date]</strong> for your [!DNL Jira] issues to be able to see this field updated in [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Custom Forms and Custom Fields</td> 
   <td> <p> Display in the [!DNL Workfront] right panel of the [!DNL Jira] issue. <br>Only the Custom Fields that have an actual value display in the panel.<br><img src="assets/custom-form-in-workfront-side-panel-274x309.png" alt="custom_form_in_workfront_side_panel.png" style="width: 274;height: 309;"></p> <p>Note: Custom Form sections are displayed with the access level of the [!DNL Workfront] administrator. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Displays in the [!DNL Workfront] right panel of the [!DNL Jira] issue. <br>It does not update the issue <strong>[!UICONTROL Priority]</strong> field in [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>A comment about the logged time is added in the <strong>[!DNL Workfront]</strong> tab of the [!DNL Jira] issue. This includes the name of the user who logs the time, as well as the user for whom the time is logged, in case they are different. No time is logged in the <strong>[!UICONTROL Work log]</strong> tab in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>The comment is added to the <strong>[!DNL Workfront]</strong> tab of the [!DNL Jira] issue. It is not added to the <strong>[!UICONTROL Comments]</strong> tab of the [!DNL Jira] issue</p> <p>Note: When you link two existing items manually, the comments that were added to the [!DNL Workfront] item before linking it to [!DNL Jira] do not synchronize to the [!DNL Jira] issue. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Update linked items in [!DNL Jira]

If you work primarily in [!DNL Jira], you can update your work items in [!DNL Jira] and their counterparts in [!DNL Workfront] also update. You do not have to have a [!DNL Workfront] license for the [!DNL Workfront] items linked to your [!DNL Jira] issues to receive the updates you are making in [!DNL Jira]. 

On condition that your [!DNL Workfront] administrator has configured [!DNL Workfront] for [!DNL Jira] to synchronize the fields between linked items, certain fields which you update in [!DNL Jira] also update for the linked [!DNL Workfront] item. 

The following list shows which [!DNL Jira] fields synchronize with [!DNL Workfront] fields on linked items: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Updated [!DNL Jira] Field</strong> </th> 
   <th><strong>Synchronized [!DNL Workfront] Field/ Update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>Issue status in [!DNL Jira] syncs with the following statuses, or statuses that equate with the following statuses, in Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Note: The [!DNL Jira] status syncs with the first [!DNL Workfront] status that equates with the appropriate status.</p> <p>For more information about statuses of items in [!DNL Workfront], see <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue Assignee]</td> 
   <td> <p> [!UICONTROL Issue or Task Assignee]</p> <p>Important: When you assign an item in [!DNL Jira] to a user who does not have a [!DNL Workfront] account, the integration creates a new active user in [!DNL Workfront] only when the option "[!UICONTROL Automatically create a user in [!DNL Workfront] if the [!DNL Jira] user does not have a [!DNL Workfront] account]" is set to [!UICONTROL Always]. This user does not occupy a [!DNL Workfront] license. Active users can be assigned to work items in [!DNL Workfront], but cannot be included in updates. For more information about configuring the automatic creation of [!DNL Workfront] users from [!DNL Jira], see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuring [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>A comment about uploading a new document in [!DNL Jira] is added to the [!UICONTROL Updates] tab of the [!DNL Workfront] issue or task.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> A comment about the change of the [!UICONTROL Due Date] in [!DNL Jira] is added to the [!UICONTROL Updates] tab of the [!DNL Workfront] issue or task. </p> <p>Note: No dates change on the [!DNL Workfront] issue or task. </p> </td> 
  </tr> 
  <tr> 
   <td> Log time in the [!DNL Workfront] right panel or from the [!UICONTROL More] menu on the [!DNL Jira] issue<br></td> 
   <td> <p>Hours<br>In addition to adding the hours logged in Jira to the linked [!DNL Workfront] item, a comment about logging time is added to the [!UICONTROL Updates] tab of the [!DNL Workfront] item.</p> <p>For more information about logging time on linked [!DNL Jira] issues, including updating the [!DNL Jira] user who is logging the time in [!DNL Workfront], see <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Log time for Linked [!DNL Jira] and [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comments <br><br></td> 
   <td> <p>Comments are added to the [!UICONTROL Updates] tab of the [!DNL Workfront] issue or task if the <strong>[!UICONTROL Comments]</strong> setting in the [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] section of the [!UICONTROL Setup] tab to <strong>[!UICONTROL Always]</strong>.</p> <p>For information about configuring Workfront settings in [!DNL Jira], see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuring [!DNL Workfront for Jira]</a>.</p> <p>For information about commenting on items from linked [!DNL Jira] issues, see <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comment from a linked [!DNL Jira] issue</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Log time from linked [!DNL Jira] issues

The time that you record for a [!DNL Jira] item in [!DNL Jira] will also transfer to the linked [!DNL Workfront] item, regardless of where in [!DNL Jira] you log the time.\
When you log time in Jira in the [!DNL Workfront] panel, the time is recorded only in [!DNL Workfront].\
The time you record in [!DNL Workfront] does not affect the time of the linked issue in [!DNL Jira]. 

>[!NOTE]
>
>If the time is added to a [!DNL Jira] item linked to a [!DNL Workfront] task, the [!UICONTROL Hour Type] for the time in [!DNL Workfront] is [!UICONTROL Task Time]. If the time is added to a [!DNL Jira] item linked to a [!DNL Workfront] issue, the [!UICONTROL Hour Type] for the time in [!DNL Workfront] is [!UICONTROL Issue Time].

A comment is added to the **[!DNL Workfront]** tab in [!DNL Jira] and to the **[!UICONTROL Updates]** tab of the item in [!DNL Workfront] to record logging the time.\
The time is also displayed in the **[!UICONTROL Hours]** tab of the [!DNL Workfront] item. 

* [Log time for Linked [!DNL Jira] and [!DNL Workfront] items](#log-time-for-linked-dnl-jira-and-dnl-workfront-items-log-time-for-linked-jira-and-workfront-items) 
* [Log time from [!DNL Jira] to a [!DNL Workfront] item](#log-time-from-dnl-jira-to-a-dnl-workfront-item-log-time-from-jira-to-a-workfront-item)

### Log time for Linked [!DNL Jira] and [!DNL Workfront] items {#log-time-for-linked-jira-and-workfront-items}

You can log time from a [!DNL Jira] issue linked to a [!DNL Workfront] item, and the time is recorded both on the [!DNL Jira] issue as well as the [!DNL Workfront] item. 

>[!IMPORTANT]
>
>If the user logging the time in [!DNL Jira] does not exist in [!DNL Workfront], the integration creates a new active user in Workfront if the **[!UICONTROL Automatically create a user in [!DNL Workfront]&#x200B;if the [!DNL Jira] user does not have a* [!DNL Workfront]&#x200B;account]** is set to **[!UICONTROL Always]**. This user does not occupy a [!DNL Workfront] license. You can assign active users to work items in [!DNL Workfront], but you cannot include them in updates. For information about configuring the automatic creation of [!DNL Workfront] users from [!DNL Jira], see [Configuring [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

To log time for an item in [!DNL Jira] and have it recorded both in [!DNL Jira] and [!DNL Workfront]:

1. Log into [!DNL Jira].
1. Go to the [!DNL Jira] issue which is linked to the [!DNL Workfront] item.
1. Expand the **[!UICONTROL More]** menu and click **[!UICONTROL Log work]**.\
   ![log_time_from_More_menu_in_Jira.png](assets/log-time-from-more-menu-in-jira-239x232.png)

1. In the **[!UICONTROL Time Spent]** field, specify the amount of time spent working on this issue. You must specify the time using the following time periods:

   * [!UICONTROL Weeks] (w)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Hours] (h)

1. Continue adding information to your time entry, including a **[!UICONTROL Work Description]**, then click **[!UICONTROL Log]**.\
   The time is added to the **[!UICONTROL Work log]** tab of the [!DNL Jira] item, as well as to the [!DNL Workfront] item linked to it.\
   The work description of the time entry is recorded as a note on the hour entry in [!DNL Workfront]. 

### Log time from [!DNL Jira] to a [!DNL Workfront] item {#log-time-from-jira-to-a-workfront-item}

You can log time just to the linked [!DNL Workfront] item from the [!DNL Jira] issue without recording this time to the [!DNL Jira] issue. 

1. Log into [!DNL Jira].
1. Navigate to a [!DNL Jira] issue which is linked to a [!DNL Workfront] item.

   The details of the [!DNL Workfront] item should display in the [!DNL Workfront] right panel of the issue.

1. Click the **[!UICONTROL Log Time]** icon.

   ![Log_time_in_Jira.png](assets/log-time-in-jira.png)

1. Specify the amount of **[!UICONTROL Hours]** and **[!UICONTROL Minutes]** you want to log for the issue.

1. Click **[!UICONTROL Log Time]**.

   The time is added to the [!DNL Workfront] item.

   This time is not added to the [!UICONTROL Work Log] tab of the [!DNL Jira] issue. 

## Comment from a linked [!DNL Jira] issue {#comment-from-a-linked-jira-issue}

When you comment on a [!DNL Jira] item from the [!DNL Workfront] right panel in [!DNL Jira], the comment is also added to the [!UICONTROL Updates] tab of the linked item in Workfront. 

To comment from [!DNL Jira] to a [!DNL Workfront] item:

1. Log into [!DNL Jira].
1. Navigate to a [!DNL Jira] issue which is linked to a [!DNL Workfront] item.

   The details of the [!DNL Workfront] item should display in the [!DNL Workfront] right panel of the issue.

1. Click the **[!UICONTROL Comments]** icon in the [!DNL Workfront] panel or n the **[!UICONTROL Comments]** tab. ![Jira_comments_icon.png](assets/jira-comments-icon.png)

1. Start typing a comment, then click **[!UICONTROL Send]**.

   The comment is added to the following:

   * The **[!DNL Workfront]** tab of the [!DNL Jira] issue.
   * The **[!UICONTROL Comments]** tab of the [!DNL Jira] issue.
   * The **[!UICONTROL Updates]** tab of the linked item in Workfront.
