---
content-type: reference
navigation-topic: notifications
title: 'Notifications: Information about work assigned to me'
description: The following notifications alert you about activities happening on a work item assigned to you.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
---
# Notifications: Information about work assigned to me

The following notifications alert you about activities happening on a work item assigned to you.

For information about configuring which notifications you receive, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

See also [Event notifications](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
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
   <td> <p><strong>A predecessor of a task assigned to my team is completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Predecessor Task Name<br>Predecessor Task Project<br>Predecessor Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of predecessors completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </p> </td> 
   <td><strong>Daily</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Predecessor Task Name<br>Predecessor Task Project<br>Predecessor Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of predecessors completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </p> </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>A task I complete is approved or rejected</strong> </p> <p>The task assignee receives an email notification when the task is approved or rejected.</p> <p>A notification is sent only if the project status is Current.</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name> on &lt;Project Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> Task Name<br>Project Name<br>Task Reference Number<br>Name of the user who granted the approval<br>New Task Status<br>Date and Time when the task was approved or rejected<br>Previous Task Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks approved or rejected<br>*Task Name<br>*Name of the user who approved or rejected the task<br>*Approval Decision ([!UICONTROL Approved]/ [!UICONTROL Rejected])<br>*Date of the daily digest<br></td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>A task I'm assigned to is completed</strong> </p> <p>The Task Assignee receives an email notification when the task is completed.</p> <p>A notification is sent only if the project status is [!UICONTROL Current].</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name> on &lt;Project name></em></p> <p> <p>Note:  If the task is changed to a status that equates with [!UICONTROL Complete], the subject of the email still displays "Complete".</p> </p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Task Name<br>Project name<br>Task Reference Number<br>Name of the user who completed the task<br>Date and Time when the task was completed<br>Previous Task Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of the daily digest<br></p> </td> 
   <td><strong>Daily</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td>
   <td><strong>Instant</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em><br></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>An issue I resolve is approved or rejected</strong> </p> <p>The assignee of an issue receives an email notification when an approval decision is made (approved or rejected).</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Issue Pending Approval: &lt;Planned Start Date&gt; &lt;Issue Reference Number&gt; - &lt;Issue Name&gt; in &lt;Project Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who approved or rejected the issue<br>Approval Decision (Approved or Rejected)<br>Issue Status<br>Name of the user who requested the approval<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of issues approved or rejected<br>*Issue Name<br>*Name of the user who approved or rejected the issue<br>*Approval Decision (Approved or Rejected)<br>*Date of the daily digest<br></td> 
   <td><strong>Daily</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>An issue I'm assigned to is completed</strong> </p> <p>A notification is sent only if the project status is [!UICONTROL Current] or [!UICONTROL Planning].</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Issue Name&gt; on &lt;Project Name&gt;</em></p> <p><em> The subject of the daily digest notification is: Digest of Work Assigned to You &lt;Date of daily digest&gt; </em> </p> </td> 
   <td> Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who completed the issue<br>New Issue Status<br>Date and Time when the issue completed<br>Previous Task Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of issues completed<br>*Issue Name<br>*Name of the user who completed the issue<br>*Date of the daily digest<br></td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documents are uploaded or changed on requests I'm assigned to</strong> </p> <p>The issue assignee receives an email notification when documents are uploaded or document details are changed on an issue he or she has added.</p> <p>An email notification is not sent if the user who triggered the issue is the issue assignee.</p> <p>A notification is sent only if the project status is [!UICONTROL Current] and if the project is set up as a Help Request Queue (as described in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>).</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Document added to] &lt;Request Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Request Name<br>Project Name (Request Queue Name)<br>Document Reference Number <br>Name of the user who uploaded the document<br>Document Name <br>Added On Date<br>Document Details (format, size, Version number)<br>Document thumbnail<br><strong>[!UICONTROL Preview]</strong> and <strong>[!UICONTROL Download]</strong> buttons<br>*Project Name<br>*Project Reference Number<br>*Total number of documents uploaded or changed<br>*Document Name<br>*Object Name<br>*Name of the user who uploaded the document<br>*Date of daily digest</p> </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>The due date changes on a task I'm assigned to</strong> </p> <p>The Task Assignee receives an email notification when the [!UICONTROL Planned Completion Date] of the task changes, unless the user who changed the Planned Completion Date is also the Task Assignee.</p> <p>A notification is sent only if the project status is anything other than [!UICONTROL Planning].</p> <p>No notification is sent regarding personal tasks.</p> <p> Users with a Review or Requestor license do not receive a notification. </p> <p> The subject of the instant notification email is: <em>[!UICONTROL Due Date has been changed.]</em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> Task Name<br>Project Name<br>Task Reference Number<br>New Due Date ([!UICONTROL Planned Completion Date])<br>Date and Time when the Due Date was changed<br>The name of the user who changed the Due Date<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks where the Due Date (Planned Completion Date) changed<br>*Task Name<br>*New Planned Completion Date<br>*Name of the user who changed the Due Date<br>*Date of daily digest </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>The due date changes on an issue I'm assigned to</strong> </p> <p>The issue assignee receives an email notification when the [!UICONTROL Planned Completion Date] changes, unless the user who changed the [!UICONTROL Planned Completion Date] is also the assignee.</p> <p>A notification is sent only if the project status is anything other than [!UICONTROL Planning].</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest></em></p> </td> 
   <td> <p>Issue Name<br>Project Name<br>Issue Reference Number<br>New Due Date ([!UICONTROL Planned Completion Date])<br>Date and Time when the due date was changed<br>Name of the user who changed the due date<br>*Project Name<br>*Project Reference Number<br>*Total number of issues where the Due Date ([!UICONTROL Planned Completion Date]) changed<br>*Issue Name<br>*New [!UICONTROL Planned Completion Date]<br>*Name of the user who changed the Due Date<br>*Date of the daily digest<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>The status changes on a task I'm assigned to</strong> <p>The Task Assignee receives an email notification when the status of the task changes, unless the user who changed the status is also the assignee.</p> <p>Note: This notification is not sent when the task status changes to complete. A separate notification is used for completed tasks. See <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">A task I'm assigned to is completed</a>, above.</p> <p>A notification is sent only if the project status is [!UICONTROL Current].</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>&lt;Task Name> from &lt;Project Name> is &lt;New Status></em></p> <p> </p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> Task Name<br>Project Name<br>Task Reference Number<br>Name of the user who changed the status<br>New Status<br>Date and Time when the status was changed<br>Preview Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks where the Status changed<br>*Task Name<br>*Previous Task Status<br>*New Task Status<br>*Name of the user who changed the Status<br>*Date of the daily digest<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>The status changes on one of my work items</strong> </p> <p>You receive an email notification when the status changes on an issue you're assigned to, unless you change the status yourself. </p> <p>A notification is sent only if the project status is [!UICONTROL Current].</p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>&lt;Issue Name> from &lt;Project Name> is &lt;New Status></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who changed the status<br>New Status<br>Date and Time when the status was changed<br>Previous Issue Status<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of issues where the Status changed<br>*Task Name<br>*Previous Issue Status<br>*New Issue Status<br>*Name of the user who changed the Status<br>*Date of daily digest </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
 </tbody> 
</table>
