---
filename: enable-delivery-emails-from-preview-sandbox-environment
navigation-topic: notifications
title: Enable delivery of emails from the Preview Sandbox environment
description: Adobe Workfront disables all email communication from both the Preview and the Custom Refresh Sandbox environments. For information about the Preview Sandbox environment, see The Adobe Workfront Preview Sandbox Environment. For information about the Custom Refresh Sandbox environment, see The Adobe Workfront Custom Refresh Sandbox environment.
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
>Report delivery and push notifications on the mobile app are always disabled for the Preview Sandbox environment. Neither you nor the Workfront administrator can enable report delivery or push notifications for the mobile app when you access the Preview Sandbox environment.
>
>For information about report deliveries, see [Report delivery overview](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>Request or higher to change your own setting</p> <p>Plan to edit the setting for other users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level.</p> <p> For information about this access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>In your access level, Edit must be selected for the Users setting. And, for the Users setting, under Fine-tune your settings <img src="assets/gear-icon-in-access-levels.png"> , the Create option and at least one of the two User Admin options must be enabled. </p> <p>If you are using the User Admin (Group Users) option, you must be a group administrator of a group where the user is a member.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>For information about the Users setting in an access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Enable the delivery of emails from the Preview Sandbox environment

<ol> 
 <li value="1">Log in to your Preview Sandbox environment.</li> 
 <li value="2"> <p>Click your profile picture in the upper-right corner of Adobe Workfront. Then, click the More menu and select Edit.</p> <p>Or</p> <p>Search for a user in Workfront and click their name. Then, click the More menu and select Edit.</p> <p>Or</p> <p>For multiple users: Click the Main Menu icon in the upper-right corner of Workfront, then click Users . Then, select multiple users and click <span class="bold">Edit</span>.</p> </li> 
 <li value="3">Click <span class="bold">Preferences</span>.</li> 
 <li value="4"> <p>Select <span class="bold">Receive emails from this test environment</span>.</p> <note type="note">
   This option is not available if you are in a production environment.
  </note> </li> 
 <li value="5">Click <span class="bold">Save Changes</span>.</li> 
</ol>

