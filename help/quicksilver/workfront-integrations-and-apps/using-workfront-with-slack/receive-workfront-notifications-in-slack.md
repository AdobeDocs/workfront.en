---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Receive [!DNL Adobe Workfront] notifications in [!DNL Slack]
description: Receive [!DNL Adobe Workfront] notifications in [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
---
# Receive [!DNL Adobe Workfront] notifications in [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

After you have installed [!DNL Adobe Workfront for Slack], you can receive [!DNL Workfront] notifications in [!DNL Slack].\
For information about installing [!DNL Workfront for Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

You can enable a select number of [!UICONTROL notifications] that appear in the notifications bubble in the [!DNL Workfront] interface, to also be delivered in [!DNL Slack].

Email notifications work independently from [!DNL Workfront] interface notifications. You or your [!DNL Workfront] administrator can disable email notifications, whereas interface notifications cannot be disabled in [!DNL Workfront].\
You can, however, disable [!DNL Workfront] notifications that you might receive in [!DNL Slack], if you want to focus on those notifications only inside the [!DNL Workfront] interface. 

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.\

## Prerequisites

Before you can receive [!DNL Workfront] notifications in [!DNL Slack], you must

* Configure [!DNL Workfront for Slack]\
   For instructions on configuring [!DNL Workfront for Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configure [!DNL Workfront] notifications for [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Conditional) After [!DNL Workfront] has been added to your [!DNL Slack] instance, log into [!DNL Workfront] from [!DNL Slack].\
   For information about logging into [!DNL Workfront] from [!DNL Slack], see [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing one of the following commands in the message field: 

   `/workfront settings`

   Or

   `/wf settings`

1. All notifications are enabled, by default.\
   Disable any of the following notifications: 

   * [!UICONTROL I'm assigned to a new task or issue]
   * [!UICONTROL My team is assigned to a new task or issue]
   * [!UICONTROL I receive a new approval or access request]
   * [!UICONTROL Someone includes me on a directed update]
   * [!UICONTROL Someone comments on a thread I'm in]
   * [!UICONTROL An update is made to a task, issue or project I am subscribed to]
   * [!UICONTROL Someone comments on one of my work items]
   * [!UICONTROL Someone comments on my help request]

   The changes you make to the [!UICONTROL notifications] options take effect immediately.\
   The notifications you have enabled are delivered in the [!DNL Workfront] [!DNL Slack] channel. When you disable notifications here, they are only disabled for [!DNL Slack], and not for the [!DNL Workfront] interface. You continue to receive them in the [!DNL Workfront] notifications bubble in the upper right of the interface. 

## Manage [!DNL Workfront] notifications from [!DNL Slack]

You can receive and respond to [!DNL Workfront] notifications from [!DNL Slack]. 

You can disable email notifications for notifications that you enable in [!DNL Slack], to ensure that you do not receive duplicate notifications.\
For information about configuring your email notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Enabling or disabling [!DNL Workfront] notifications in [!DNL Slack] does not affect the notifications you receive inside the [!DNL Workfront] interface.\
Notifications inside the [!DNL Workfront] interface cannot be disabled. 

To manage your [!DNL Workfront] notifications for [!DNL Slack]: 

1. Log in to [!UICONTROL Slack].
1. Log in to [!DNL Workfront] from [!DNL Slack].\
   For information about logging in to [!DNL Workfront] from [!DNL Slack], see the "Logging in to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Ensure that your [!DNL Workfront] notifications for [!DNL Slack] are enabled.\
   For more information about which [!DNL Workfront] notifications can be configured to also be sent to [!DNL Slack], see [Configure [!DNL Workfront] notifications for [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Go to the **[!DNL Workfront]** channel to find your [!DNL Workfront] notifications. 
1. (Conditional and optional) Do any of the following: 

   * Click **[!UICONTROL Work on it]** to accept to work on a task.

   * (Conditional and optional) Click **[!UICONTROL Reply in [!DNL Workfront]]** to reply to a comment, type your reply, and click **[!UICONTROL Reply]**.

   * (Conditional and optional) Click **[!UICONTROL Approve]** or **[!UICONTROL Reject]** to approve or reject a task, issue, or project that are pending your approval.

   * (Conditional and optional) Click **[!UICONTROL Approve]**, **[!UICONTROL Changes]**, or **[!UICONTROL Reject]**, to approve, approve with changes, or reject a document.

      You can also mouse over the thumbnail of the document and click the magnifying glass icon to view a larger preview of the document, before you approve it.\
      Only the approved Slack [file types](https://api.slack.com/types/file) can be previewed. 

   * (Conditional and optional) Click **[!UICONTROL Grant]** or **[!UICONTROL Ignore]** to grant or ignore the request for more access from another user.\

      You receive a confirmation that your action has been completed in [!DNL Workfront], for every decision you make within your notifications.  
