---
navigation-topic: notifications
title: Enable delivery of emails from the Preview Sandbox environment
description: If you want to receive email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings while you are logged into Preview.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
---
# Enable delivery of emails from the Preview Sandbox environment

Adobe Workfront disables all email communication from both the Preview and the Custom Refresh Sandbox environments. For information about the Preview Sandbox environment, see [The Adobe Workfront Preview Sandbox Environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). For information about the Custom Refresh Sandbox environment, see [The Adobe Workfront Custom Refresh Sandbox environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

If you want to receive the following email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings while you are logged into Preview:

* Email notifications triggered by event notifications
* Reminder notifications
* Automatic late or early reminder notifications
* Email invitations

You can do this for yourself or for any user that you have access to edit. For more information about the access needed to edit users, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Preview Sandbox environment. Neither you nor the [!DNL Workfront] administrator can enable report delivery or push notifications for the mobile app when you access the Preview Sandbox environment.
>
>For information about report deliveries, see [Report delivery overview](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Request or higher to change your own setting</p> <p>Plan to edit the setting for other users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level.</p> <p> For information about this access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>In your access level, [!UICONTROL Edit] must be selected for the Users setting. And, for the Users setting, under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> , the [!UICONTROL Create] option and at least one of the two User Admin options must be enabled. </p> <p>If you are using the [!UICONTROL User Admin (Group Users)] option, you must be a group administrator of a group where the user is a member.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>For information about the Users setting in an access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Enable the delivery of emails from the Preview Sandbox environment

1. Log in to your Preview Sandbox environment.
1. Click your profile picture in the upper-right corner of Adobe Workfront. Then, click the **[!UICONTROL More]** menu and select **Edit**.

   Or

   Search for a user in [!DNL Workfront] and click their name. Then, click the **[!UICONTROL More]** menu and select **Edit**.

   Or

   For multiple users: Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Users** ![](assets/users-icon-in-main-menu.png).  Then, select multiple users and click **Edit**.

1. Click **Preferences**.
1. Select **[!UICONTROL Receive emails from this test environment]**.

   >[!NOTE]
   >
   >This option is not available if you are in a production environment.

1. Click **Save Changes**.
