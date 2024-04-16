---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Reply to updates
description: When someone adds or replies to an update on a work object, their reply appears in the communication thread in the Updates section for the object. You can add a reply to an update or Like it if you have View access to the object.
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
---
# Reply to updates

<!-- Audited: April 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

When someone replies to a comment or a system update on a work object, their reply appears in the communication thread in the Comments and All tabs in the Updates section for the object. 

>[!IMPORTANT]
>
>It is not possible to reply to system updates in the System Activity tab. Any replies to system updates made in the legacy commenting experience prior to April 11, 2024 display as read-only . 

This article describes how you reply to comments from most objects in Workfront. For differences between the Updates sections of various objects, see [Updates section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md). 

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p> 
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Reply to an update or a reply in Workfront

You can reply to a comment in the thread of an object that you can view, or you can log in as a Workfront or group administrator and reply to a comment on behalf of another user. For more information, see [Log in as another user](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md). 

### Reply to a comment 

Reply to a comment in the Updates section of an object is similar for most objects in Workfront.

1. Go to the object to which you want to add a reply.
1. Click **Updates**, then click the **Comments** tab for the object and find the comment or reply to which you want to reply

   Or

   Click the **All** tab, then click **Reply in Comments** to open the comment in the Comments tab and reply to it. You cannot reply in the All tab.

1. (Optional) To include text from a previous update in your reply, click the **More** menu in the upper-right corner of the comment you want to reply to, then click **Quote reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. Click **Reply**.

   ![](assets/reply-to-update-empty-box.png)

   You can see the users who are actively engaged in the conversation at the bottom of the **Add reply...** box and you can add more, or remove the ones that are no longer relevant. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   To add additional replies to an existing reply, you can start typing in the **Add reply ...** box, or click **Reply** on the original comment. Your reply is added at the end of the thread.
   
1. Start typing your reply and use any additional options from the Rich Text toolbar. For information about using Rich Text or other updating capabilities, see [Update work](../updating-work-items-and-viewing-updates/update-work.md). 

1. Click **Submit** to save the reply.

1. (Optional) Click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the comment you want to reply to for more options to manage the reply. For more information, see [Update work](../updating-work-items-and-viewing-updates/update-work.md). 

<!--
### Reply to an update or reply in the legacy Updates section

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

-->

## Reply to an update from an email notification

Depending on how your email notifications are configured, you might receive an email notification when an update is made to certain objects to which you have access.

You can reply to an update from an email notification in the following ways:

* Reply to the email that you receive. Your reply email is added as a Workfront reply to the original comment.
* Use the Comment button inside the email to navigate back to Workfront and reply to the update in the Updates area. 

The following is an example of an email notification triggered as a result of an update made on the Updates tab of a task:

![email.png](assets/email-350x202.png)

For information, see [Reply to email notifications](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md). 






