---
filename: notifications-misc-information
content-type: reference
navigation-topic: notifications
title: Notifications: Miscellaneous information
description: The following notifications alert you about activities happening on a project you are sponsoring.
---

# Notifications: Miscellaneous information

The following notifications alert you about activities happening on a project you are sponsoring.

For information about configuring which notifications you receive, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

See also [Event notifications](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>You cannot enable or disable daily notifications and you do not receive daily digest emails for the events in this category. You can enable or disable individual instant notifications for the Miscellaneous category.

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
   <td> <p><span class="bold">A message is sent to the Announcement Center</span> </p> <p>You receive an email notification when a new message has been sent to the Announcement Center. </p> <p>The subject of the instant notification email is: <em><em>Adobe Workfront</em> Announcement: &lt;Subject of the Announcement&gt;</em></p> </td> 
   <td> Subject of the Announcement<br>Text of the message included in the Announcement<br>Attached Document(s)<br>Name of the user who sent the Announcement<br>Date and Time when the Announcement was sent </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">A task assignment change affects one of my people</span> </p> <p>When one of the Direct Reports of a user designated as a manager is assigned to a new task, the manager receives an email about the assignment. </p> <p>A notification is sent only if the project status is Current.</p> <p>The subject of the instant notification email is: <em>Task Resource Assignment: &lt;Task Name&gt;</em></p> </td> 
   <td>Project Name<br>Task Name<br>Date and Time when the task was created<br>Name of the user who created the task<br>Assignment Names<br>Due Date (Planned Completion Date)<br>Task Status<br></td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">After receiving a document upload request, the request is canceled</span> </p> <p>The Document Requestee receives an email notification when a document request is canceled.</p> <p>The subject of the instant notification email is: <em>&lt;Name of the user who canceled the request&gt; canceled the document request. </em></p> <p>The following text is included in the body of the email notification:</p> <p><em>Hi &lt;Your Name&gt;, <br><br>&lt;Name of the user who canceled the request&gt; no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.</em> </p> </td> 
   <td>Name of the user who canceled the request<br>The text of the original document upload request<br>A "CANCELED" banner over the original document request<br>Date and Time of the original document request<br></td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">An error was found that needs my attention</span> </p> <p>The user replying to a comment via email receives an email notification when the reply fails to be delivered.</p> <p>The subject of the instant notification email is: <em>Failed to Process on &lt;subject of original message&gt;</em></p> <p>For information about using email to reply to comments, see&nbsp;.<span class="bold"><br></span></p> </td> 
   <td>&nbsp;</td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">An issue assignment change affects one of my people</span> </p> <p>The manager of a user assigned to an issue receives an email notification when that user is removed from or assigned to an issue. </p> <p>A notification is sent only if the project status is Current or Planning.</p> <p>The subject of the instant notification email is: <em>Issue Assignment: &lt;Issue Name&gt;</em></p> </td> 
   <td> <p>Issue Name<br>Project Name<br>Issue Reference Number<br>Name of the user who made the assignment<br>Issue Type<br>Name of the user assigned to the issue<br>Issue Date Entered<br>Issue Priority<br>Primary Contact<br>Issue Planned Completion Date<br>Issue Status<br><span class="bold">See More Details</span> button</p> </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">One of my people is added to a project</span> </p> <p>A manager receives an email notification when one of his or her users is added to a project. This notification is sent regardless of the status of the project.&nbsp;</p> <p>Users with a Review license do not receive a notification.</p> <p>The subject of the email is: <em>Project Assignment: &lt;User Name&gt;[&lt;Project GUID&gt;_ &lt;User GUID&gt;]</em></p> </td> 
   <td> <p>Project Name<br>Portfolio Name<br>Project Reference Number<br>Name of the user who added the person to the project<br>Name of the user who was added to the project<br>Project Planned Start Date<br>Project Planned Completion Date<br>Project Percent Complete<br>Names of Others on Project<br>Project Status<br>Project Owner<br><span class="bold">See More Details</span> button<br><br><br></p> </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Someone adds a project to a portfolio or program I own</span> </p> <p>The portfolio and/ or the program owner receive a notification when a new project is added to a portfolio or a program.</p> <p>The subject of the instant notification email is: <em>Project added to &lt;Portfolio Name&gt;[Project GUID]</em></p> </td> 
   <td> Portfolio Name<br>Project Reference Number<br>Name of the user who added the project to the portfolio/ program<br><br></td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Someone shares an object with me</span> </p> <p>You receive an email notification when someone adds you to the Sharing list of permissions on an object.</p> <p>The subject of the instant notification email is: <em>Access Granted: &lt;Object Name&gt;</em></p> </td> 
   <td> Object Name<br>Parent Object Name<br>Object Reference Number<br>Original Access to the object<br>New Access granted to the object<br>Date and Time when the access was granted <br>Name of the user who granted the access </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Someone shares an object with my team</span> </p> <p>You receive an email notification when someone adds your team to the Sharing list of permissions on an object.</p> <p>The subject of the instant notification email is: <em>Access Granted: &lt;Object Name&gt; [Access Rule GUID]</em></p> </td> 
   <td> Object Name<br>Parent Object Name<br>Object Reference Number<br>Old Access<br>New Access<br>Date and Time when the access was granted<br>Name of your team<br>Name of the user who granted the access </td> 
   <td><span class="bold">Instant</span> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">An update is made to a task, issue, or project I am &nbsp; subscribed to</span> </p> <p>You receive an email notification when someone comments on an item to which you are subscribed.</p> <p>The subject of the subscription email is: <em>An update was made to the &lt;Object Type&gt;&nbsp;you are subscribed to: &lt;Object&nbsp;Name&gt;</em></p> </td> 
   <td> Object Name<br> Object Reference Number<br> Name of the user who made a comment on&nbsp;the subscribed item<br> Date comment was made<br> Comment added&nbsp;to the subscribed item&nbsp; </td> 
   <td><span class="bold">Instant&nbsp;</span> </td> 
  </tr> 
 </tbody> 
</table>

