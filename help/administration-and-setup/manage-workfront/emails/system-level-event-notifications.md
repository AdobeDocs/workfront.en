



# System-level event notifications {#system-level-event-notifications}

As a `Workfront administrator`, you can enable event notifications that send email notifications for various types of events in your organization. For more information, see [Enable and disable event notifications](enable-and-disable-event-notification.md).


When you enable event notifications at the system level, email notifications are enabled for all users in the system. Depending on which event you enable, users receive instant, daily, or both instant and daily email notifications for the specified event.&nbsp;Users can configure in their user profile what notifications they want to receive.&nbsp;For more information, see [Configure email notifications](configure-email-notifications.md).


The following table lists all of the event notifications that a `Workfront administrator` can enable at the system level, a brief description of the event, and whether the event is active or inactive by default:


## Action needed {#action-needed}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 1112px;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 170px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 190px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Access Request to User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Someone requests access from me.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>&nbsp;</p> <p>Document</p> <p>&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document Request Add to Requestee</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Request me to upload document(s).</p> <p>The Document Requestee receives an email notification when he or she receives a request to upload a document.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document pending approval to approvers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I need to approve a document.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Assignment to Issue Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I'm assigned to an issue.</p> <p>The issue assignee receives an email notification only if the status of the project is Current and the status of the issue is not Closed or something that equates with Closed.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Pending Approval to Approvers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I need to approve an issue.</p> <p>Which users receive an email notification for this event depends&nbsp;on whether the&nbsp;'Approver not&nbsp;required to be on the project team (for approval processes&nbsp;that include a role)' setting is enabled (as described in&nbsp;<a href="establish-approval-settings.md" class="MCXref xref">Establish approval settings</a>).&nbsp;</p> <p><b>If this option is enabled</b>, an email notification is sent to all users in the system with the 'Approver' Job Role.</p> <p><b>If this option is disabled</b>, only project team members with the 'Approver' Job Role receive an email notification.</p> <p>A notification is sent if the project is in the Planning or Current status. </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Pending Approval to Delegated Approver</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I need to review an issue approval I've been delegated.</p> <p>When someone delegates an issue approval to another user, that user is&nbsp;notified.&nbsp;</p> <p>A notification is sent only when the project is in the Current status.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project Pending Approval to Approvers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I need to approve a project.</p> <p>Which users receive an email notification for this event depends&nbsp;on whether the&nbsp;'Approver not&nbsp;required to be on the project team (for approval processes&nbsp;that include a job role)' setting is enabled (as described in&nbsp;<a href="establish-approval-settings.md" class="MCXref xref">Establish approval settings</a>).&nbsp;</p> <p><b>If this option is enabled</b>, an email notification is sent to all users in the system with the 'Approver' Job Role.</p> <p><b>If this option is disabled</b>, only project team members with the 'Approver' Job Role receive an email notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project &nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project Pending Approval to Delegated Approver&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I need to review a project approval I've been delegated.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;Active</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task Assignment to Task Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I'm set as the primary assignee of a task.</p> <p>The Task Assignee receives an email notification if he or she is made the primary assignee of the task, unless the assignee is the user who made the assignment.</p> <p>A notification is sent if the project status is Current and the task is not marked Complete.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Pending Approval to Approvers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I need to approve a task.</p> <p>Which users receive an email notification for this event depends&nbsp;on whether the&nbsp;'Approver not&nbsp;required to be on the project team (for approval processes&nbsp;that include a role)' setting is enabled (as described in&nbsp;<a href="establish-approval-settings.md" class="MCXref xref">Establish approval settings</a>).&nbsp;</p> <p><b>If this option is enabled</b>, an email notification is sent to all users in the system with the 'Approver' Job Role.</p> <p><b>If this option is disabled</b>, only project team members with the 'Approver' Job Role receive an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current at the time of the request.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task Pending Approval to Delegated Approver</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I need to review a task approval I've been delegated.</p> <p>When someone delegates an issue approval to another user, that user is&nbsp;notified.&nbsp;</p> <p>A notification is sent only if the project status is&nbsp;Current at the time of the request.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Timesheet</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Timesheet Re-opened to User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>My timesheet is re-opened.</p> <p>The Timesheet Owner receives an email notification when the timesheet is re-opened, unless the user who re-opened the timesheet is also the owner of the timesheet.</p> <p>An email notification is sent only if the timesheet status is Open.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Timesheet</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Timesheet Rejection to User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>My timesheet is rejected.</p> <p>The Timesheet Owner receives an email notification when the timesheet is rejected, unless the user who rejected the timesheet is also the owner.</p> <p>An email notification is sent only if the timesheet status is Rejected.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Timesheet</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Timesheet Submission to Approver</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I need to approve a timesheet.</p> <p>The Timesheet Approver receives an email notification when a timesheet that they need to approve is submitted, unless the user who submitted the timesheet is also the Timesheet Approver.</p> <p>A notification is sent only if the status of the timesheet is Submitted.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Assignment</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Work Item Request to Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>My team gets a new work request.</p> <p>Team Members receive an email notification when the team receives a new work request.&nbsp;(The user who submitted the request does not receive a notification if he or she is a member of the team.)</p> <p>A notification is sent only if the project status is&nbsp;Current at the time the Work Request is made and the Work Request status is New.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Assignment</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Work Item Request to Work Item Assignee</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>I get a new work request.</p> <p>The assignee of the work item receives an email notification, unless the user making the request is also the assignee.&nbsp;</p> <p>A notification is not sent if the&nbsp;task status is Complete or the issue status is Closed.</p> <p>A notification is sent only if the project status is&nbsp;Current at the time of the request.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
 </tbody> 
