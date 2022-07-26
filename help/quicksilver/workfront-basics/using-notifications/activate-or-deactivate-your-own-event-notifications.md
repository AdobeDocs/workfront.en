---
product-area: setup
navigation-topic: notifications
title: Activate or deactivate your own event notifications
description: Your Adobe Workfront administrator configures which event notifications users receive when events occur in Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
---
# Activate or deactivate your own event notifications

<!--
{{highlighted-preview}}
-->

Your Adobe Workfront administrator configures which event notifications users receive when events occur in Workfront (as described in [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

Your group administrator can also configure which event notifications are activated for you and the users in your Home Group. If your Home Group is a subgroup, you receive the event notifications activated for the top-level group above your group.

You can customize this further by configuring which notifications you receive. You can also choose whether you want to receive notifications as events happen or in one daily digest email.

For information about email notifications, see [Adobe Workfront notifications](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* If you activate a notification type and then find that you are not receiving notifications of that type, it may be because that type does not apply for your role.
>* The Workfront administrator or a group administrator cannot configure notifications for Workfront Goals. For more information about what notifications the Workfront administrator can configure, see [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). For information about configuring individual notifications for Workfront Goals continue to read this article. 
>

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## View and modify your email notification settings

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click your user name next to your profile picture.

1. Click the **More** icon ![](assets/more-icon.png) , then click **Edit**.

1. In the **Edit Person** box that displays, go to the **Notifications** section.

1. Click a category to view the notification settings related to that category.

   ![](assets/my-profile-notifications.png)

1. Select or deselect the check boxes on the right to specify whether you want to receive or not receive notifications daily, instantly, or both.

   You can also use the check boxes for a category to activate or deactivate all notifications in that category.

   >[!NOTE]
   >
   >If you are a team member for a project, you continue to receive email notifications for it until you are removed from the team, even if you no longer have access to the project. For instructions on removing users from a team, see [Remove users from projects](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   For the **Communication** category, you can select individual notifications for instant delivery only. To have notifications delivered in a daily digest, you must select all of them.

   If all email notifications for a given category are activated, the box in the category title appears as selected. If all email notifications in a given category are deactivated, the box is unselected. If some notifications are activated and others are deactivated, the category checkbox appears as a straight line.  
   When you modify a notification setting, the label **Edited** appears for that notification setting, to let you know that that notification setting has been modified.

1. If you selected any notifications to be sent as a daily digest, select the time of the day you want to receive it at the top of the **Notifications** section in the **Email Daily Digest after** menu.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   The daily digest includes events that meet the criteria of the notifications 24 hours prior to the selected time. You receive one daily digest email for each type of notification.  
   The daily digest may arrive after the time you select, depending on how many emails are queued for delivery in the system. The time listed is your local time as specified in your browser settings.

1. (Conditional and optional) When modifying email notifications settings in the Preview environment, enable the **Receive emails from this test environment** setting to receive emails. Emails are not automatically generated from the Preview environment.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Click **Save Changes**.
