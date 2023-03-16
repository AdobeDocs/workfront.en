---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Update work
description: You can add an update on a Adobe Workfront object (project, task, or issue) to communicate about progress on the object. Users who are assigned or subscribed to the object can view your update. You can also tag users to bring their attention to the update.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
---
# Update work

<!-- Drafted for commenting experience: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

You can add comments to several objects in Workfront. For more information, see [Updates tab overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md). 

You can add an update on a Adobe Workfront object (project, task, or issue) to communicate about progress on the object, in addition to commenting on it. Users who are assigned or subscribed to the object can view your update. You can also tag users to bring their attention to the update. 

The information on this page refers to updating work for projects, tasks, or issues. For information about adding comments and updaes to goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).

You can update project, tasks, and issues from the following areas of Workfront:

* From a Workfront object, in the Updates  section  
* From the Home area (for tasks and issues)
* From the Summary panel in a list of objects (for tasks and issues)
* From the timesheet (for tasks and issues)

## Access requirements

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add an update to a work item

<!--drafted for the commenting experience - change the NOTE at the top of this paragraph with every new release to other objects

Adding an update to a work item differs depending on what environment and what object you choose. 

### Add an update to a work item in the Production environment

>[!NOTE]
>
>The following functionality is available for all objects except for goals, in the Production and Preview environments. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. Click **Start a new update,** then type your update.  

1. (Optional) To add rich text formatting to your update, use any attributes on the **Rich Text** toolbar as you type.

   | **Attribute** |**Toolbar Button** |**Mac Shortcut Keys** |**PC Shortcut Keys** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png)|⌘+b |Ctrl+B |
   | Italics | ![mceclip9.png](assets/mceclip9.png)|⌘+i |Ctrl+I |
   | Underline | ![mceclip8.png](assets/mceclip8.png)|⌘+u |Ctrl+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png)|⌘+K |Ctrl+K |
   | Bulleted List | ![mceclip6.png](assets/mceclip6.png)|⌘+Shift+8 |Ctrl+Shift+8 |
   | Numbered List | ![mceclip5.png](assets/mceclip5.png)|⌘+Shift+7 |Ctrl+Shift+7 |
   | Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |Ctrl+Shift+9 |

    To stop formatting text, deselect the attribute on the **Rich Text** toolbar.

   >[!NOTE]
   >
   >* Formatting also displays in any email notification users receive containing your update.
   >* Rich Text formatting applied to an update in an email does not display on the update when viewed in the Updates tab.  
   >* If your organization uses Workfront with Internet Explorer, any formatted text pasted into an update loses its Rich Text formatting and displays as plain text. You can reformat the text using the attributes on the Rich Text toolbar.
   >* Rich Text formatting is not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.

1. (Optional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting.

   ![](assets/block-quote-marked-350x144.png)

1. (Optional) Add any emojis to your update.

   >[!NOTE]
   >
   >* Workfront does not replace punctuation emoticons such as :) with emojis.
   >* Emojis are not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.
   >* The emoji feature in Workfront utilizes Unicode characters and, as such, displays only on browsers and operating systems that support Unicode code points. Users on a platform, browser, or operating system version different than yours might not have access to the same emojis.
   >* An unsupported emoji is represented by a black or white box.
   >* Windows 7 supports only black and white emojis.  
   >* Emojis that are applied to an update made via email do not display on the update when viewed in the Updates area.

1. (Optional) To add a URL link to additional information sources:

   1. Click in your update where you want to insert a link.
   1. On the **Rich Text** toolbar, click the **Hyperlink** icon. ![](assets/link-icon.png)  

   1. In the **Create Link** box that appears, under **URL**, type or paste the URL of the source to which you want to link.
   
   1. Under **Text to display**, type or paste the link text.
   1. Click **Save**.



1. (Optional) To attach an image to your update, click the **Image** icon ![](assets/addimageicon-35x32.png) and browse to the image on your computer.  
   Or  
   Drag the image into the update area.

   >[!NOTE]
   >
   >* Your Workfront administrator must enable adding images before you can see the Image icon.
   >* The maximum image file size is 7 MB. Supported image file types are .jpg, .gif, and .png.
   >* Images are accessible only from the Updates tab on an object, and they are not available on the Documents tab.
   >* You can send an update with an image and no text.

1. (Optional) Specify any of the following items:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who need to be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might need to make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update will be posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--
### Add an update to a work item in the Preview environment

>[!NOTE]
>
> In the Preview environment, the following functionality is available only for issues, after opting in the Beta program for the new commenting experience.
> 
> In the Production environment, the following functionality is available for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md). 

