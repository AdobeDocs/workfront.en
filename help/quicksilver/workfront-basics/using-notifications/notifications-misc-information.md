---
content-type: reference
navigation-topic: notifications
title: 'Notifications: Miscellaneous information'
description: The following notifications alert you about activities happening on a project you are sponsoring.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
---
# Notifications: Miscellaneous information

The following notifications alert you about activities happening on a project you are sponsoring.

For information about configuring which notifications you receive, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

See also [Event notifications](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>You cannot enable or disable daily notifications and you do not receive daily digest emails for the events in this category. You can enable or disable individual instant notifications for the [!UICONTROL Miscellaneous] category.

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
   <td> <p><strong>A message is sent to the [!UICONTROL Announcement Center]</strong> </p> <p>You receive an email notification when a new message has been sent to the [!UICONTROL Announcement Center]. </p> <p>The subject of the instant notification email is: <em>[!UICONTROL [!DNL Adobe Workfront] Announcement]: &lt;Subject of the Announcement></em></p> </td> 
   <td> Subject of the Announcement<br>Text of the message included in the Announcement<br>Attached Document(s)<br>Name of the user who sent the Announcement<br>Date and Time when the Announcement was sent </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A task assignment change affects one of my people</strong> </p> <p>When one of the Direct Reports of a user designated as a manager is assigned to a new task, the manager receives an email about the assignment. </p> <p>A notification is sent only if the project status is [!UICONTROL Current].</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Task Resource Assignment]: &lt;Task Name></em></p> </td> 
   <td>Project Name<br>Task Name<br>Date and Time when the task was created<br>Name of the user who created the task<br>Assignment Names<br>Due Date (Planned Completion Date)<br>Task Status<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>After receiving a document upload request, the request is canceled</strong> </p> <p>The Document Requestee receives an email notification when a document request is canceled.</p> <p>The subject of the instant notification email is: <em>&lt;Name of the user who canceled the request> canceled the document request. </em></p> <p>The following text is included in the body of the email notification:</p> <p><em>[!UICONTROL Hi] &lt;Your Name>, <br><br>&lt;Name of the user who canceled the request>[!UICONTROL no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.]</em> </p> </td> 
   <td>Name of the user who canceled the request<br>The text of the original document upload request<br>A "[!UICONTROL CANCELED]" banner over the original document request<br>Date and Time of the original document request<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An error was found that needs my attention</strong> </p> <p>The user replying to a comment via email receives an email notification when the reply fails to be delivered.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Failed to Process on] &lt;subject of original message></em></p> <p>For information about using email to reply to comments, see .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An issue assignment change affects one of my people</strong> </p> <p>The manager of a user assigned to an issue receives an email notification when that user is removed from or assigned to an issue. </p> <p>A notification is sent only if the project status is Current or Planning.</p> <p>The subject of the instant notification email is: <em>Issue Assignment: &lt;Issue Name></em></p> </td> 
   <td> <p>Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who made the assignment<br>Issue Type<br>Name of the user assigned to the issue<br>Issue Date Entered<br>Issue Priority<br>Primary Contact<br>Issue [!UICONTROL Planned Completion Date]<br>Issue Status<br><strong>[!UICONTROL See More Details]</strong> button</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>One of my people is added to a project</strong> </p> <p>A manager receives an email notification when one of his or her users is added to a project. This notification is sent regardless of the status of the project. </p> <p>Users with a [!UICONTROL Review] license do not receive a notification.</p> <p>The subject of the email is: <em>Project Assignment: &lt;User Name>[&lt;Project GUID>_ &lt;User GUID>]</em></p> </td> 
   <td> <p>Project Name<br>Portfolio Name<br>Project Reference Number<br>Name of the user who added the person to the project<br>Name of the user who was added to the project<br>Project [!UICONTROL Planned Start Date]<br>Project [!UICONTROL Planned Completion Date]<br>Project Percent Complete<br>Names of Others on Project<br>Project Status<br>Project Owner<br><strong>[!UICONTROL See More Details]</strong> button<br><br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone adds a project to a portfolio or program I own</strong> </p> <p>The portfolio and/ or the program owner receive a notification when a new project is added to a portfolio or a program.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Project added to] &lt;Portfolio Name>[Project GUID]</em></p> </td> 
   <td> Portfolio Name<br>Project Reference Number<br>Name of the user who added the project to the portfolio/ program<br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone shares an object with me</strong> </p> <p>You receive an email notification when someone adds you to the [!UICONTROL Sharing] list of permissions on an object.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Access Granted]: &lt;Object Name></em></p> <p>A notification Is sent only if the project is in [!UICONTROL Current] status.</p> </td> 
   <td> Object Name<br>Parent Object Name<br>Object Reference Number<br>Original Access to the object<br>New Access granted to the object<br>Date and Time when the access was granted <br>Name of the user who granted the access </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone shares an object with my team</strong> </p> <p>You receive an email notification when someone adds your team to the Sharing list of permissions on an object.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Access Granted]: &lt;Object Name> [Access Rule GUID]</em></p> </td> 
   <td> Object Name<br>Parent Object Name<br>Object Reference Number<br>Old Access<br>New Access<br>Date and Time when the access was granted<br>Name of your team<br>Name of the user who granted the access </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An update is made to a task, issue, or project I am subscribed to</strong> </p> <p>You receive an email notification when someone comments on an item to which you are subscribed.</p> <p>The subject of the subscription email is: <em>[!UICONTROL An update was made to the] &lt;Object Type> you are subscribed to: &lt;Object Name></em></p> </td> 
   <td> Object Name<br> Object Reference Number<br> Name of the user who made a comment on the subscribed item<br> Date comment was made<br> Comment added to the subscribed item  </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
