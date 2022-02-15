---
filename: view-and-configure-event-notifications-group
user-type: administrator
product-area: system-administration;user-management
keywords: view,group,event,notifications,configure,enable,disable
navigation-topic: create-and-manage-groups
---



# View and configure event notifications for a group {#view-and-configure-event-notifications-for-a-group}

As an *`group administrator`*, you can view the event notifications that are activated for a group you manage.


Also, if a *`Adobe Workfront administrator`* unlocks an event notification, you can configure it for a top-level group that you manage. Configuration of an event notification consists of activating or deactivating it.


A *`Workfront administrator`* can also do this for any group.


Configuring an event notification for a group affects users for whom that group, or one of its subgroups, is their Home Group. In their user profiles, these users see the event notifications that are activated for their Home Group instead of the event notifications that are activated system-wide.


For information on how a *`Workfront administrator`* unlocks an event notification, see [Unlock or re-lock configuration of event notifications for groups](unlock-configuration-of-event-notifications-for-groups.md).


For information about the default notification setting for an event, see [Event notifications available in Adobe Workfront](event-notifications-available-in-wf.md). 


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## View`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  and configure</MadCap:conditionalText>` a group’s event notifications {#view-and-configure-a-group-s-event-notifications}




1. (Conditional and optional) If you are a *`Workfront administrator`* and you are already on the Email Notifications page (Setup > Email > Notifications), you can do the following and then skip to step 6: Delete `System Event Notifications` in the box above the list , start typing the group’s name in the box, then click it when it appears.

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1. Click the name of the top-level group.
1.  In the left menu, click `Event notifications`.


   In the list that displays, the `Active`column on the left shows which notifications are active (blue) and inactive (grey) for the group.

1.  Do any of the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Activate or deactivate an unlocked event notification</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Click the button in the <span class="bold">Active </span>column to activate <img src="assets/email-notification-enabled-unlocked.png"> or deactivate <img src="assets/email-notification-disabled-unlocked.png"> it.</p> <p>For example, you could configure the top two Marketing group event notifications shown below that have been unlocked for groups.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/configure-group-event-notifications-350x193.png" style="width: 350;height: 193;"> </p> 
    <ul> 
     <li>If a button in the <span class="bold">Active</span> column is grey and dimmed <img src="assets/email-notification-disabled-locked.png">, the event notification is <span class="bold" style="font-weight: normal;">deactivated for all users and </span><span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can’t activate it for their groups.</li> 
     <li>If a button in the <span class="bold">Active</span> column is grey and not dimmed <img src="assets/email-notification-disabled-unlocked.png">, the event notification is <span class="bold" style="font-weight: normal;">deactivated for all users and</span> <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can activate it for their groups.</li> 
    </ul> 
    <ul> 
     <li>If a button in the <span class="bold">Active</span> column is blue and dimmed <img src="assets/email-notification-enabled-locked.png">, the event notification is <span class="bold" style="font-weight: normal;">activated for all users and </span><span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can’t deactivate it for their groups.</li> 
     <li>If a button in the <span class="bold">Active</span> column is blue and not dimmed <img src="assets/email-notification-enabled-unlocked.png">, the event notification is <span class="bold" style="font-weight: normal;">activated for all users and</span> <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can deactivate it for their groups.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>




