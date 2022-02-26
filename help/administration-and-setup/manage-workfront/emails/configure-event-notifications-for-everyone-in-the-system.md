

# Configure event notifications for everyone in the system

Event notifications trigger emails to users when a certain event occurs. As an *Adobe Workfront administrator* or a user with a Planner access level, you can configure an event notification for all users in the system. Configuration of an event notification consists of activating or deactivating it

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
and customizing its email subject line
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  and customizing its email subject line</MadCap:conditionalText>`.

Depending on the event you enable and the user keeps enabled on their own profile, users receive instant, daily, or both instant and daily email notifications when an event occurs.

You first must specify which notifications you want all your users to receive in the Setup area of your *Workfront* instance. Once you activate a notification in the Setup area, it displays as activated for each user in their profile page.

After notifications are activated in the Setup area and they appear in the users' profile pages, individual users or another user with a Plan license can also configure the activated notifications in a user profile to control what notifications that specific user receives and how often. For more information, see [Activate or deactivate your own event notifications](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

For a list of all event notifications that you can activate and deactivate, see [Event notifications available in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

For information about unlocking an event notification so that *group administrators* can configure it for their groups, see [Unlock or lock configuration of event notifications for all groups](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) and [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Planner or higher, with administrative access to reminder notifications</p> <p>For information about giving a Plan user administrative access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Configure event notifications for all users

You must enable notifications in the Setup area of *Workfront* before users can enable or disable them in their profiles.

>[!TIP]
>
>`You cannot activate notifications for *Workfront Goals* from the Setup area.` Users `can activate these notifications only in their profiles. Users with Plan licenses can activate them for other users. For information about enabling *Workfront Goals* notifications for users, see` [Notifications: Goals](../../../workfront-basics/using-notifications/notifications-goals.md).

<ol data-mc-continue="false"> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Email</span> > <span class="bold">Notifications</span>.</li> 
 <li value="3"> Make sure the <span class="bold">Event Notifications</span> tab is open.</li> 
 <li value="4"> <p>.<draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the switch to the left of the event name to turn it on or off.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the switch to the left of the event name to turn it on or off.
   </MadCap:conditionalText></p> <p>To see the default notification status for an event, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.</p> </li> 
 <li value="5"> <p>(Optional) Click the name of an event notification to customize the subject line of the email notification.<br></p> <p>For more information about customizing the subject lines of email notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>.</p> </li> 
 <li value="6"> <p>(Optional) If you want to unlock configuration for an email notification so that <em>group administrators</em> can configure it separately for their groups, click the button <img src="assets/lock-toggle-button.png"> to the right of the notification to switch it to the unlocked position <img src="assets/unlock-toggle-button.png">.</p> <note type="note">
   This functionality is available initially only to customers on Cluster 4 as part of a phased roll-out. It will become available for other clusters shortly thereafter. This article will be updated as this occurs.
  </note> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md" class="MCXref xref">Unlock or lock configuration of event notifications for all groups</a>.</p> </li> 
</ol>

