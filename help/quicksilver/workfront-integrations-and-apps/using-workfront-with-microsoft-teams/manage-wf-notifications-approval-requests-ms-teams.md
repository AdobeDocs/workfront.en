---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Manage [!DNL Adobe Workfront] notifications in [!DNL Microsoft] Teams
description: You can receive notifications from [!DNL Adobe Workfront] about items you need to approve, assignments you've been given, or comments and changes to items you're associated with.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
---
# Manage [!DNL Adobe Workfront] notifications in [!DNL Microsoft Teams]

>[!NOTE]
>
>The Adobe Workfront for Microsoft Teams integration is currently supported only for the classic Microsoft Teams experience.

You can receive notifications from [!DNL Adobe Workfront] about items you need to approve, assignments you've been given, or comments and changes to items you're associated with.

These notifications contain [!DNL Workfront] actions that you can take within [!DNL Microsoft Teams] without navigating away from [!DNL Microsoft Teams] to accomplish them. 

>[!NOTE]
>
>[!DNL Microsoft Teams] no longer supports [!DNL Internet Explorer]. To use the [!DNL Adobe Workfront for Microsoft Teams integration], you must use a web browser other than [!DNL Internet Explorer].


## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Prerequisites for Receiving [!DNL Workfront] Notifications in [!DNL Microsoft Teams]

You can receive [!DNL Workfront] notifications in [!DNL Microsoft Teams] if the following conditions are met:

* A team owner has installed and configured [!DNL Workfront for Microsoft Teams] for your team.
* You are logged into [!DNL Workfront] from [!DNL Microsoft Teams].
* You have enabled instant notifications in [!DNL Workfront]. For information on enabling instant notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

