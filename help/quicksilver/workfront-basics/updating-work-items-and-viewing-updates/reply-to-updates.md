---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Reply to updates
description: When someone adds or replies to an update on a work object, their reply appears in the communication thread in the Updates section for the object. You can add a reply to an update or Like it if you have View access to the object.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
---
# Reply to updates

<!--take "Beta" references out when we remove the beta-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
>
>* Issues, <span class="preview">projects, tasks, and documents</span>.
>
>  This is available when you enable the commenting Beta experience.   
>
>  This functionality is available only for the Updates section, and it is not available for the following areas:
>
>  * Home
>  * Summary panel in lists
>  * Summary panel in timesheets
>
>* Goals
>
>  The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>  For information about commenting on goals, see [Manage goal comments in Adobe    Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md). 

When someone replies to a comment or a system update on a work object, their reply appears in the communication thread in the Updates section for the object. 

>[!IMPORTANT]
>
>It is not possible to reply to system updates in the new commenting Beta experience. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>Requestor or higher for issues and documents; Reviewer or higher for all other objects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Reply to an update or a reply

Replying to a comment or reply differs depending on which experience and which object you select.

### Reply to an update or reply in the current Updates section

1. Go to the object to which you want to add a reply.
1. On the **Updates** tab for the object, find the update or reply to which you want to reply.

1. (Optional) To view an image in the existing update do one of the following:

   * Click the **Preview** icon ![](assets/previewimageicon-31x31.png) on the image thumbnail to open the full-size image in a new browser tab.
   * Click the **Download** icon ![](assets/downloadimageicon.png) on the image thumbnail to download the image.

1. Click **Reply** on the update, then type a reply in the box that appears.

   You can see the users who are actively engaged in the conversation or tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)
   
1. (Optional) To include text from a previous update in your reply, click the **More** menu next to the update or reply you want to quote, then click **Quote Reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. (Optional) Use formatting, emojis, include links, or images as explained in the section "Use Rich Text in a Workfront update" in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Click **Reply** to save the reply.

### Reply to a comment when using the commenting Beta experience

1. Go to the object to which you want to add a reply.
1. Click **Updates**, then click the **Comments** tab for the object and find the comment or reply to which you want to reply. 
1. Click **Reply**. 

   You can see the users who are actively engaged in the conversation at the bottom of the **New comment** box and you can add more, or remove the ones that are no longer relevant. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Start typing your reply and use any additional options from the Rich Text toolbar. For information about using Rich Text or other updating capabilities, see [Update work](../updating-work-items-and-viewing-updates/update-work.md). 

1. Click **Submit** to save the reply.

1. (Optional) Click the **More** menu ![](assets/more-menu.png) next to the update for more options to manage the  reply. For more information, see [Update work](../updating-work-items-and-viewing-updates/update-work.md). 


## Reply to an update via email notification

Depending on how your email notifications are configured, you might receive an email notification when an update is made to certain objects to which you have access.

>[!NOTE]
>
>Replying to updates by email is not available for environments on Cluster 6.

The following is an example of an email notification triggered as a result of an update made on the Updates tab of a task:

![email.png](assets/email-350x202.png)

From the email, you can easily add a reply directly to the communications thread of the object in Workfront. You can also add a reply without logging in to Workfront, on an email that is generated from comments made to the following objects:

* Project
* Task
* Issue
* Document
* Template and template task
* Portfolio
* Program
* Iteration
* Timesheet

### Reply to an update from an email notification

When you receive an email notification, you can quickly open the associated Workfront object and add a reply directly to the communication thread.

1. Click **Comment** on the email notification.

   The Details page for the object opens in Workfront.

1. Go to the update to which you want to add a reply.

   In addition to seeing the users who are actively engaged in the conversation, you can see who was tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive notification whenever an update or reply is made on the object. To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Click **Reply,** enter your reply, then click **Reply**.

### Add an update to an object outside of Workfront

When you receive a Workfront email notification, you can quickly add an update to the communication thread without logging in to Workfront.

To add an update to a Workfront email:

1. From your email application, open the Workfront email to which you want to respond, then open a reply email window.
1. Type your update.  
   Attachments are not permitted, and any Rich Text formatting applied to an update in an email does not display on the update when viewed in the Updates tab.
1. Click **Send**.

   Your update is added to the communications thread of the object.
