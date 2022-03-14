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

<table cellspacing="0"> 
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

## Viewand configure a group’s event notifications

1. Do any of the following:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Activate or deactivate an unlocked event notification</td> 
      <td> <p>Click the button in the <span class="bold">Active</span> column to activate <img src="assets/email-notification-enabled-unlocked.png"> or deactivate <img src="assets/email-notification-disabled-unlocked.png"> it.</p> <p>For example, you could configure the top two Marketing group event notifications shown below that have been unlocked for groups.</p>  
       <ul> 
        <li>If a button in the <span class="bold">Active</span> column is grey and dimmed <img src="assets/email-notification-disabled-locked.png">, the event notification is deactivated for all users and group administrators can’t activate it<!--
          or edit its email subject line
         --> for their groups.</li> 
        <li>If a button in the <span class="bold">Active</span> column is grey and not dimmed <img src="assets/email-notification-disabled-unlocked.png">, the event notification is <span class="bold" style="font-weight: normal;">deactivated for all users and</span> group administrators can activate it<!--
          or edit its email subject line
         --> for their groups.</li> 
       </ul> 
       <ul> 
        <li>If a button in the <span class="bold">Active</span> column is blue and dimmed <img src="assets/email-notification-enabled-locked.png">, the event notification is activated for all users and group administrators can’t deactivate it<!--
          or edit its email subject line
         --> for their groups.</li> 
        <li>If a button in the <span class="bold">Active</span> column is blue and not dimmed <img src="assets/email-notification-enabled-unlocked.png">, the event notification is <span class="bold" style="font-weight: normal;">activated for all users and</span> group administrators can deactivate it<!--
          or edit its email subject line
         --> for their groups.</li> 
       </ul> </td> 
     </tr> <!--
      Customize the email subject line of an event notification Click the name of the event notification. In the Event Notification box that displays, in the Email Subject Line box, change the text and fields, including custom fields, then click Update to save the new subject lines for your emails. Important: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the Adobe Workfront API. For more information about customizing the email subject line of an event notification, see Customize email subjects for event notifications.
     --> 
    </tbody> 
   </table>

