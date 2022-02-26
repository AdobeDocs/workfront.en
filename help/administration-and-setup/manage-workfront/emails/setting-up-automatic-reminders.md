---
filename: setting-up-automatic-reminders
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Set up automatic reminders
description: As an Adobe Workfront administrator, you can set up automatic reminders to trigger email notifications when all tasks or issues are due, late, or near the planned completion date. After you configure these settings, users cannot disable automatic reminders.
---

# Set up automatic reminders

As an *Adobe Workfront administrator*, you can set up automatic reminders to trigger email notifications when all tasks or issues are&nbsp;due, late, or near the planned completion date. After you configure these settings, users cannot disable automatic reminders.

For late notifications, the email is sent nightly until the task or issue is completed.

An automatic reminder can be sent to one or more of the following:

* The users assigned to a task or issue
* The user's immediate manager
* The manager of the immediate manager

>[!NOTE]
>
>You cannot change the content or the subject line of the email triggered by an automatic reminder.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set up automatic reminders

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Email</span> ><span class="bold">Automatic Reminders</span>.</li> 
 <li value="3"> <p>In the <span class="bold">Send a late notification to</span> area, select any of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">The 'Assigned To' user</span> </td> 
     <td>Select this option if you want the user assigned to a task or issue to receive a late notification about their work item being late.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">The user's manager</td> 
     <td>Select this option if you want the user's manager to receive a late notification about their direct report's work item being late.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">The manager's manager</td> 
     <td>Select this option if you want the immediate manager's manager&nbsp;to receive a late notification about a&nbsp;work item of one of their direct report's users being late.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">The 'Assigned To' user</td> 
     <td>(In he <span class="bold">Send deadline reminder to</span> area.) Select this option if you want the user assigned to a task or an issue to receive a notification about their work item approaching the&nbsp;due date.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Select the time&nbsp;for the automatic reminder to send by selecting the amount of time before or after the due date of the work item.</p> <p>The time is calculated from the Planned Completion Date of the task or issue.<br></p> <p>Specify the number of minutes, hours, days, weeks, or months to add time to the Planned Completion Date of the tasks or issues. Select <span class="bold">Elapsed Minutes</span>, <span class="bold">Elapsed Hours</span>, <span class="bold">Elapsed Days</span>, or <span class="bold">Elapsed Weeks</span> to add time that includes any weekends,&nbsp;holidays, and non-working hours as indicated in your schedule.<br></p> <p>For example, if a task is assigned on Friday and&nbsp;has a duration of 3 elapsed days, the task completion date is set for Monday (assuming that Saturday and Sunday is a weekend). If the task has a duration of 3 days (not elapsed), the&nbsp;task completion date is set for Wednesday.<br></p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/time-increments-for-automatic-reminder-qs-350x180.png" style="width: 350;height: 180;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/time-increments-for-automatic-reminder-qs-350x180.png" style="width: 350;height: 180;"> </p> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

## Receive automatic reminders

If you are the designated entity in an Automatic Reminder notification, you receive an email when the specified deadline is met. For late notifications, the email is sent nightly until the task or issue is completed.

Tasks with certain dependency types may deliver after the specified start date, even though they are past due. For example, if a task has a predecessor with a Finish-Start (fs) dependency, it won't be included in the email, even if it's passed the specified start date, because you can't start the task until the predecessor is complete.

For more information about receiving Automatic Reminders emails, see the [Automatic reminders](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) section in [Adobe Workfront notifications](../../../workfront-basics/using-notifications/wf-notifications.md).

## Send automatic reminders

Automatic reminders are sent as soon as the time selected by the *Workfront administrator* is met.

If you want to trigger sending the automatic reminder emails manually, you can do so by using Diagnostics. For more information about accessing and using Diagnostics in *Workfront*, see [Use Diagnostics to trigger automated processes](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
