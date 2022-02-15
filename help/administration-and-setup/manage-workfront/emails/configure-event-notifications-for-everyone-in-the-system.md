


# Configure event notifications for everyone in the system {#configure-event-notifications-for-everyone-in-the-system}

Event notifications trigger emails to users when a certain event occurs. As an *`Adobe Workfront administrator`* or a user with a Planner access level, you can configure an event notification for all users in the system. Configuration of an event notification consists of activating or deactivating it`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  and customizing its email subject line</MadCap:conditionalText>`.


Depending on the event you enable and the user keeps enabled on their own profile, users receive instant, daily, or both instant and daily email notifications when an event occurs.


You first must specify which notifications you want all your users to receive in the Setup area of your *`Workfront`* instance. Once you activate a notification in the Setup area, it displays as activated for each user in their profile page. 


After notifications are activated in the Setup area and they appear in the users' profile pages, individual users or another user with a Plan license can also configure the activated notifications in a user profile to control what notifications that specific user receives and how often. For more information, see [Activate or deactivate your own event notifications](activate-or-deactivate-your-own-event-notifications.md).


For a list of all event notifications that you can activate and deactivate, see [Event notifications available in Adobe Workfront](event-notifications-available-in-wf.md).


For information about unlocking an event notification so that *`group administrators`* can configure it for their groups, see [Unlock or re-lock configuration of event notifications for groups](unlock-configuration-of-event-notifications-for-groups.md) and [View and configure event notifications for a group](view-and-configure-event-notifications-group.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Planner or higher, with administrative access to reminder notifications</p> <p>For information about giving a Plan user administrative access, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Configure event notifications for all users {#configure-event-notifications-for-all-users}

You must enable notifications in the Setup area of *`Workfront`* before users can enable or disable them in their profiles.


>[!TIP] {type="tip"}
>
>`You cannot activate notifications for *`Workfront Goals`* from the Setup area.` `Users` `can activate these notifications only in their profiles. Users with Plan licenses can activate them for other users. For information about enabling *`Workfront Goals`* notifications for users, see` [Notifications: Goals](notifications-goals.md).





1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Email` > `Notifications`.

1.  Make sure the `Event Notifications` tab is open.
1.  .`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the switch to the left of the event name to turn it on or off.</MadCap:conditionalText>`


   To see the default notification status for an event, see [Event notifications](event-notifications.md).

1.  (Optional) Click the name of an event notification to customize the subject line of the email notification.  



   For more information about customizing the subject lines of email notifications, see [Customize email subjects for event notifications](custom-email-subjects-event-notification.md).

1.  (Optional) If you want to unlock configuration for an email notification so that *`group administrators`* can configure it separately for their groups, click the button ![](assets/lock-toggle-button.png) to the right of the notification to switch it to the unlocked position ![](assets/unlock-toggle-button.png).


   >[!NOTE]
   >
   >This functionality is available initially only to customers on Cluster 4 as part of a phased roll-out. It will become available for other clusters shortly thereafter. This article will be updated as this occurs.


   For more information, see [Unlock or re-lock configuration of event notifications for groups](unlock-configuration-of-event-notifications-for-groups.md).



