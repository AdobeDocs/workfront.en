

# Set up reminder notifications

Reminder notifications send emails to recipients based on specified criteria. As an Adobe Workfront administrator or a user with a Planner access level and administrative access to reminder notifications, you can manually associate reminder notifications with your work items, such as projects, tasks, issues, and timesheets.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Planner or higher, with administrative access to reminder notifications</p> <p>For information about giving a Plan user administrative access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Customize the reminder email

You can customize the reminder notification with a custom email that includes a custom email subject and body. The email body can contain custom HTML.

Or, you can use the default email included with the reminder notification. The default email uses the reminder notification name as the email subject and the object name in the email body, including the event that triggered the notification.

If you want to customize the reminder email, you need to&nbsp;create&nbsp;an email template and attach&nbsp;it to the reminder notification.

For information about how to create an email template, see [Configure email templates](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Create&nbsp;a reminder notification

1. Click `Email` > `Notifications`.

1. Click the `Reminder Notifications` tab, then click `New Reminder Notification`.

1. In the drop-down list, click&nbsp;the&nbsp;object type you want to associate with the reminder notification.

   For example, if you want to attach a reminder notification to a timesheet, click `Timesheet`.

1. In the `New Reminder Notification` box that appears, specify the following information.

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Reminder Notification Name</td> 
      <td>Specify a name for the reminder notification.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Qualifying Period</td> 
      <td> <p>Specify the number of hours, work days, days (calendar days), weeks, or months before or after the date in the <span class="bold">Timing</span> field.</p> <p>Note:  
        <ul> 
         <li> <p>Reminder notifications begin 24 hours after the specified date and once all criteria are met.</p> </li> 
         <li> <p>Reminder notifications for projects, tasks, and issues trigger every night at midnight, US Mountain Time. All objects that qualify for a reminder notification from that day trigger a notification to the designated users shortly after that time.</p> </li> 
         <li> <p>Reminder notifications for timesheets are sent at the specified time based on your time zone and the timesheet's End Date, Start Date, or Last Update Date.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Select the event that triggers the reminder notification to be scheduled.</p> <p>If the reminder notification is intended for projects, tasks, or issues, the available options are related to the Completion Date or Start Date. The reminder notification takes into account the time stamp on the Completion and Start Dates of projects, tasks and issues.</p> <p>If the reminder notification is intended for Timesheets, the available options are related to the End Date, Start Date, or Last Update Date. The reminder notification for Timesheets takes into account the time stamp of the timesheet End, Start and Last Update Date. The Timesheet starts at midnight on the day of the Start Date (12:00 AM) and ends right before midnight on the End Date (11:59 PM).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criteria</td> 
      <td> <p>Select the criteria to qualify the reminder notification to be scheduled. Reminder notifications are not scheduled unless the criteria selection is met.</p> <p>The following criteria options are available, depending on the object type that you&nbsp;selected in Step 4:</p> 
       <ul> 
        <li><span class="bold">Incomplete in Current Projects:</span>&nbsp;(Available for task and issue reminders) The reminder notification is scheduled to be sent only when the object status that the reminder notification is associated with is not Complete and the project status is Current.</li> 
        <li><span class="bold">All in Current Projects:&nbsp;</span>(Available for task and issue reminders) The reminder notification is scheduled to be sent regardless of the object status and only when the project status that the reminder notification is associated with is Current.</li> 
        <li><span class="bold">Incomplete Projects:</span> (Available for project reminders) The reminder notification is scheduled to be sent when the project status is anything but Complete.</li> 
        <li><span class="bold">Complete Projects:</span> (Available for project reminders) The reminder notification is scheduled to be sent when the project status is Complete.</li> 
        <li><span class="bold">Open Timesheets:</span> (Available for timesheet reminders) The reminder notification is scheduled to be sent when the timesheet status is Open.</li> 
        <li><span class="bold">Submitted Timesheets:</span> (Available for timesheet reminders) The reminder notification is scheduled to be sent when the timesheet status is Submitted.</li> 
        <li><span class="bold">Open Timesheet or Less than 40 Hours per Week:</span> (Available for timesheet reminders) The reminder notification is scheduled to be sent when the timesheet status is Open or when the timesheet has less than 40 hours logged.</li> 
        <li><span class="bold">Email Template:</span>&nbsp;From the drop-down, select an email template to attach to your reminder.<br>For information on how to build an email template, refer to <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configure email templates</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recipients</td> 
      <td>Select the types of&nbsp;users you want to&nbsp;receive the notification. Select from various object stakeholders, such as owner, approver, or assignee.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click `Save`.
1. Attach the reminder notification to a work item, as described in [Attach a reminder notification to an object](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Receive a reminder notification

When the condition is met on the item which has&nbsp;the reminder notification attached, an email notification is triggered to the user defined in the reminder notification.

For more information about receiving&nbsp;reminder notifications, see the [Reminder notifications](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) section in [Adobe Workfront notifications](../../../workfront-basics/using-notifications/wf-notifications.md).

## Test reminder notification delivery

Reminder notifications trigger every night at midnight, Mountain Time. All the objects that qualify for a reminder notification trigger a notification to the designated users shortly&nbsp;after that.

To cause reminder notifications to trigger manually, the condition for the reminder&nbsp;must first be met.  
For instance, if a reminder is set to trigger an hour after the Planned Completion Date&nbsp;of a project, that time must&nbsp;have passed between when the reminder was set and now.&nbsp;Any projects that had planned completion dates passed before the reminder was activated will not trigger a notification.

To cause a reminder notification to trigger manually:

1. Click  `System` > `Diagnostics` in the lower left corner of Workfront. 

1. Click `Send Reminder Notifications` and wait for the confirmation at the top of the screen that they have been sent.

   The users&nbsp;designated in the reminder notification receive an email.