</table>



## Requests I have made {#requests-i-have-made}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 170px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 190px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document Approval Status Change to Requestor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A document approval request is completed.</p> <p>The Document Requestor receives an email notification when the document approval request is completed.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document Request Complete to Requestor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A document upload request is fulfilled.</p> <p>The Document Requestor receives an email notification when &nbsp;a request to upload a document is fulfilled.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Add to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I add an issue to a project.</p> <p>The primary contact on an issue receives a notification when he or she adds an issue in a project.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issue Assignment to Issue Primary Contact</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Someone is assigned to an issue for which I'm the primary contact</p> <p>The primary contact on an issue receives a notification when the issue is assigned to a user.&nbsp;</p> <p>A notification is sent only if the project status is Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;Inactive</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Completion to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>An issue for which I'm the primary contact is completed.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project Status Change to Entered By</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The status changes on a project I created.</p> <p>The user who created the project receives an email notification when the project status changes.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Request Add to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I submit a request (confirmation).</p> <p>The Primary Contact on the issue receives an email notification when he or she submits an issue.</p> <p>A notification is sent only if the project status is&nbsp;Current and if the project is using a 'Is&nbsp;Help Desk' View.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Request Assignment to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Someone is assigned to my request.</p> <p>The primary contact of the issue receives an email notification when a user is assigned to the issue, unless the primary contact and the assigned user are the same user.</p> <p>A notification is sent only if the project status is&nbsp;Current and if the project is using a 'Is&nbsp;Help Desk' View.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Request Closed to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>My request is closed (confirmation).</p> <p>The issue's primary contact receives an email notification when the request is closed.</p> <p>A notification is sent only if the project status is&nbsp;Current and if the project is using a 'Is&nbsp;Help Desk' View.</p> <p>If the notifications for "issue completion" are enabled, they will always trigger instead of the "Request closed to Issue Primary Contact." If you want this notification to trigger, you must disable the "issue completion" notifications.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Request Document Add to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A document is changed or uploaded on an issue for which I am the primary contact.</p> <p>The issue's primary contact receives an email notification when a document is uploaded or changed on the issue, unless the user who uploaded or changed the document is also the primary contact.</p> <p>A notification is sent only if the project status is&nbsp;Current and if the project has the 'Publish as Help Request Queue' enabled on the Queue Setup tab. For more information on publishing &nbsp;a project as a Help Request Queue, see Overview of the Queue Details tab in a project.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Request Status Change to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>The status changes on my request.</p> <p>The primary contact of the issue receives an email notification when the issue status changes, unless the user who changed the status is also the primary contact.</p> <p>A notification is sent only if the project status&nbsp;is Current and the project is using a 'Is&nbsp;Help Desk' View.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
 </tbody> 
</table>



