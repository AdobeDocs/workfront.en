---
filename: notifications-action-needed
content-type: reference
navigation-topic: notifications
title: Notifications: Action needed
description: The following notifications let you know if you need to take action on a work item. For information about configuring which notifications you receive, see Activate or deactivate your own event notifications.
---

# Notifications: Action needed

The following notifications let you know if you need to take action on a work item. For information about configuring which notifications you receive, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

See also [Event notifications](../../workfront-basics/using-notifications/event-notifications.md).

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>Fields included </p> <p> *Daily digest fields only</p> </th> 
   <th>Default status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">I get a new work request</span> </p> <p>The assignee of the work item receives an email notification, unless the user making the request is also the assignee. </p> <p>A notification is not sent if the task status is Complete or the issue status is Closed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>New Work Request: &lt;Request Name&gt;</em></p> <p>The subject of the daily digest notification is: <em>Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>Task name</p> <p>Planned Completion Date</p> <p>Parents</p> <p>Assigned by</p> <p>Assigned to</p> <p>Status</p> <p>Description</p> <p>View button<br>Option to add to the daily digest</p> <br> </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to approve a document</span> </p> <p>The approver of a document receives a notification when they are listed as the approver.</p> <p>The subject of the instant notification email is: <em>&lt;Name of the user who submitted the approval&gt; asked you to approve a document in Adobe Workfront.</em></p> <p>The subject of the daily digest notification is:<em> Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Project Name<br>Portfolio Name<br>Name of the user who submitted the approval<br>Document Name<br>Document Reference Number<br>Date and Time of Approval Requested<br>Document Details (format, size, version number)<br><span class="bold">Make Approval Decision</span> button<br>*Total number of pending document approvals<br>*Link to <span class="bold">Document Approvals<br></span>*<span class="bold">See All Approvals</span> button<br>*Date of the daily digest<br></td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to approve a project</span> </p> <p>In case of job role approvals, which users receive an email notification for this event depends on whether the 'Approver not required to be on the project team (for approval processes that include a role)' setting is enabled (as described in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>). </p> <p><span class="bold">If this option is enabled</span>, an email notification is sent to all users in the system with the job role associated with the approval. </p> <p><span class="bold">If this option is disabled</span>, only project team members with the job role associated with the approval process receive an email notification.</p> <p>If the approval is associated with a user, that user receives the notification.</p> <p>The subject of the instant notification email is: <em>Project Pending Approval: &lt;Project Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Action Needed &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Project Name<br>Portfolio Name<br>Project Reference Number<br>Name of user who submitted the approval<br>Pending Approval Status<br>Date and Time of Approval Requested<br>Project Priority<br>Approval Step Pending Approval<br>Number of decisions waiting for approval<br>Approvers Name (users only)<br>Project Planned Completion Date <br><span class="bold">Make Approval Decision </span>button<br>*Total number of pending project approvals <br>*Link to <span class="bold">Project Approvals</span><br>*<span class="bold">See All Approvals</span> button<br>*Date of the daily digest</p> </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to approve a task</span> </p> <p>In case of job role approvals, which users receive an email notification for this event depends on whether the 'Approver not required to be on the project team (for approval processes that include a role)' setting is enabled (as described in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>). </p> <p><span class="bold">If this option is enabled</span>, an email notification is sent to all users in the system with the job role associated with the approval. </p> <p><span class="bold">If this option is disabled</span>, only project team members with the job role associated with the approval process receive an email notification.</p> <p>If the approval is associated with a user, that user receives the notification. </p> <p>A notification is sent only if the project status is Current.</p> <p>The subject of the instant notification email is: <em>Task Pending Approval: &lt;Task Name&gt;</em></p> <p> T he subject of the daily digest notification is: <em> Digest of Action Needed &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Task Name<br>Project Name<br>Name of the user who submitted the approval<br>Pending Approval Status<br>Date and Time of Approval Requested<br>Task Priority<br>Approval Stage Name<br>Approvers Names<br>Task Planned Completion Date<br><span class="bold">Make Approval Decision </span>button<br>*Total number of pending task approvals<br>*Link to<span class="bold">Task Approvals<br></span><span class="bold">*See All Approvals </span>button<span class="bold"><br></span>*Date of the daily digest<br></p> </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to approve a timesheet</span> </p> <p>The Timesheet Approver receives an email notification when a timesheet that they need to approve is submitted, unless the user who submitted the timesheet is also the Timesheet Approver.</p> <p>A notification is sent only if the status of the timesheet is Submitted.</p> <p>The subject of the instant notification email is: <em>Timesheet Submitted: &lt;Timesheet Owner&gt;, &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Action Needed &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> Name of the user who submitted the timesheet for approval<br>Date and Time when the timesheet was submitted<br>Status of the timesheet<br>Start and End Dates of the Timesheet<br>Number of hours logged on the timesheet<br>Number of Overtime hours logged on the timesheet<br><span class="bold">Review</span> and <span class="bold">Approve</span> buttons<br>*The total number of pending timesheet approvals<br>*Link to <span class="bold">Timesheet Approvals</span><br><span class="bold">*See All Approvals </span>button<br>*Date of the daily digest </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to approve an issue</span> </p> <p>In case of job role approvals, which users receive an email notification for this event depends on whether the 'Approver not required to be on the project team (for approval processes that include a role)' setting is enabled (as described in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configure global approval settings</a>). </p> <p><span class="bold">If this option is enabled</span>, an email notification is sent to all users in the system with the job role associated with the approval. </p> <p><span class="bold">If this option is disabled</span>, only project team members with the job role associated with the approval process receive an email notification.</p> <p>If the approval is associated with a user, that user receives the notification. </p> <p>A notification is sent only if the project status is Current.</p> <p>The subject of the instant notification email is: <em>Issue Pending Approval: &lt;Issue Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Action Needed &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who submitted the issue for approval<br>Pending Approval Status<br>Date and Time of Approval Requested<br>Issue Priority<br>Approval Stage<br>Names of Approvers<br>Issue Planned Completion Date<br>Primary Contact<br><span class="bold">Make Approval Decision</span> button<br>*The total number of pending issue approvals<br>*Link to <span class="bold">Issue Approvals</span><br><span class="bold">*See All Approvals </span>button<br>*Date of the daily digest </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to review a project approval I've been delegated</span> </p> <p>A project approval was delegated to you and you need to review it.</p> <p>The subject of the instant notification email is: <em>Delegated Project Approval - Please Review &lt;Project Name&gt;</em></p> <p><em>The subject of the daily digest notification is: Digest of Action Needed &lt;Date of the daily digest&gt;</em> </p> </td> 
   <td> Project Name<br>Portfolio Name<br>Project Reference Number<br>Name of the user who asked for approval<br>Name of the user on whose behalf you are approving the Project<br>Pending Approval Status<br>Date and Time of Approval Requested<br>Project Priority<br>Approval Step<br>Names of Approvers<br>Project Planned Completion Date<br><span class="bold">Make Approval Decision</span> button<br>*Total number of pending project approvals<br>*Link to <span class="bold">Project Approvals<br></span><span class="bold">*See All Approvals </span>button <br>*Date of the daily digest </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to review a task approval I've been delegated</span> </p> <p>A task approval was delegated to you and you need to review it.</p> <p>The subject of the instant notification email is: <em>Delegated Task Approval - Please Review &lt;Task Name&gt;</em></p> <p>The subject of the daily digest notification is:<em> Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Task Name<br>Project Name<br>Task Reference Number<br>Name of the user who asked for approval<br>Name of the user on whose behalf you are approving the Task<br>Pending Approval Status<br>Date and Time of Approval Requested<br>Task Priority<br>Approval Stage<br>Names of Approvers<br>Task Planned Completion Date<br><span class="bold">Make Approval Decision</span> button <br>*Total number of pending task approvals<br>*Link to <span class="bold">Task Approvals<br></span><span class="bold">*See All Approvals </span>button<br>*Date of the daily digest </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I need to review an issue approval I've been delegated</span> </p> <p>An issue approval was delegated to you and you need to review it.</p> <p>The subject of the instant notification email is: <em>Delegated Issue Approval - Please Review &lt;Issue Name&gt;</em></p> <p>The subject of the daily digest notification is:<em> Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who asked for approval<br>Name of the user on whose behalf you are approving the Issue<br>Pending Approval Status<br>Date and Time of Approval Requested<br>Issue Priority<br>Approval Stage<br>Names of Approvers<br>Issue Planned Completion Date<br>Primary Contact<br><span class="bold">Make Approval Decision</span> button<br>*Total number of pending issue approvals<br>*Link to <span class="bold">Issue Approvals</span><br><span class="bold">*See All Approvals </span>button<br>*Date of the daily digest<br></td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I'm assigned to an issue</span> </p> <p>The issue assignee receives an email notification. The issue assignee does not receive an email if the status of the issue is or equates with Closed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>A notification is sent only if the project status is Current.</p> <p>The subject of the instant notification email is: <em>New Work Request: &lt;Issue Name&gt;</em></p> <p>The subject of the daily digest notification is:<em> Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>Issue Name<br>Project Name<br>Issue Reference Number<br>Your Name<br>Issue Due Date (Planned Completion Date)<br>Name of the user who assigned the issue to you<br><span class="bold">Work On It</span> button<br>*Total number of assignments<br>*Total number of tasks and issues assigned to you<br>*Link to <span class="bold">Work Requests</span><br>*Date of the daily digest<br></p> </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">I'm set as the primary assignee of a task</span> </p> <p>The Task Assignee receives an email notification if he or she is made the primary assignee of the task, unless the assignee is the user who made the assignment.</p> <p>A notification is sent if the project status is Current and the task is not marked Complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>New Work Request: &lt;Task Name&gt;</em></p> <p>The subject of the daily digest notification is:<em> Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Task Name<br>Project Name<br>Task Reference Number<br>Your Name<br>Task Due Date (Planned Completion Date)<br>Name of the user who assigned the task to you<br><span class="bold">Work On It</span> button<br>*Total number of tasks and issues assigned to you<br>*Link to <span class="bold">Work Requests<br></span>*Date of the daily digest </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">My team gets a new work request</span> </p> <p>Team Members receive an email notification when the team receives a new work request. (The user who submitted the request does not receive a notification if he or she is a member of the team.)</p> <p>A notification is sent only if the project status is Current and the Work Request status is New.</p> <p>Users with a Review license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>New Work Request: &lt;Request Name&gt;</em></p> <p>The subject of the daily digest notification is: <em>Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p> Issue Name<br>Project Name (Request Queue Name)<br>Issue Reference Number<br>Team Name<br>Issue Due Date (Planned Completion Date)<br>Name of the user who submitted the Request<br><span class="bold">Work On It</span> button<br>*Total number of requests assigned to your team</p> <p>*Work request name</p> <p>*Planned Completion Date</p> <p>*Name of user who submitted the request<br>*Link to <span class="bold">Team Requests</span><br>*Date of the daily digest </p> <p><span class="preview">* Team assignments</span> </p> </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">My timesheet is re-opened</span> </p> <p>The Timesheet Owner receives an email notification when the timesheet is re-opened, unless the user who re-opened the timesheet is also the owner of the timesheet.</p> <p>An email notification is sent only if the timesheet status is Open.</p> <p>The subject of the instant notification email is: <em>Timesheet Re-opened: &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt;</em></p> <p>Note:  You cannot configure this notification for a daily digest email.</p> </td> 
   <td> Name of the user who re-opened the Timesheet<br>Date and Time when the Timesheet was re-opened<br>Status of the Timesheet (Re-opened)<br>Number of Total Hours logged on the Timesheet<br>Number of Overtime Hours logged on the Timesheet<br><span class="bold">Review</span> button </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">My timesheet is rejected</span> </p> <p>The Timesheet Owner receives an email notification when the timesheet is rejected, unless the user who rejected the timesheet is also the owner.</p> <p>An email notification is sent only if the timesheet status is Rejected.</p> <p>The subject of the instant notification email is: <em>Timesheet Rejected:&lt;Start Date of the Timesheet&gt; - &lt;End Date of the Timesheet&gt;</em></p> <p>Note:  You cannot configure this notification for a daily digest email.</p> </td> 
   <td> Name of the user who rejected the Timesheet<br>Status of the Timesheet (Rejected)<br>Date and Time of when the Timesheet was rejected<br><span class="bold">Review</span> button </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Someone requests access from me</span> </p> <p>Asking me to do something, so turn it on.</p> <p>The person who creates the project gets access to it.</p> <p>This is what makes the user get the notification when someone requests access.</p> <p>The subject of the instant notification email is: <em>&lt;Name of user who requested the access&gt; needs access to &lt;Object Name&gt;</em></p> <p>The subject of the daily digest notification is:<em> Digest of Action Needed &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>Object Name<br>Parent Object Name<br>Object Reference Number<br>Name of the user who requested the access<br>The type of access the user is requesting<br><span class="bold">Grant &lt;Name of the access requested&gt; Access</span> and <span class="bold">Grant different access</span> buttons<br>*Total number of pending access request approvals<br>*Link to <span class="bold">Access Request</span> Approvals<br>*Date of daily digest</p> </td> 
   <td><span class="bold">Instant and </span><span class="bold">Daily</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Someone requests me to upload a document</span> </p> <p>The Document Requestee receives an email notification when a user receives a request to upload a document.</p> <p>The subject of the instant notification email is: <em>&lt;Name of the user requesting the document&gt; needs a document from you in Workfront.</em></p> <p> <p>Note:  You cannot configure this notification for a daily digest email.</p> </p> </td> 
   <td> Name of the user requesting the document<br>Name of the object where the document should be uploaded<br><span class="bold">Attach it here</span> link </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
 </tbody> 
</table>

