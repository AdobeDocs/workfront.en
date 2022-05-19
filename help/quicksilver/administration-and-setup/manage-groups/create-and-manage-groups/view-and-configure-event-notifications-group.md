---
filename: view-and-configure-event-notifications-group
user-type: administrator
product-area: system-administration;user-management
keywords: view,group,event,notifications,configure,enable,disable
navigation-topic: create-and-manage-groups
title: View and configure event notifications for a group
description: As an group administrator, you can view the event notifications that are activated for a group you manage.
---

# View and configure event notifications for a group

As an group administrator, you can view the event notifications that are activated for a group you manage.

Also, if a Adobe Workfront administrator unlocks an event notification, you can configure it for a top-level group that you manage. Configuration of an event notification consists of activating or deactivating it.

A Workfront administrator can also do this for any group.

Configuring an event notification for a group affects users for whom that group, or one of its subgroups, is their Home Group. In their user profiles, these users see the event notifications that are activated for their Home Group instead of the event notifications that are activated system-wide.

For information on how a Workfront administrator unlocks an event notification, see [Unlock or lock configuration of event notifications for all groups](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

For information about the default notification setting for an event, see [Event notifications available in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront license</a>*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## View and configure a group's event notifications

1. (Conditional and optional) If you are a Workfront administrator and you are already on the Email Notifications page (Setup > Email > Notifications), you can do the following and then skip to step 6: Delete **System Event Notifications** in the box above the list , start typing the group's name in the box, then click it when it appears.
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the top-level group.
1. In the left menu, click **Event notifications**.

   In the list that displays, the **Active** column on the left shows which notifications are active (blue) and inactive (grey) for the group.

1. Do any of the following:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Activate or deactivate an unlocked event notification</td> 
      <td> <p>Click the button in the <strong>Active</strong> column to activate <img src="assets/email-notification-enabled-unlocked.png"> or deactivate <img src="assets/email-notification-disabled-unlocked.png"> it.</p> <p>For example, you could configure the top two Marketing group event notifications shown below that have been unlocked for groups.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/configure-group-event-notifications-350x193.png" style="width: 350;height: 193;"> </p> 
       <ul> 
        <li>If a button in the <strong>Active</strong> column is grey and dimmed <img src="assets/email-notification-disabled-locked.png">, the event notification is deactivated for all users and group administrators can't activate it<!--
          <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
            or edit its email subject line
          </MadCap:conditionalText>
         --> for their groups.<!--
          <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Edit feature coming</span>
         --></li> 
        <li>If a button in the <strong>Active</strong> column is grey and not dimmed <img src="assets/email-notification-disabled-unlocked.png">, the event notification is <strong>deactivated for all users and</strong> group administrators can activate it<!--
          <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
            or edit its email subject line
          </MadCap:conditionalText>
         --> for their groups.</li> 
       </ul> 
       <ul> 
        <li>If a button in the <strong>Active</strong> column is blue and dimmed <img src="assets/email-notification-enabled-locked.png">, the event notification is activated for all users and group administrators can't deactivate it<!--
          <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
            or edit its email subject line
          </MadCap:conditionalText>
         --> for their groups.</li> 
        <li>If a button in the <strong>Active</strong> column is blue and not dimmed <img src="assets/email-notification-enabled-unlocked.png">, the event notification is <strong>activated for all users and</strong> group administrators can deactivate it<!--
          <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
            or edit its email subject line
          </MadCap:conditionalText>
         --> for their groups.</li> 
       </ul> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader"><span class="preview">Customize the email subject line of an event notification</span> </td> 
       <td> 
        <ol class="preview"> 
         <li value="1">Click the name of the event notification.</li> 
         <li value="2"> <p>In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.</p> <p>Important: The names of the fields added must match the camel case syntax of our database structure. <!--For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.--></p> <p>For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. </p> </li> 
        </ol> </td> 
      </tr>
     --> 
    </tbody> 
   </table>