## Communication {#communication}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 169px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 190px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 422px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 56px;"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Comment on Document to Document Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A comment is added on my document.</p> <p>The owner of a document in <span class="WFVariablesProdNameWF">Workfront</span> receives an email notification when a comment is posted on the document, unless the user who posted the comment is also the document owner.</p> <p>Any users who are directly included in the comment also receive an email notification.</p> <p>A notification is sent only if the project status is Current.&nbsp;</p> <p>The subject of the instant notification email is: <em>Comment on &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></p> <p> The subject of the daily digest notification is:<em> Digest of Communication &lt;Date of daily digest&gt;</em></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Note</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Request Note Add to Issue Primary Contact</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>When a comment is posted on&nbsp;a request, email the issue primary contact.</p> <p>The primary contact for an issue receives&nbsp;an email notification when a comment is posted on a request, unless the user who posted the comment is also the primary contact for the issue.</p> <p>Any users who are directly included on the comment also receive an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Directed Update to User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Someone includes me on a directed update.</p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="tag-others-on-updates.md" class="MCXref xref">Tag others on updates </a>.</p> <p>In this case, the user who is included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only if the user has access rights to the object.&nbsp;</p> <p>This event notification is enabled by default and cannot be disabled.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Directed Update to Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Someone includes my team on a directed update.</p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="tag-others-on-updates.md" class="MCXref xref">Tag others on updates </a>.</p> <p>In this case, any member of the team that is included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only to users who have access rights to the object of the update.</p> <p>If the user sending the directed update is a member of the team being included, the user sending the update does not receive an email notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Note</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Work Item Comment to Thread Participants</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Someone comments on a thread I'm in.</p> <p>Participants in the thread and users who are included in a direct message&nbsp;receive an email notification when a user makes a comment in the thread.</p> <p>Users must have View access&nbsp;to receive a notification.</p> <p>The following users do not receive a notification:</p> 
    <ul> 
     <li value="1"> <p>Teams that are included in a direct message</p> </li> 
     <li value="2"> <p>The owner of the Note</p> </li> 
     <li value="3"> <p>The Primary Contact</p> </li> 
    </ul> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Note</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Work Item Comment to Work Item Assignee</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Someone comments on one of my work items.</p> <p>The assignee of the work item receives an email notification any time a user adds an update to a work item, unless the user who adds the update is also the assignee.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Note</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Work Request Reply To Work Requester</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Someone replies to my request.</p> <p>After a user submits a request and another user replies to that request, the user who submitted the request receives an email notification.</p> <p>An email notification is not sent if:</p> 
    <ul> 
     <li value="1"> <p>The user who replies is the same user who made the request</p> </li> 
     <li value="2"> <p>The user does not have access to see the note</p> </li> 
    </ul> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
 </tbody> 
</table>



## Approval information {#approval-information}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 168px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 190px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 424px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Approval Delegation to Another User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>I'm delegated as an approver.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Delegated Issue Approval Status Change</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A delegated issue approval request is completed.&nbsp;</p> <p>When you delegate an issue approval to someone else, you receive an email notification when they finish that approval (whether they approve or reject the issue approval).&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Delegated Project Approval Status Change</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A delegated project approval request is completed.</p> <p>When you delegate a project approval to someone else, you receive an email notification when they finish that approval (whether they approve or reject the project&nbsp;approval).</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Delegated Task Approval Status Change</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A delegated task approval status is completed.</p> <p>When you delegate a task approval to someone else, you receive an email notification when they finish that approval (whether they approve or reject the task&nbsp;approval).</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document Approval Cancel to Approver</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A document approval request is canceled.</p> <p>The Document Approver of the document receives an email notification when the document approval request is canceled.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Timesheet</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Timesheet Approval to User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>My timesheet is approved.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>



## Information about work assigned to me {#information-about-work-assigned-to-me}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 168px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 190px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 415px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>All Predecessor Task Completion to Task Dependents</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>All predecessors of my tasks are completed.</p> <p>The task assignee receives an email notification.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Approval decision to issue assigned to</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue I resolve is approved or rejected.</p> <p>The assignee of an issue receives an email notification when an approval decision is made (approved or rejected).</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Approval decision to Task Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A task I complete is approved or rejected.</p> <p>The task assignee receives an email notification when the task is approved or rejected.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Completion to Issue Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue I'm assigned to is completed.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Planned Completion Date changed</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>The due date changes on an issue I'm assigned to.</p> <p>The issue assignee receives an email notification when the Planned Completion Date changes, unless the user who changed the Planned Completion Date is also the assignee.</p> <p>A notification is sent only if the project status is&nbsp;anything other than Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Status Change to Issue Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The status changes on one of my work items.</p> <p>The assignee of the issue receives an email notification when the status changes, unless the user who changed the status is also the assignee.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Request Document Add to Issue Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Documents are uploaded or changed on requests I'm assigned to.</p> <p>The issue assignee receives an email notification when documents are uploaded or changed on an issue he or she has added.</p> <p>An email notification is not sent if the user who entered&nbsp;the issue is the issue assignee.</p> <p>A notification is sent only if the project status is&nbsp;Current and if the project has the 'Publish as Help Request Queue' enabled on the Queue Setup tab. For more information on publishing &nbsp;a project as a Help Request Queue, see Overview of the Queue Details tab in a project.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Completion to Task Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A task I'm assigned to is completed.</p> <p>The Task Assignee receives an email notification when the task is completed. Notifications are not sent when a personal task is completed.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task Completion to Task Dependents</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A predecessor of one of my tasks is completed.</p> <p>The task assignee receives an email notification when one of their task's predecessors has been completed.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Planned Completion Date Changed</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The due date changes on a task I'm assigned to.</p> <p>The Task Assignee receives an email notification when the Planned Completion Date of&nbsp;the task changes, unless the user who changed the Planned Completion Date&nbsp;is also the Task Assignee.</p> <p>A notification is sent only if the project status is&nbsp;anything other than Planning.</p> <p>No notification is sent regarding personal tasks.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Task Status Change to Task Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>The status changes on a task I'm assigned to.</p> <p>The Task Assignee receives an email notification when the status of the task changes, unless the user who changed the status is also the assignee.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> <p>Users with a Review license do not receive a notification.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>