For information about installing [!DNL Workfront for Microsoft Teams] and logging in to [!DNL Workfront from Microsoft Teams], see [Install [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Managing [!DNL Workfront] Notifications in [!DNL Microsoft Teams]

When the [!DNL Workfront for Microsoft Teams] app is installed, a [!DNL Workfront] chat channel is created in [!DNL Microsoft Teams] for every member of that team. When an certain action is performed in [!DNL Workfront], you can configure the settings for [!DNL Workfront for Microsoft Teams] to receive notifications about that action in the [!DNL Workfront] chat channel of [!DNL Microsoft Teams].

Consider the following when working with [!DNL Workfront] notifications from [!DNL Microsoft Teams]:

* You cannot receive all, but only a select number of [!DNL Workfront] notifications in [!DNL Microsoft Teams].
* All notifications you receive from [!DNL Workfront] appear in the [!DNL Workfront] bot chat channel.

   For information on installing the [!DNL Workfront] bot channel, see the [Logging in to [!DNL Workfront] from [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) section in [Installing [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) article.

* There can be up to a 5 minute delay between the time when an update is made in [!DNL Workfront] and when you receive the notification about it in [!DNL Microsoft Teams].
* For each [!DNL Microsoft Teams] notification, you also receive an email notification.

To manage the [!DNL Workfront] notifications that you can receive in [!DNL Microsoft Teams]:

1. Click the **[!UICONTROL More added]** (three-dot) apps icon on the left navigation bar in [!DNL Microsoft Teams].

1. Click [!DNL Workfront] in the list that appears.
1. Select the **[!UICONTROL Settings]** tab.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Disable any of the notifications that you do not want to receive. You can enable or disable groups of notifications, such as information or approval notifications, or you can manage notifications individually.

   All notifications are enabled by default.

   The notifications settings for [!DNL Workfront for Microsoft] Teams are saved automatically.

   >[!NOTE]
   >
   >You cannot add more notifications to the ones that are available by default.

## Responding to [!DNL Workfront] Notifications and Approval Requests in [!DNL Microsoft Teams]

1. Log in to [!DNL Workfront] from [!DNL Microsoft Teams].\
   For information about logging in to [!DNL Workfront], see [Install [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Go to the **[!UICONTROL Chat]** area and click the **[!DNL Workfront]** bot channel.\
   This channel is for your personal chat with the [!DNL Workfront] bot. All [!DNL Workfront] notifications display here. 
1. Depending on what type of notification you receive, proceed to the relevant section:

    * [Approval notifications](#approval-notifications-approval-notifications)
    * [Assignment notifications](#assignment-notifications-assignment-notifications)
    * [Comment notifications](#comment-notifications-comment-notifications)
    * [Update notifications](#update-notifications-update-notifications)
    * [Date Change notifications](#date-change-notifications-date-change-notifications)

### Approval notifications {#approval-notifications}

You receive approval notifications when you are asked to approve an object, such as a task, timesheet, or proof. You can still comment on the notification, however.From the approval notification, you can perform the following actions:

* **[!UICONTROL Approve]**: Click to approve the item.
* **[!UICONTROL Change]**: Click to approve the item with changes.
* **[!UICONTROL Reject]**: Click to reject the item. 
* **[!UICONTROL Comment]**: Click to make a comment. Your comment also appears in [!DNL Workfront] as an update to the object that the notification is about.
* **[!UICONTROL Go to Proof]**: Click to open the proof. You can then make a decision directly in the proof. For more information, see [Make a decision on a proof in the proofing viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Once you have made an approval decision, you can not change it from the notification.

#### Actions available on specific approval notifications:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Go to Proof] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">You need to approve a project</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">You need to approve a task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">You need to approve an issue</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">You need to approve a document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">You need to approve access to an object</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">You need to approve a timesheet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Someone wants you to approve this proof</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Your timesheet is rejected</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Your timesheet is re-opened</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A document approval request that you requested is approved</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A document approval request that you requested is approved with changes</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A document approval request that you requested is rejected</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Your timesheet is approved</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Assignment notifications {#assignment-notifications}

You receive assignment notifications when you, or a team you are on, are assigned to a task or issue in Workfront. From the assignment notification, you can perform the following actions:

* **[!UICONTROL Work on it]**: Select to commit to work on the item. A notification displays briefly to confirm that a new item was added to your work list.
* **[!UICONTROL View in [!DNL Workfront]]**: Select to view the assigned issue or task in Workfront, which opens a new tab.
* **[!UICONTROL Start]**: Click to start work on the item. A notification displays briefly to confirm that a new item was added to your work list. 
* **[!UICONTROL Comment]**: Click to make a comment on the item. Your comment also appears in the item's update stream in Workfront.
* **[!UICONTROL Status]**: Click, then select the new status for the work item from the drop-down menu.

#### Actions available on specific assignment notifications:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">You are assigned to a task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">You are assigned to an issue</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A team to which you are assigned receives a work request for a task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A team to which you are assigned receives a work request for an issue</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Comment notifications {#comment-notifications}

You receive a communication notification when someone comments on an item you are associated with, or includes you in an update. From the communication notification, you can perform the following actions:

* **Rep[!UICONTROL ]ly**: Click to reply to the comment or [!UICONTROL update]. Your reply also appears in the update stream where the comment appears in Workfront.
* **[!UICONTROL View in Workfront]**: Select to view the comment and the item in Workfront, which is opened in a new tab.
* **[!UICONTROL Status]**: Click, then select a new status for the work item that the comment or update is about.

#### Actions available on specific communication notifications:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">A comment is posted on your request</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A reply is posted on your work request</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Someone comments on a thread you are in</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Someone comments on one of your work items</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Someone comments on a timesheet you approve</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A comment is added on your user profile page or by bulk editing multiple users</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A comment is added on one of your updates</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A comment is added on your timesheet</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Update notifications {#update-notifications}

You receive an information notification when there is an update to an item you are associated with, but you do not need to take any action on the item. From the information notification, you can perform the following actions:

* **[!UICONTROL Reply]**: Click to reply to the [!UICONTROL update]. Your reply also appears in the item's update stream in Workfront.
* **View in Workfront**: Select to view the comment and the item in Workfront, which is opened in a new tab.
* **[!UICONTROL Status]**: Click, then select the new status for the item from the drop-down menu.

#### Actions available on specific information notifications:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">An update is made to a task, issue or project you are subscribed to</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Someone includes you on a directed update</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Someone includes your team on a [!UICONTROL directed update]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Date Change notifications {#date-change-notifications}

You receive a date change notification when the date changes on a work item you are assigned to. From the date change notification, you can perform the following actions.

* **[!UICONTROL Comment]**: Click to make a comment on the item. Your comment also appears in the item's update stream in Workfront.
* **[!UICONTROL Status]**: Click, then select the new status for the work item from the drop-down menu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">The due date changes on a task you are assigned to</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
