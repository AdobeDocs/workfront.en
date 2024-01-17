---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Event notifications available in Adobe Workfront
description: Event notifications are emails triggered by various types of events on objects such as projects, tasks, and issues. This article lists and describes the available types of event notifications.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
---
# Event notifications available in Adobe Workfront

<!-- Audited: 1/2024 -->

Event notifications are emails triggered by various types of events on objects such as projects, tasks, and issues, as explained in [Event notifications](../../../workfront-basics/using-notifications/event-notifications.md).

These notifications can be configured at the system and group level:

* For information about configuring event notifications at the system level, see [Configure event notifications for everyone in the system](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* For information about configuring event notifications at the group level, see [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Individual users can also activate and deactivate their individual event notifications in their individual profile. For more information, see [Modify your own email notifications](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

The following tables list all of the Adobe Workfront event notifications, a brief description of the event, and whether the event is active or inactive by default.

## Action needed

See also [Notifications: Action needed](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th>Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>User</p> </td> 
   <td> <p>Access Request</p> </td> 
   <td> <p>User</p> </td> 
   <td> <p>Someone requests access from me.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> <p> </p> </td> 
   <td> <p>Document Request Add</p> </td> 
   <td> <p>User that document is requested from</p> </td> 
   <td> <p>Someone requested that I upload document(s).</p> <p>The Document Requestee receives an email notification when they get a request to upload a document.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document pending approval</p> </td> 
   <td> <p>Approvers</p> </td> 
   <td> <p>I need to approve a document.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Assignment</p> </td> 
   <td> <p>User that issue is assigned to</p> </td> 
   <td> <p>I'm assigned to an issue.</p> <p>The issue assignee receives an email notification only if the status of the project is Current and the status of the issue is not Closed or something that equates with Closed.</p> <p>Users with a Review or Request license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Pending Approval</p> </td> 
   <td> <p>Approvers</p> </td> 
   <td> <p>I need to approve an issue.</p> <p>Which users receive an email notification for this event depends on whether the "Approver not required to be on the project team (for approval processes that include a role)" setting is enabled (as described in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>). </p> <p>If this option is enabled</strong>, an email notification is sent to all users in the system with the "Approver" Job Role.</p> <p>If this option is disabled</strong>, only project team members with the "Approver" Job Role receive an email notification.</p> <p>A notification is sent if the project is in the Planning or Current status. </p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Pending Approval</p> </td> 
   <td> <p>Delegated Approver</p> </td> 
   <td> <p>I need to review an issue approval I"ve been delegated.</p> <p>When someone delegates an issue approval to another user, that user is notified. </p> <p>A notification is sent only when the project is in the Current status.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Pending Approval</p> </td> 
   <td> <p>Approvers</p> </td> 
   <td> <p>I need to approve a project.</p> <p>Which users receive an email notification for this event depends on whether the "Approver not required to be on the project team (for approval processes that include a job role)" setting is enabled (as described in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>).</p> <p>If this option is enabled</strong>, an email notification is sent to all users in the system with the "Approver" Job Role.</p> <p>If this option is disabled</strong>, only project team members with the "Approver" Job Role receive an email notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Project Pending Approval</td> 
   <td>Delegated Approver</td> 
   <td> <p>I need to review a project approval I've been delegated.</p> </td> 
   <td> Active</td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Assignment</p> </td> 
   <td> <p>User that task is assigned to</p> </td> 
   <td> <p>I'm set as the primary assignee of a task.</p> <p>The Task Assignee receives an email notification if they are made the primary assignee of the task, unless the assignee is the user who made the assignment.</p> <p>A notification is sent if the project status is Current and the task is not marked Complete.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Pending Approval</p> </td> 
   <td> <p>Approvers</p> </td> 
   <td> <p>I need to approve a task.</p> <p>Which users receive an email notification for this event depends on whether the "Approver not required to be on the project team (for approval processes that include a role)" setting is enabled (as described in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>). </p> <p>If this option is enabled</strong>, an email notification is sent to all users in the system with the "Approver" Job Role.</p> <p>If this option is disabled</strong>, only project team members with the "Approver" Job Role receive an email notification.</p> <p>A notification is sent only if the project status is Current at the time of the request.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Pending Approval</p> </td> 
   <td> <p>Delegated Approver</p> </td> 
   <td> <p>I need to review a task approval I've been delegated.</p> <p>When someone delegates an issue approval to another user, that user is notified. </p> <p>A notification is sent only if the project status is Current at the time of the request.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Timesheet</p> </td> 
   <td> <p>Timesheet Re-opened</p> </td> 
   <td> <p>User that timesheet belongs to</p> </td> 
   <td> <p>My timesheet is re-opened.</p> <p>The Timesheet Owner receives an email notification when the timesheet is re-opened, unless the user who re-opened the timesheet is also the owner of the timesheet.</p> <p>An email notification is sent only if the timesheet status is Open.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Timesheet</p> </td> 
   <td> <p>Timesheet Rejection</p> </td> 
   <td> <p>User that timesheet belongs to</p> </td> 
   <td> <p>My timesheet is rejected.</p> <p>The Timesheet Owner receives an email notification when the timesheet is rejected, unless the user who rejected the timesheet is also the owner.</p> <p>An email notification is sent only if the timesheet status is Rejected.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Timesheet</p> </td> 
   <td> <p>Timesheet Submission</p> </td> 
   <td> <p>Approver</p> </td> 
   <td> <p>I need to approve a timesheet.</p> <p>The Timesheet Approver receives an email notification when a timesheet that they need to approve is submitted, unless the user who submitted the timesheet is also the Timesheet Approver.</p> <p>A notification is sent only if the status of the timesheet is Submitted.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assignment</p> </td> 
   <td> <p>Work Item Request</p> </td> 
   <td> <p>Members of the team that the item is requested for</p> </td> 
   <td> <p>My team gets a new work request.</p> <p>Team Members receive an email notification when the team receives a new work request. (The user who submitted the request does not receive a notification if they are a member of the team.)</p> <p>A notification is sent only if the project status is Current at the time the Work Request is made and the Work Request status is New.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assignment</p> </td> 
   <td> <p>Work Item Request</p> </td> 
   <td> <p>User that work item is requested for</p> </td> 
   <td> <p>I get a new work request.</p> <p>The assignee of the work item receives an email notification, unless the user making the request is also the assignee. </p> <p>A notification is not sent if the task status is Complete or the issue status is Closed.</p> <p>A notification is sent only if the project status is Current at the time of the request.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requests I have made

See also [Notifications: Requests I have made](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Approval Status Change</p> </td> 
   <td> <p>Requestor</p> </td> 
   <td> <p>A document approval request is completed.</p> <p>The Document Requestor receives an email notification when the document approval request is completed.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Request Complete</p> </td> 
   <td> <p>Requestor</p> </td> 
   <td> <p>A document upload request is fulfilled.</p> <p>The Document Requestor receives an email notification when a request to upload a document is fulfilled.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>I add an issue to a project.</p> <p>The primary contact on an issue receives a notification when they add an issue in a project.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td>Issue</td> 
   <td>Issue Assignment</td> 
   <td>Issue Primary Contact</td> 
   <td> <p>Someone is assigned to an issue for which I'm the primary contact.</p> <p>The primary contact on an issue receives a notification when the issue is assigned to a user. </p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> Inactive</td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Completion</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>An issue for which I'm the primary contact is completed.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Status Change</p> </td> 
   <td> <p>User that created project (Entered By)</p> </td> 
   <td> <p>The status changes on a project I created.</p> <p>The user who created the project receives an email notification when the project status changes.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Request Add</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>I submit a request (confirmation).</p> <p>The Primary Contact on the issue receives an email notification when they submit an issue.</p> <p>A notification is sent only if the project status is Current and if the project is using a "Is Help Desk" View.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Request Assignment</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>Someone is assigned to my request.</p> <p>The primary contact of the issue receives an email notification when a user is assigned to the issue, unless the primary contact and the assigned user are the same user.</p> <p>A notification is sent only if the project status is Current and if the project is using a "Is Help Desk" View.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Request Closed</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>My request is closed (confirmation).</p> <p>The issue's primary contact receives an email notification when the request is closed.</p> <p>A notification is sent only if the project status is Current and if the project is using a "Is Help Desk" View.</p> <p>If the notifications for "issue completion" are enabled, they will always trigger instead of the "Request closed to Issue Primary Contact." If you want this notification to trigger, you must deactivate the "issue completion" notifications.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Request Document Add</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>A document is changed or uploaded on an issue for which I am the primary contact.</p> <p>The issue's primary contact receives an email notification when a document is uploaded or changed on the issue, unless the user who uploaded or changed the document is also the primary contact.</p> <p>A notification is sent only if the project status is Current and if the project has the "Publish as Help Request Queue" enabled on the Queue Setup tab.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Request Status Change</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>The status changes on my request.</p> <p>The primary contact of the issue receives an email notification when the issue status changes, unless the user who changed the status is also the primary contact.</p> <p>A notification is sent only if the project status is Current and the project is using a "Is Help Desk" View.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Communication

See also [Notifications: Communication](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Comment on Document</p> </td> 
   <td> <p>Document Owner</p> </td> 
   <td> <p>A comment is added on my document.</p> <p>The owner of a document in Workfront receives an email notification when a comment is posted on the document, unless the user who posted the comment is also the document owner.</p> <p>Any users who are directly included in the comment also receive an email notification.</p> <p>A notification is sent only if the project status is Current. </p> <p>The subject of the instant notification email is: <em>Comment on &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></p> <p> The subject of the daily digest notification is:<em> Digest of Communication &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>Active </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Request Note Add</p> </td> 
   <td> <p>Issue Primary Contact</p> </td> 
   <td> <p>When a comment is posted on a request, email the issue primary contact.</p> <p>The primary contact for an issue receives an email notification when a comment is posted on a request, unless the user who posted the comment is also the primary contact for the issue.</p> <p>Any users who are directly included on the comment also receive an email notification.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>User</p> </td> 
   <td>Directed Update</td> 
   <td>User</td> 
   <td> <p>Someone includes me on a directed update.</p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p> <p>In this case, the user who is included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only if the user has access rights to the object and if they keep it enabled in their profile.  </p> <p>This event notification is activated by default and cannot be deactivated.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Directed Update</p> </td> 
   <td> <p>Team members</p> </td> 
   <td> <p>Someone includes my team on a directed update.</p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p> <p>In this case, any member of the team that is included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only to users who have access rights to the object of the update.</p> <p>If the user sending the directed update is a member of the team being included, the user sending the update does not receive an email notification.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Work Item Comment</p> </td> 
   <td> <p>Thread Participants</p> </td> 
   <td> <p>Someone comments on a thread I'm in.</p> <p>Participants in the thread and users who are included in a direct message receive an email notification when a user makes a comment in the thread.</p> <p>Users must have View access to receive a notification.</p> <p>The following users do not receive a notification:</p> 
    <ul> 
     <li> <p>Teams that are included in a direct message</p> </li> 
     <li> <p>The owner of the Note</p> </li> 
     <li> <p>The Primary Contact</p> </li> 
    </ul> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Work Item Comment</p> </td> 
   <td> <p>Work Item Assignee</p> </td> 
   <td> <p>Someone comments on one of my work items.</p> <p>The assignee of the work item receives an email notification any time a user adds an update to a work item, unless the user who adds the update is also the assignee.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Work Request Reply</p> </td> 
   <td> <p> Work Requestor</p> </td> 
   <td> <p>Someone replies to my request.</p> <p>After a user submits a request and another user replies to that request, the user who submitted the request receives an email notification.</p> <p>An email notification is not sent if:</p> 
    <ul> 
     <li> <p>The user who replies is the same user who made the request</p> </li> 
     <li> <p>The user does not have access to see the note</p> </li> 
    </ul> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Approval information

See also [Notifications: Approval information](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>User</p> </td> 
   <td> <p>Approval Delegation</p> </td> 
   <td> <p>User</p> </td> 
   <td> <p>I'm delegated as an approver.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Delegated Issue Approval Status Change</p> </td> 
   <td> <p>User that delegated the approval</p> </td> 
   <td> <p>A delegated issue approval request is completed. </p> <p>When you delegate an issue approval to someone else, you receive an email notification when they finish that approval (whether they approve or reject the issue approval). </p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Delegated Project Approval Status Change</p> </td> 
   <td> <p>User that delegated the approval</p> </td> 
   <td> <p>A delegated project approval request is completed.</p> <p>When you delegate a project approval to someone else, you receive an email notification when they finish that approval (whether they approve or reject the project approval).</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Delegated Task Approval Status Change</p> </td> 
   <td> <p>User that delegated the approval</p> </td> 
   <td> <p>A delegated task approval status is completed.</p> <p>When you delegate a task approval to someone else, you receive an email notification when they finish that approval (whether they approve or reject the task approval).</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Approval Cancel to Approver</p> </td> 
   <td> <p>User that delegated the approval</p> </td> 
   <td> <p>A document approval request is canceled.</p> <p>The Document Approver of the document receives an email notification when the document approval request is canceled.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Timesheet</p> </td> 
   <td> <p>Timesheet Approval</p> </td> 
   <td> <p>User that timesheet belongs to</p> </td> 
   <td> <p>My timesheet is approved.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information about work assigned to me

See also [Notifications: Information about work assigned to me](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Task</td> 
   <td>All Predecessor Task Completion</td> 
   <td>Members of the team assigned to dependent tasks</td> 
   <td> <p>All predecessors of the team's tasks are completed.</p> <p>The task assignees (all members of the team) receive an email notification.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td>Inactive</td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>All Predecessor Task Completion</p> </td> 
   <td> <p>User assigned to dependent tasks</p> </td> 
   <td> <p>All predecessors of my tasks are completed.</p> <p>The task assignee receives an email notification.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Approval decision</p> </td> 
   <td> <p>User that the issue is assigned to</p> </td> 
   <td> <p>An issue I resolve is approved or rejected.</p> <p>The assignee of an issue receives an email notification when an approval decision is made (approved or rejected).</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Approval decision</p> </td> 
   <td> <p>User that the task is assigned to</p> </td> 
   <td> <p>A task I complete is approved or rejected.</p> <p>The task assignee receives an email notification when the task is approved or rejected.</p> <p>A notification is sent only if the project status is Current.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Completion</p> </td> 
   <td> <p>User that the issue is assigned to</p> </td> 
   <td> <p>An issue I'm assigned to is completed.</p> <p>A notification is sent only if the project status is Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Planned Completion Date changed</p> </td> 
   <td> <p>User that the issue is assigned to</p> </td> 
   <td> <p>The due date changes on an issue I'm assigned to.</p> <p>The issue assignee receives an email notification when the Planned Completion Date changes, unless the user who changed the Planned Completion Date is also the assignee.</p> <p>A notification is sent only if the project status is anything other than Planning.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Status Change</p> </td> 
   <td> <p>User that the issue is assigned to</p> </td> 
   <td> <p>The status changes on one of my work items.</p> <p>The assignee of the issue receives an email notification when the status changes, unless the user who changed the status is also the assignee.</p> <p>A notification is sent only if the project status is Current.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Request Document Add</p> </td> 
   <td> <p>User that the issue is assigned to</p> </td> 
   <td> <p>Documents are uploaded or changed on requests I'm assigned to.</p> <p>The issue assignee receives an email notification when documents are uploaded or changed on an issue they added.</p> <p>An email notification is not sent if the user who entered the issue is the issue assignee.</p> <p>A notification is sent only if the project status is Current and if the project has the "Publish as Help Request Queue" enabled on the Queue Setup tab.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Completion</p> </td> 
   <td> <p>User that the task is assigned to</p> </td> 
   <td> <p>A task I'm assigned to is completed.</p> <p>The Task Assignee receives an email notification when the task is completed. Notifications are not sent when a personal task is completed.</p> <p>A notification is sent only if the project status is Current.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Completion</p> </td> 
   <td> <p>User assigned to dependent task</p> </td> 
   <td> <p>A predecessor of one of my tasks is completed.</p> <p>The task assignee receives an email notification when one of their task's predecessors has been completed.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Planned Completion Date Changed</p> </td> 
   <td> <p>User that the task is assigned to</p> </td> 
   <td> <p>The due date changes on a task I'm assigned to.</p> <p>The Task Assignee receives an email notification when the Planned Completion Date of the task changes, unless the user who changed the Planned Completion Date is also the Task Assignee.</p> <p>A notification is sent only if the project status is anything other than Planning.</p> <p>No notification is sent regarding personal tasks.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Status Change</p> </td> 
   <td> <p>User that the task is assigned to</p> </td> 
   <td> <p>The status changes on a task I'm assigned to.</p> <p>The Task Assignee receives an email notification when the status of the task changes, unless the user who changed the status is also the assignee.</p> <p>A notification is sent only if the project status is Current.</p> <p>Users with a Review license do not receive a notification. </p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Information about projects I'm on

See also [Notifications: Information about projects I'm on](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Current Project Status</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>A project I'm on becomes active.</p> <p>Users on the project receive an email notification when the project becomes active.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Add</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>A document is added to a project I'm on.</p> <p>Users on the project team receive an email notification when a document is added to the project, except for the user who added the document.</p> <p>A notification is sent only if the project status is Current and the document is not Private. </p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>An issue is added to a project I'm on.</p> <p>Users in a project receive an email notification when an issue is added to the project.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Completion</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>An issue is completed on a project I'm on.</p> <p>Any user on the project receives a notification.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Milestone Task Completion</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>A milestone task is completed on a project I'm on.</p> <p>All users on the Project Team receive a notification when a milestone task is completed. </p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Completion</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>A project I'm on is completed.</p> <p>Users on a project team receive an email notification when the project status is Complete.</p> <p>Tip: If projects are completed regularly, enabling this option can create a lot of email for users who have a limited number of tasks on many projects. </p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Status Change</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>The status changes on a project I'm on.</p> <p>Users on the Project Team receive an email notification when the status of the project changes. </p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project User</p> </td> 
   <td> <p>Project User Add</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>I'm added to a project.</p> <p>The user who was added to the project receives an email notification when they are added, unless the user was self-added to the project.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Completion</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>A task is completed on a project I'm on.</p> <p>Members of the project team receive an email notification.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Unassigned Issue Added</p> </td> 
   <td> <p>Members of project team</p> </td> 
   <td> <p>An unassigned issue is added to a project I'm on.</p> <p>Users on a project receive an email notification when an unassigned issue is added to the project.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information about projects I own

See also [Notifications: Information about projects I own](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Add</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>A document is added to a project I own.</p> <p>The Project Owner receives an email notification when a document is added to the project, unless the user who added the document is also the Project Owner.</p> <p>A notification is sent only if the project status is Current and the document is not Private.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>An issue is added to a project I own.</p> <p>The Project Owner receives an email notification when an issue is added to the project.</p> <p>A notification is sent only if the project status is Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Commit Date Change</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>The commit date changes for an issue on one of my projects.</p> <p>The Project Owner receives an email notification when the Commit Date changes for an issue on the project, unless the user who changes the Commit Date is the same user as the Project Owner.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Completion</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>An issue is completed on a project I own.</p> <p>The project owner receives an email notification.</p> <p>A notification is sent only if the project status is Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Milestone Task Completion</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>A milestone task is completed on a project I own.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Owner Assignment</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>I'm set as the owner of a new project.</p> <p>When a user is assigned as the owner of a project, that user receives an email notification.</p> <p>If the project owner is the same user who made the assignment, an email notification is not sent</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Progress Change</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>A project I own gets behind.</p> <p>The project owner receives an email notification when the project is behind schedule.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Commit Date Change</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>The commit date changes for a task on one of my projects.</p> <p>The Project Owner receives an email notification when the Commit Date changes for a task on the project, unless the user who changed the Commit Date is also the Project Owner.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Completion</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>A task is completed on a project I own.</p> <p>The project owner receives a notification. </p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Progress Change</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>A task on a project I own gets behind.</p> <p>The Project Owner receives an email notification when a task on the project gets behind schedule.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Unassigned Issue Add</p> </td> 
   <td> <p>Project Owner</p> </td> 
   <td> <p>An unassigned issue is added to a project I own.</p> <p>The Project Owner receives an email notification when an unassigned issue is added to the project.</p> <p>A notification is sent only if the project status is Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information about projects I sponsor

See also [Notifications: Information about projects I sponsor](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Add</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>A document is added to a project I sponsor.</p> <p>The Project Sponsor receives an email notification when a document is added to the project, unless the document is added by the Project Sponsor.</p> <p>A notification is sent only if the project status is Current and if the document is not Private.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>An issue is added to a project I sponsor.</p> <p>The Project Sponsor receives an email notification when an issue is added to the project.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Completion</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>An issue is completed on a project I sponsor.</p> <p>The project sponsor receives an email notification.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Milestone Task Completion</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>A milestone task is completed on a project I sponsor.</p> <p>The Project Sponsor receives an email notification when a milestone task is completed on a project they sponsor.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Progress Change</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>A project I sponsor gets behind.</p> <p>The Project Sponsor receives an email notification when the project gets behind schedule.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project Sponsor Assignment</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>I'm set as the sponsor of a project.</p> <p>The project sponsor receives an email notification when they are set as the sponsor of a project.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Completion</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>A task is completed on a project I sponsor.</p> <p>The project sponsor receives an email notification.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Progress Change</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>A task on a project I sponsor gets behind.</p> <p>The Project Sponsor receives an email notification when a task on the project gets behind schedule.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Unassigned Issue Add</p> </td> 
   <td> <p>Project Sponsor</p> </td> 
   <td> <p>An unassigned issue is added to a project I sponsor.</p> <p>The Project Sponsor receives an email notification when an unassigned issue is added to the project.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>

## Miscellaneous information

See also [Notifications: Miscellaneous information](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Type</th> 
   <th>Event</th> 
   <th>Recipient</th> 
   <th>Description</th> 
   <th> Default state</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Announcement</td> 
   <td> <p>Announcement was added</p> </td> 
   <td> <p></p> </td> 
   <td> <p>A message is sent to the Announcement Center.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document Request Cancel</p> </td> 
   <td> <p>User that document is requested from</p> </td> 
   <td> <p>Cancel a document upload request from me.</p> <p>The Document Requestee receives an email notification when a document request is canceled.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Error Notification</p> </td> 
   <td> <p></p> </td> 
   <td> <p>An error was found that needs your attention.</p> <p>An email notification is generated after Workfront tries and fails to connect to a POP account. After 25 tries, Workfront disables the connection to the POP account in order to preserve resources and it sends out a notification. </p> <p>The email notification is sent to the Project Owner, if the POP email is associated with a request queue, or to the Workfront administrators, if the POP account is associated with the "Incoming Mail" feature in Email Setup.
   </p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Issue</p> </td> 
   <td> <p>Issue Assignment</p> </td> 
   <td> <p>Resource Owner</p> </td> 
   <td> <p>An issue assignment change affects one of my people.</p> <p>The Issue Assignee Manager receives an email notification when a change affects a user they manage.</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>User</p> </td> 
   <td> <p>New User</p> </td> 
   <td> <p>User</p> </td> 
   <td> <p>When a new user is created in Workfront, email the user.</p> <p>After the new user is created, the user receives an email invitation, notifying them that a Workfront account has been created and prompting them to set their password.</p> <p>When creating a new user, users can select the option "Send an invite email to this person" (as described in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a><span style="font-weight: 400;">). However, when the "New User to User" option is enabled globally, all new users receive the email invitation regardless of whether the "Send an invite email to this person" option is selected.</span></p> </td> 
   <td> Inactive </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Object Share</p> </td> 
   <td> <p>Members of team that object was shared with</p> </td> 
   <td> <p>Someone shares an object with my team.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>User</p> </td> 
   <td> <p>Object Share</p> </td> 
   <td> <p>User that object was shared with</p> </td> 
   <td> <p>Someone shares an object with me.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project User</p> </td> 
   <td> <p>Project User Add</p> </td> 
   <td> <p>Resource Owner</p> </td> 
   <td> <p>One of my people is added to a project.</p> <p>A manager receives an email notification when one of his or her direct reports is added to a project.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>Project added to a portfolio or program</p> </td> 
   <td> <p>Portfolio or Program Owner</p> </td> 
   <td> <p>Someone adds a project to a portfolio or program I own.</p> </td> 
   <td> <p>Active</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task</p> </td> 
   <td> <p>Task Assignment</p> </td> 
   <td> <p>Resource Owner</p> </td> 
   <td> <p>A task assignment change affects one of my people.</p> <p>The Task Assignee's Manager receives an email notification.</p> <p>A notification is sent only if the project status is Current.</p> </td> 
   <td> <p>Inactive</p> </td> 
  </tr> 
  <tr> 
   <td> Project <br>Task <br>Issue</td> 
   <td>New Update</td> 
   <td>Subscriber </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">An email is sent when an update is made to a task, issue, or project that I am subscribed to.</span> </p> </td> 
   <td>Active</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Delegation

See also [Notifications: Delegation](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Object Type      | Event                        | Recipient               | Description                                                  | Default state |
|------------------|------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Tasks and issues | Task and issue delegation |Assignee       | I delegate my tasks and issues (confirmation)                | Active        |
| Tasks and issues | Stop task and issue delegation | Assignee  | I stop the delegation of my tasks and issues (confirmation)  | Active        |
| Tasks and issues | Task and issue delegation | Delegate       | Someone delegates their tasks and issues to me               | Active        |
| Tasks and issues | Stop tasks and issue delegation | Delegate | Someone stops the delegation of their tasks and issues to me | Active        |
