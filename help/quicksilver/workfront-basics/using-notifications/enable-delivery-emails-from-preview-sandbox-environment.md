---
navigation-topic: notifications
title: Enable delivery of emails from the Preview Sandbox environment
description: If you want to receive email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings while you are logged into Preview.
author: Courtney, Becky
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
---
# Enable delivery of emails from the Preview Sandbox environment

[!UICONTROL Adobe Workfront] disables all email communication from both the Preview and the Custom Refresh Sandbox environments. For information about the Preview Sandbox environment, see [The Adobe Workfront Preview Sandbox Environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). For information about the Custom Refresh Sandbox environment, see [The Adobe Workfront Custom Refresh Sandbox environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

If you want to receive the following email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings while you are logged into Preview:

* Email notifications triggered by event notifications
* Email invitations

You can do this for yourself or for any user that you have access to edit. For more information about the access needed to edit users, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Preview Sandbox environment. Neither you nor the [!DNL Workfront] administrator can enable report delivery or push notifications for the mobile app when you access the Preview Sandbox environment.
>
>For information about report deliveries, see [Report delivery overview](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td> 
   <p>Contributor or higher to change your own setting</p> <p>Standard to edit the setting for other users</p> 
   Or
   <p> Request or higher to change your own setting</p> <p>Plan to edit the setting for other users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The [!UICONTROL System Administrator] access level.</p> </li> 
     <li> <p>In your access level, [!UICONTROL Edit] must be selected for the [!UICONTROL Users] setting. And, for the [!UICONTROL Users] setting, under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> , the [!UICONTROL Create] option and at least one of the two [!UICONTROL User Admin] options must be enabled. </li> 
     <li>If you are using the [!UICONTROL User Admin (Group Users)] option, you must be a group administrator of a group where the user is a member.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Enable the delivery of emails from the Preview Sandbox environment

1. Log in to your Preview Sandbox environment.
1. Click your profile picture in the upper-right corner of [!DNL Adobe Workfront]. Then, click the **[!UICONTROL More]** menu and select **[!UICONTROL Edit]**.

   Or

   Search for a user in [!DNL Workfront] and click their name. Then, click the **[!UICONTROL More]** menu and select **[!UICONTROL Edit]**.

   Or

   For multiple users: Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **[!UICONTROL Users]** ![User icon](assets/users-icon-in-main-menu.png).  Then, select multiple users and click **[!UICONTROL Edit]**.

1. Click **[!UICONTROL Preferences]**.
1. Select **[!UICONTROL Receive emails from this test environment]**.

   >[!NOTE]
   >
   >This option is not available if you are in a production environment.

1. Click **[!UICONTROL Save Changes]**.
