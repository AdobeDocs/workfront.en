---
content-type: reference
navigation-topic: notifications
title: 'Notifications: Communication'
description: The following notifications alert you about communication, such as an update comment, happening on a work item you are involved with. For information about configuring which notifications you receive, see Modify your own email notifications.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
---
# Notifications: Communication

The following notifications alert you about communication, such as an update comment, happening on a work item you are involved with. For information about configuring which notifications you receive, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>These notifications alert you about all comments that have been posted on a specific item. For this reason, you must select or deselect all of the notifications at the same time to be delivered in a daily digest email. If you want to be notified about certain comments only as they happen, you can specify the individual notifications be for instant delivery.

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
   <td> <p><strong>Someone includes me on a directed update</strong> </p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] updates</a>.</p> <p>In this case, the user who is included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only if the user has access rights to the object.</p> <p>The subject of the instant notification email is: <em>&lt;Name of the user who included you in the update> [!UICONTROL wanted you to know]</em></p> <p>The subject of the daily digest notification is: <em>[!UICONTROL Digest of Communication] &lt;Date of daily digest></em></p> </td> 
   <td> Object Name where the update was made<br>Parent Object Name<br>Object Reference Number<br>Names of all users and teams included in the directed update<br>Date and Time when the update was made<br>Text of directed update<br><strong>[!UICONTROL Comment]</strong> button<br>*Total number of comments received<br>*Number of comments received for each object<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of the daily digest<br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone replies to my request</strong> </p> <p>After a user submits a work request and another user replies to that work request, the user who submitted the request receives an email notification.</p> <p>An email notification is not sent if:</p> 
    <ul> 
     <li> <p>The user who replies is the same user who made the request</p> </li> 
     <li> <p>The user does not have access to see the note</p> </li> 
    </ul><strong>The subject of the instant notification email is: <em>[!UICONTROL Comment on] &lt;Request Name> on &lt;Project Name> (ref# &lt;Request Reference Number>)</em></strong> The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></td> 
   <td> Request Name<br>Project name<br>Reference Number<br>Name of the user who replied to your Request<br>Date and Time when the comment was made<br>Text of comment made on your Request<br>*Total number of comments received<br>*Number of comments received for each request<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of the daily digest<br></td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A comment is posted on my request</strong> </p> <p>The primary contact for an issue receives an email notification when a comment is posted on a [!UICONTROL Help Desk] request, unless the user who posted the comment is also the primary contact for the issue.</p> <p>Any users who are directly included in the comment also receive an email notification.</p> <p>A notification is sent only if the project status is [!UICONTROL Current].</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Comment on] &lt;Request Name> on &lt;Project Name> (ref# &lt;Request Reference Number>)</em></p> <p>The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></p> </td> 
   <td> Request Name<br>Project name<br>Reference Number<br>Name of the user who replied to your Request<br>Date and Time when the comment was made<br>Text of comment made on your Request<br>*Total number of comments received<br>*Number of comments received for each request<br>*Project Name<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of the daily digest<br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A comment is added on my document</strong> </p> <p>The owner of a document in [!DNL Adobe Workfront] receives an email notification when a comment is posted on the document, unless the user who posted the comment is also the document owner.</p> <p>Any users who are directly included in the comment also receive an email notification.</p> <p>A notification is sent only if the project status is [!UICONTROL Current]. </p> <p>The subject of the instant notification email is: <em>[!UICONTROL Comment on] &lt;Request Name> on &lt;Project Name> (ref# &lt;Request Reference Number>)</em></p> <p> The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></p> </td> 
   <td>Document Name<br>Project, Task, or Issue Name<br>Reference Number<br>Name of the user who replied to your Request<br>Date and Time when the comment was made<br>Text of comment made on the document</td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone comments on a thread I'm in</strong> </p> <p>Participants in the thread and users who are included in a direct message receive an email notification when a user makes a comment in the thread.</p> <p>Users must have [!UICONTROL View] access to receive a notification.</p> <p>The following users do not receive a notification:</p> 
    <ul> 
     <li>Teams that are included in a direct message</li> 
     <li>The owner of the Note</li> 
     <li>The Primary Contact</li> 
    </ul> <p><strong>The subject of the instant notification email is: <em>[!UICONTROL RE: Comment on] &lt;Object Name>&lt;Object Type> on &lt;Project Name>(ref# &lt;Object Reference Number></em>)</strong> </p> <p><strong> The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></strong> </p> </td> 
   <td> Object Name<br>Parent Object Name<br>Name of the user who commented on the thread<br>Text of comment made on the thread<br>Date and Time when the comment was made<br>*Total number of comments received<br>*Number of comments received for each object<br>*Project Name<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of daily digest </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone comments on one of my work items</strong> </p> <p>The assignee of the work item receives an email notification any time a user adds an update to a work item, unless the user who adds the update is also the assignee. </p> <p>When a comment is posted on a request, email the issue primary contact.</p> <p>The primary contact for an issue receives an email notification when a comment is posted on a request, unless the user who posted the comment is also the primary contact for the issue.</p> <p>Any users who are directly included in the comment also receive an email notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Comment on] &lt;Work Item Name> on &lt;Project Name (ref# &lt;Work Item Reference Number>)</em></p> <p> The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></p> </td> 
   <td> Work Item Name<br>Project Name<br>Work Item Reference Number<br>Name of the user who commented on the Work Item<br>Text of the comment made on the Work Item<br>Date and Time when the comment was made<br>*Total number of comments received<br>*Number of comments received for each object<br>*Project Name<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of daily digest </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Someone includes my team on a directed update</strong> </p> <p>A directed update is when a user specifically includes another user in an update, as described in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p> <p>In this case, any member of the team included in the directed update receives an email notification about the update.</p> <p>The email notification is sent only to users who have access rights to the object.</p> <p>If the user sending the directed update is a member of the team being included, the user sending the update does not receive an email notification.</p> <p>The subject of the instant notification email is: [!UICONTROL Comment on] &lt;Object name> on &lt;Parent Object Name> (ref# &lt;Object Reference Number>)</p> <p> The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></p> </td> 
   <td> <p>Object Name<br>Parent Object Name<br>Object Reference Number<br>Name of the user who made the directed update<br>Name of all the teams and users included in the directed update<br>Date and Time when the directed update was made<br>Text of the directed update<br><strong>[!UICONTROL Comment]</strong> button<br>*Total number of comments received<br>*Number of comments received for each object<br>*Project Name<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of daily digest </p> </td> 
   <td><strong>Daily</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>When comment is added on user</strong> </p> <p>You can make a comment on a user in the [!UICONTROL Updates] tab of the user object. You can also make a comment on a user when you are editing the settings of the user. The user against which the comment is made gets an email to notify them of this comment. </p> <p>You must have permissions to at least [!UICONTROL View] the user in order to enter an update on the [!UICONTROL Updates] tab of the user. You must have [!UICONTROL Edit] permissions on the user in order to edit the settings of the user. </p> <p>For more information about making comments on users in the Updates tab, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</p> <p>For more information about entering a comment on a user when you edit the settings of the user, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.</p> <p>The subject of the instant notification email is: <em>&lt;User Name> [!UICONTROL wanted you to know]</em></p> <p>The subject of the daily digest notification is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest></em></p> </td> 
   <td> Your User Name<br>Name of the user who added the comment<br>Text of the comment<br>Date and Time the comment was made<br>*Total number of comments received<br>*Number of comments received for each object<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Date of daily digest </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>and Daily</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
