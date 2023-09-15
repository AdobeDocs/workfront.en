---
content-type: reference
navigation-topic: notifications
title: 'Notifications: Requests I have made'
description: The following notifications let you know about requests you have made in Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
---
# Notifications: Requests I have made

The following notifications let you know about requests you have made in [!DNL Adobe Workfront].

For information about configuring which notifications you receive, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

See also [Event notifications](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Requests I Have Made</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A document approval request is completed</strong> </p> <p>The user who requested an approval on a document receives an email notification when the document approval request is completed.</p> <p>The subject of the instant notification email is:<em> &lt;Approver Name> has &lt;Approval Decision ([!UICONTROL Approved], [!UICONTROL Approved with Changes], [!UICONTROL Rejected])> this document.</em></p> <p>Note:  You cannot configure this notification for a daily digest email.</p> </td> 
   <td> Document Name<br>Approver Name </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A document is changed or uploaded on an issue for which I am the primary contact</strong> </p> <p>The issue's primary contact receives an email notification when a document is uploaded or changed on the issue, unless the user who uploaded or changed the document is also the primary contact.</p> <p>A notification is sent only if the project is set up as a [!UICONTROL Help Request Queue] (as described in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>The subject of the instant notification email is: <em>Document added to &lt;Issue Name></em></p> <p>The subject of the daily digest notification is: <em>Digest of Your Requests &lt;Date of the daily digest></em></p> </td> 
   <td> Object Name where the document was uploaded<br>Parent Object Name<br>Document Reference Number<br>Name of the user who uploaded the document<br>Document Name<br>Added On Date<br>Document Details (format, size, Version Number)<br>Document thumbnail<br><strong>[!UICONTROL Preview]</strong> and <strong>[!UICONTROL Download]</strong> buttons<br>*Project Name<br>*Project Reference Number<br>*Total number of documents uploaded<br>*Name of document<br>*Parent Object Name<br>*Name of the user who added the document<br>*Date of the daily digest </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A document upload request is fulfilled</strong> </p> <p>The Document Requestor receives an email notification when a document upload request is fulfilled.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Your document request from] &lt;User Name> was fulfilled</em></p> <p>Note:  You cannot configure this notification for a daily digest email.</p> </td> 
   <td> <p>Name of the user who uploaded the document<br>Object Name where the document was uploaded<br>Document Name<br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A personal task I've assigned to someone else is completed</strong> </p> <p>A notification is sent out to the user who assigned an ad-hoc task to someone else when that task is completed. </p> <p>For more information about ad hoc tasks, see <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Create work items from the [!UICONTROL Home] area</a>.</p> <p>The subject of the instant notification email is: <em>Task Completion: &lt;Task Name></em></p> <p> <p>Note:  You cannot configure this notification for a daily digest email.</p> </p> </td> 
   <td> Task Name<br>Default Project Name (Personal Project of the user who received the personal task)<br>Task Reference Number<br>Task Owner Name<br>New Task Status<br>Date and Time when the task was completed<br>Previous Task Status<br><strong>[!UICONTROL See More Details]</strong> button<br><br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An issue for which I'm the primary contact is completed</strong> </p> <p>The primary contact on an issue receives a notification when the issue is completed.</p> <p>A notification is sent only if the project status is [!UICONTROL Current] or [!UICONTROL Planning].</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Issue Completion]: &lt;Issue Name></em></p> <p>The subject of the daily digest notification is:<em> Digest of your Requests &lt;Date of the daily digest></em></p> <p> </p> </td> 
   <td> Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who completed the issue<br>New Status<br>Date and Time when the issue was completed<br>Previous Issue Status<br><strong>[!UICONTROL See More Details]</strong> button <br>*Project Name<br>*Project Reference Number<br>*Total number of completed issues<br>*Issue Name<br>*Name of the user who completed the issue<br>*Date of daily digest </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>I add an issue to a project</strong> </p> <p>The primary contact on an issue receives a notification when he or she adds an issue in a project.</p> <p>A notification is sent only if the project status is [!UICONTROL Current] or [!UICONTROL Planning].</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Issue submitted]: &lt;Issue Name> on &lt;Project Name></em></p> <p>The subject of the daily digest notification is:<em> Digest of your Requests &lt;Date of the daily digest></em></p> </td> 
   <td> Project Name<br>Portfolio Name<br>Issue Reference Number<br>Your Name<br>Issue Name<br>Date Entered<br>Issue Priority<br>Issue Status<br>Assigned To Name<br>Primary Contact<br>*Project Name<br>*Project Reference Number<br>*Total number of issues added<br>*Issue Name<br>*Date of daily digest </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>I submit a request (confirmation)</strong> </p> <p>The Primary Contact on the issue receives an email notification when he or she submits an issue.</p> <p>A notification is sent only if the project status is [!UICONTROL Current] and if the project is set up as a [!UICONTROL Help Request Queue] (as described in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Request Submitted]: &lt;Request Name> on &lt;Project (Request Queue) Name></em></p> <p>The subject of the daily digest notification is:<em> Digest of your Requests &lt;Date of the daily digest></em></p> </td> 
   <td> <p>Project Name (Request Queue Name)<br>Portfolio Name<br>Issue Reference Number<br>Issue Name<br>Date Entered<br>Issue Priority<br>Issue Status<br>Assigned To Name<br>Primary Contact<br>*Project Reference Number<br>*Project Name<br>*Total number of requests submitted<br>*Request Name<br>*Request Priority<br>*Date of daily digest</p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>My request is closed (confirmation)</strong> </p> <p>The issue's primary contact receives an email notification when the request is closed.</p> <p>A notification is sent only if the project status is Current and if the project is set up as a [!UICONTROL Help Request Queue] (as described in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>).</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Your request has been closed]:"&lt;Request Name>"</em></p> <p>The subject of the daily digest notification is:<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest></em></p> </td> 
   <td> Request Name<br>Project Name<br>Request Reference Number<br>Name of the user who closed the Request<br>Issue Status<br>Date and Time when the Request was closed<br>Previous Request Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Reference Number<br>*Project Name<br>*Total number of requests closed<br>*Request Name<br>*Name of the user who closed the request<br>*Date of daily digest </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone is assigned to my request</strong> </p> <p>The primary contact for the issue receives an email notification when a user is assigned to the issue, unless the primary contact and the assigned user are the same user.</p> <p>A notification is sent only if the project status is Current and if the project is set up as a [!UICONTROL Help Request Queue] (as described in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>The subject of the instant notification email is: <em>&lt;Name of the user who is assigned to your request> [!UICONTROL has been assigned to your request]: "&lt;Request Name>"</em></p> <p>The subject of the daily digest notification is:<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest></em></p> </td> 
   <td> <p>Issue Name<br>Project Name<br>Issue Reference Number<br>Request Name<br>Request Type<br>Date Entered<br>Issue Priority<br>Primary Contact<br>Planned Completion Date<br>Issue Status<br><strong>See More Details</strong> button <br>*Project Name<br>*Project Reference Number<br>*Total number of requests assigned<br>*Request Name<br>*Assigned To Name<br>*Date of daily digest</p> </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>The status changes on a project I created</strong> </p> <p>The user who created the project receives an email notification when the project status changes.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Project Status Change]: &lt;Project Name></em></p> <p>The subject of the daily digest notification is:<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest></em></p> </td> 
   <td> <p>Project Name<br>Portfolio Name<br>Project Reference Number<br>Name of the user who changed the status<br>New Status<br>Date and Time when the Project Status was changed<br>Previous Project Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Project New Status<br>*Name of the user who changed the project status<br>*Date of daily digest</p> </td> 
   <td> <p><strong>Instant</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>The status changes on my request</strong> </p> <p>The primary contact of the issue receives an email notification when the issue status changes, unless the user who changed the status is also the primary contact.</p> <p>A notification is sent only if the project status is Current and the project is set up as a [!UICONTROL Help Request Queue] (as described in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>The subject of the instant notification email is: <em>&lt;Request Name> is &lt;New Status></em></p> <p>The subject of the daily digest notification is:<em> Digest of your Requests &lt;Date of the daily digest></em></p> </td> 
   <td> Request Name<br>Project Name<br>Request Reference Number<br>Name of the user who changed the Status of the Request<br>New Status<br>Date and Time when the Status of the Request was changed<br>Previous Request Status<br><strong>[!UICONTROL See More Details]</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of requests whose status changed<br>*Request Name<br>*Previous Request Status<br>*New Request Status<br>*Name of the user who changed the status<br>*Date of the daily digest<br></td> 
   <td> <p><strong>Daily</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