1. Locate the object you want to add comments to, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Activate the **Beta** toggle in the upper-right corner of the Updates area. This switches the Updates area to the new commenting experience. 
1. Click the **Comments** tab in the upper-left corner of the Updates area.
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any attributes on the **Rich Text** toolbar as you type.

   | **Attribute** |**Toolbar Button** |**Mac Shortcut Keys** |**PC Shortcut Keys** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png)|⌘+b |Ctrl+B |
   | Italics | ![mceclip9.png](assets/mceclip9.png)|⌘+i |Ctrl+I |
   | Underline | ![mceclip8.png](assets/mceclip8.png)|⌘+u |Ctrl+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png)|⌘+K |Ctrl+K |
   | Bulleted List | ![mceclip6.png](assets/mceclip6.png)|⌘+Shift+8 |Ctrl+Shift+8 |
   | Numbered List | ![mceclip5.png](assets/mceclip5.png)|⌘+Shift+7 |Ctrl+Shift+7 |
   | Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |Ctrl+Shift+9 |

    To stop formatting text, deselect the attribute on the **Rich Text** toolbar.

   >[!NOTE]
   >
   >* Formatting also displays in any email notification users receive containing your update.
   >* Rich Text formatting applied to an update in an email does not display on the update when viewed in the Updates tab.  
   >* If your organization uses Workfront with Internet Explorer, any formatted text pasted into an update loses its Rich Text formatting and displays as plain text. You can reformat the text using the attributes on the Rich Text toolbar.
   >* Rich Text formatting is not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.

   ************ HIDE THIS ********* 1. (Optional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting.

   ********  HIDE THIS ******** 1. (Optional) Add any emojis to your update.

   >[!NOTE]
   >
   >* Workfront does not replace punctuation emoticons such as :) with emojis.
   >* Emojis are not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.
   >* The emoji feature in Workfront utilizes Unicode characters and, as such, displays only on browsers and operating systems that support Unicode code points. Users on a platform, browser, or operating system version different than yours might not have access to the same emojis.
   >* An unsupported emoji is represented by a black or white box.
   >* Windows 7 supports only black and white emojis.  
   >* Emojis that are applied to an update made via email do not display on the update when viewed in the Updates area.

1. (Optional) To add a URL link to additional information sources:

   1. Click in your update where you want to insert a link.
   1. On the **Rich Text** toolbar, click the **Hyperlink** icon. ![](assets/link-icon.png)  

   1. In the **Create Link** box that appears, under **URL**, type or paste the URL of the source to which you want to link.
   
   1. Under **Text to display**, type or paste the link text.
   1. Click **Save**.   
1. Click **Submit**. 
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********)
1. (Optional) Click the **Like** icon![](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click on the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When a goal is updated, Workfront generates a note about that update that and displays it in the System Activity tab. Workfront also records a system update when a result, activity, or project is added to the goal or when it is updated. 

-->
 


## Copy update information

There are several ways you can copy an update. After copying a link, you can share the link with others to direct them to the update.

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)

### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![Select Copy body text](assets/update-stream-copy-body-text-350x152.png)

### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.
1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Delete an update or reply

Depending on the access your Workfront administrator gives you, you might be able to delete updates you added on the Updates tab of an object. For more information, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) in the article [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

No Workfront user (including the Workfront administrator) can delete updates made by another user. However, if a user's access level allows them to delete their own updates, the Workfront administrator can log in as that user and delete updates they made. For more information, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) and [Log in as another user](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Go to the update or reply you want to delete.
1. Click the **More** menu next to the update or reply you wish to delete, then click **Delete**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. In the message that appears, click **Confirm**.

>[!NOTE]
>
>Deleting an update with an attached image deletes both the comment and the image.

## Add an update on a Timesheet

1. Go to a Timesheet on which you want to make an update.
1. Click the Timesheet to open it.
1. At the bottom of the Timesheet, click **Include a comment**.
1. In the box that displays at the bottom of the Timesheet, type an update.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Conditional)To save your update without submitting the Timesheet for approval, click **Save for Later**.

   Or

   To save your update and submit the Timesheet for approval, click **Submit for Approval**.

   Or

   If your Timesheet is not set up with an approver, click **Save and Close Timesheet** to save your update.

## Enable or disable system updates

The Updates section for a Workfront object displays two types of information:

* **User updates:** User updates are comments that you and other users in your system enter.

  ![](assets/user-update-cl-350x277.png)

* **System updates:** System updates record removing assets, adding or deleting versions, attaching or removing an approval request, as well as any edits or changes made to the documents on the object.

  ![](assets/system-updates-cl-350x277.png)

Depending on your Workfront license, system updates might be enabled by default. Workfront administrators can determine what is tracked in system updates, as explained in [System-tracked updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). You can also filter out system updates or activities so that you see only user updates for all objects.

For more information about the difference between user and system updates, see [System-tracked updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

To enable or disable system updates:

1. Click the **Updates** tab on an object.
1. Click **Show System Updates** to slide the switch left (disabled) or right (enabled).

   ![](assets/show-system-updates-qs-350x55.png)

   This option is persistent across all objects throughout Workfront and remains in the position you select, even if you log out of Workfront.