## Information about projects I'm on {#information-about-projects-im-on}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 167px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 190px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 419px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Current Project Status Change to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A project I'm on becomes active.</p> <p>Users on the project receive an email notification when the project becomes active.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document Add to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A document is added to a project I'm on.</p> <p>Users on the project team receive an email notification when a document is added to the project, except for the user who added the document.</p> <p>A notification is sent only if the project status is&nbsp;Current and the document is not Private.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Add to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>An issue is added to a project I'm on.</p> <p>Users in a project receive an email notification when an issue is added to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Completion to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue is completed on a project I'm on.</p> <p>Any user on the project receives a notification.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Milestone Task Completion to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A milestone task is completed on a project I'm on.</p> <p>All users on the Project Team&nbsp;receive a notification when a milestone task is completed.&nbsp;</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project Completion to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A project I'm on is completed.</p> <p>Users on a project team receive an email notification when the project status is Complete.</p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span>If projects are completed regularly, enabling this option can create a lot of email for&nbsp;users who have a limited number of tasks on many projects.&nbsp;
    </div> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project Status Change to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>The status changes on a project I'm on.</p> <p>Users on the Project Team receive an email notification when the status of the project changes.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project User Add to Project User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I'm added to a project.</p> <p>The user who was added to the project receives an email notification when he or she is added, unless the user added himself or herself to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task Completion to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A task is completed on a project I'm on.</p> <p>Members of the project team&nbsp;receive&nbsp;an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Unassigned Issue Added to Project Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>An unassigned issue is added to a project I'm on.</p> <p>Users on a project receive an email notification when an unassigned issue is added to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>



## Information about projects I own {#information-about-projects-i-own}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 168px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 189px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 420px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document Add to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A document is added to a project I own.</p> <p>The Project Owner receives an email notification when a document is added to the project, unless the user who added the document is also the Project Owner.</p> <p>A notification is sent only if the project status is&nbsp;Current and the document is not Private.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Add to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue is added to a project I own.</p> <p>The Project Owner receives an email notification when an issue is added to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Commit Date Change to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>The commit date changes for an issue on one of my projects.</p> <p>The Project Owner receives an email notification when the Commit Date changes for an issue on the project, unless the user who changes the Commit Date is the same user as the Project Owner.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Completion to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue is completed on a project I own.</p> <p>The project owner receives an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Milestone Task Completion to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A milestone task is completed on a project I own.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project Owner Assignment to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I'm set as the owner of a new project.</p> <p>When a user is assigned as the owner of a project, that user receives an email notification.</p> <p>If the project owner is the same user who made the assignment, an email notification is not sent</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project Progress Change to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A project I own gets behind.</p> <p>The project owner receives an email notification when&nbsp;the project is behind schedule.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Commit Date Change to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The commit date changes for a task on one of my projects.</p> <p>The Project Owner receives an email notification when the Commit Date changes for a task on the project, unless the user who changed the Commit Date is also the Project Owner.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task Completion to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A task is completed on a project I own.</p> <p>The project owner receives a notification.&nbsp;</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Progress Change to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A task on a project I own gets behind.</p> <p>The Project Owner receives an email notification when a task on the project gets behind schedule.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Unassigned Issue Add to Project Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>An unassigned issue is added to a project I own.</p> <p>The Project Owner receives an email notification when an unassigned issue is added to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>



