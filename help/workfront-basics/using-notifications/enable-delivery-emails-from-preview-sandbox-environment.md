---
filename: enable-delivery-emails-from-preview-sandbox-environment
navigation-topic: notifications
title: Enable delivery of emails from the Preview Sandbox environment
description: Adobe Workfront disables all email communication from both the Preview and the Custom Refresh Sandbox environments. For information about the Preview Sandbox environment, see The Adobe Workfront Preview Sandbox Environment. For information about the Custom Refresh Sandbox environment, see The Adobe Workfront Custom Refresh Sandbox environment.
---

# Enable delivery of emails from the Preview Sandbox environment

*Adobe Workfront* disables all email communication from both the Preview and the Custom Refresh Sandbox environments. For information about the Preview Sandbox environment, see [The Adobe Workfront Preview Sandbox Environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). For information about the Custom Refresh Sandbox environment, see [The Adobe Workfront Custom Refresh Sandbox environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

If you want to receive the following email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings while you are logged into Preview:

* Email notifications triggered by event notifications
* Reminder notifications
* Automatic late or early reminder notifications
* Email invitations

You can do this for yourself or for any user that you have access to edit. For more information about the access needed to edit users, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Preview Sandbox environment. Neither you nor the *Workfront administrator* can enable report delivery or push notifications for the mobile app when you access the Preview Sandbox environment.
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
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Request</em> or higher to change your own setting</p> <p><em>Plan</em> to edit the setting for other users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level.</p> <p> For information about this access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>In your access level, Edit must be selected for the Users setting. And, for the Users setting, under Fine-tune your settings <img src="assets/gear-icon-in-access-levels.png"> , the Create option and at least one of the two User Admin options must be enabled. </p> <p>If you are using the User Admin (Group Users) option, you must be a <em>group administrator</em> of a group where the user is a member.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>For information about the Users setting in an access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Enable the delivery of emails from the Preview Sandbox environment

<ol> 
 <li value="1">Log in to your Preview Sandbox environment.</li> 
 <li value="2"> <p>Click your profile picture in the upper-right corner of <em>Adobe Workfront</em>. <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Then, click the 
     <span class="bold">More</span> menu and select 
     <span class="bold">Edit</span>. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Then, click the 
    <span class="bold">More</span> menu and select 
    <span class="bold">Edit</span>. 
   </MadCap:conditionalText></p> <p>Or</p> <p>Search for a user in <em>Workfront</em> and click their name. <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Then, click the 
     <span class="bold">More</span> menu and select 
     <span class="bold">Edit</span>. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Then, click the 
    <span class="bold">More</span> menu and select 
    <span class="bold">Edit</span>. 
   </MadCap:conditionalText></p> <p>Or</p> <p>For multiple users: <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
     <span class="bold">Main Menu</span> icon 
     <img src="assets/main-menu-icon.png"> in the upper-right corner of 
     <em>Workfront</em>, then click 
     <span class="bold">Users</span> 
     <img src="assets/users-icon-in-main-menu.png">. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Workfront</em>, then click 
    <span class="bold">Users</span> 
    <img src="assets/users-icon-in-main-menu.png">. 
   </MadCap:conditionalText> Then, select multiple users and click <span class="bold">Edit</span>.</p> </li> 
 <li value="3">Click <span class="bold">Preferences</span>.</li> 
 <li value="4"> <p>Select <span class="bold">Receive emails from this test environment</span>.</p> <note type="note">
   This option is not available if you are in a production environment.
  </note> </li> 
 <li value="5">Click <span class="bold">Save Changes</span>.</li> 
</ol>

