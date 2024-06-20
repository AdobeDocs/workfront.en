---
user-type: administrator
product-area: system-administration
keywords: modify,email,notification,settings,bulk,bulk-edit,configure,multiple,users
navigation-topic: emails-administration
title: Modify multiple users' email notification settings
description: This article provides information for the Workfront or group administrators about how they can update the email notifications of other users.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
---
# Modify multiple users' email notification settings

<!-- Audited: 12/2023 -->

If you are an Adobe Workfront administrator or you have a Planner access level allowing you to edit other users' settings, you can configure the notification settings for multiple users at one time. This includes specifying whether users receive notifications as events happen, or in one daily digest email, as described in [Adobe Workfront notifications](../../../workfront-basics/using-notifications/wf-notifications.md). For information about the access level needed to edit users, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

You can also configure email notifications for one user at a time, including your own profile. For more information, see [Modify your own email notifications](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New plan: Standard </p>
 <p>or</p> 
<p>Current plan: Plan </p> 
</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modify email notification settings for multiple users

When you configure notification settings in bulk, you can change only the settings that the selected users have in common.

When you modify a notification setting, the label **Edited** appears for that notification setting, to let you know that that notification setting has been modified.

To modify email notification settings for multiple users:

{{step-1-to-users}}

1. Select the users, then click **Edit**. 
1. In the **Edit Person** box that appears, click **Notifications**.

1. Expand a category to view notification settings related to that category.

   If there is at least one user selected where the notifications do not match the notifications of the other selected users, the category check box for that notification contains a horizontal line ![](assets/straight-line-instead-of-checkmark.jpg) instead of a check mark.


1. Click any notifications that you want the users to receive either daily or instantly, or clear any that you want them to stop receiving.

   >[!NOTE]
   >
   >   For the **Communication** category, you can select individual notifications for instant delivery only. You must select all of the notifications to be delivered in a daily digest.


1. If you selected notifications to be sent as a daily digest, select the time of the day you want the digest delivered at the top of the **Notifications** section in the **Email Daily Digest after** menu.

   ![](assets/daily-digest-time.png)

   The daily digest includes events that meet the criteria of the notifications 24 hours prior to the selected time. Users receive one daily digest email for each notification type.

   The daily digest may arrive after the time you select, depending on how many emails are queued for delivery in the system. The time listed is your local time as specified in your browser settings.