## Information about projects I sponsor {#information-about-projects-i-sponsor}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 170px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 187px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 421px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Document Add to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A document is added to a project I sponsor.</p> <p>The Project Sponsor receives an email notification when a document is added to the project, unless the document is added by the Project Sponsor.</p> <p>A notification is sent only if the project status is&nbsp;Current and if the document is not Private.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Add to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue is added to a project I sponsor.</p> <p>The Project Sponsor receives an email notification when an issue is added to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Issue Completion to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>An issue is completed on a project I sponsor.</p> <p>The project sponsor receives an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Milestone Task Completion to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A milestone task is completed on a project I sponsor.</p> <p>The Project Sponsor receives an email notification when a milestone task is completed on a project he or she sponsors.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project Progress Change to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A project I sponsor gets behind.</p> <p>The Project Sponsor receives an email notification when the project gets behind schedule.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project Sponsor Assignment to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>I'm set as the sponsor of a project.</p> <p>The project sponsor receives an email notification when he or she is set as the sponsor of a project.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Task Completion to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A task is completed on a project I sponsor.</p> <p>The project sponsor receives an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Progress Change to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A task on a project I sponsor gets behind.</p> <p>The Project Sponsor receives an email notification when a task on the project gets behind schedule.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Unassigned Issue Add to Project Sponsor</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>An unassigned issue is added to a project I sponsor.</p> <p>The Project Sponsor receives an email notification when an unassigned issue is added to the project.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Inactive</p> </td> 
  </tr> 
 </tbody> 
</table>



## Miscellaneous information {#miscellaneous-information}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" border="1" cellspacing="0" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 171px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 187px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 420px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Object Type</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Event</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><b>Description</b> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Announcement was added</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A message is sent to the Announcement Center.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Document Request Cancel to Requestee</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Cancel a document upload request from me.</p> <p>The Document Requestee receives an email notification when a document request is canceled.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Error Notification</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>An error was found that needs your attention.</p> <p>An email notification is generated after <span class="WFVariablesProdNameWF">Workfront</span> tries and fails to connect to a POP account.&nbsp;After 25&nbsp;tries, <span class="WFVariablesProdNameWF">Workfront</span> disables the connection to the POP account&nbsp;in order to preserve resources and it sends out a notification.&nbsp;</p> <p>The email notification is sent&nbsp;to the&nbsp;Project Owner, if the POP email is associated with a request queue, or to the <span class="WFVariablesAdminWF">Workfront administrator</span>s,&nbsp;if the POP account is associated with the "Incoming Mail" feature in Email Setup.<br>For more information on how to associate a request queue with a POP account, see Overview of the Queue Details tab in a project.<br>For more information on how to enable a POP account for incoming mail, see <a href="allow-users-reply-to-email-notifications.md" class="MCXref xref">Allow users to reply to email notifications</a>.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Issue Assignment to Resource Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>An issue assignment change affects one of my people.</p> <p>The Issue Assignee Manager receives an email notification when a change affects a user they manage.</p> <p>A notification is sent only if the project status is&nbsp;Current or Planning.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>New User to User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>When a new user is created in <span class="WFVariablesProdNameWF">Workfront</span>, email the user.</p> <p>After the new user is created, the user receives an email invitation, notifying them that a <span class="WFVariablesProdNameWF">Workfront</span> account has been created and prompting them to set their password.</p> <p><span style="font-weight: 400;">When creating a new user, users can select the option "Send an invite email to this person" (as described in </span><a href="add-users.md" class="MCXref xref">Add users</a><span style="font-weight: 400;">). However, when the "New User to User" option is enabled globally, all new users receive the email invitation regardless of whether the 'Send an invite email to this person' option is selected.</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> Inactive&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Object Share to Team</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Someone shares an object with my team.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Object Share to User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Someone shares an object with me.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Project User Add to Resource Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>One of my people is added to a project.</p> <p>A manager receives an email notification when one of his or her direct reports&nbsp;is added to a project.</p> <p>Users with a Review license do not receive a notification.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project added to a portfolio or program</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Someone adds a project to a portfolio or program I own.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Active</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Task Assignment to Resource Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>A task assignment&nbsp;change affects one of my people.</p> <p>The Task Assignee's Manager receives an email notification.</p> <p>A notification is sent only if the project status is&nbsp;Current.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Inactive</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> Project <br>Task <br>Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">New Update to Subscriber&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p class="p1"><span class="s1 wysiwyg-font-size-medium">An email is sent when an update is made to a task, issue, or project that I am subscribed to.</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Active</td> 
  </tr> 
 </tbody> 
</table>

