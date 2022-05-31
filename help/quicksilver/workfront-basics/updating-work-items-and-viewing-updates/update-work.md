---
filename: update-work
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Update work
description: You can add an update on a Adobe Workfront object (project, task, or issue) to communicate about progress on the object. Users who are assigned or subscribed to the object can view your update. You can also tag users to bring their attention to the update.
---

# Update work

You can add an update on a Adobe Workfront object (project, task, or issue) to communicate about progress on the object. Users who are assigned or subscribed to the object can view your update. You can also tag users to bring their attention to the update.

You&nbsp;can add updates to an object from the following areas of Workfront:

* From a Workfront object, in the Updates  section  
* From the Home area (for tasks and issues)
* From the Summary panel in a list of objects (for tasks and issues)
* From the timesheet (for tasks and issues)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or Edit access for the object the update is on</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add an update to a work item

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section .
1. Click **Start a new update,** then type your update.  

1. (Optional) To add rich text formatting to your update, use any attributes on the **Rich Text** toolbar as you type.

   | **Attribute** |**Toolbar Button** |**Mac Shortcut Keys** |**PC Shortcut Keys** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png)|⌘+b |Ctrl+B |
   | Italics | ![mceclip9.png](assets/mceclip9.png)|⌘+i |Ctrl+I |
   | Underline | ![mceclip8.png](assets/mceclip8.png)|⌘+u |Ctrl+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png)|⌘+K |Ctrl+K |
   | Bulleted List | ![mceclip6.png](assets/mceclip6.png)|⌘+Shift+8 |Ctrl+Shift+8 |
   | Numbered List | ![mceclip5.png](assets/mceclip5.png)|⌘+Shift+7 |&nbsp;Ctrl+Shift+7 |
   | Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |Ctrl+Shift+9 |

   {style="table-layout:auto"}

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

1. (Optional) To insert a Zoom meeting URL in your update, click the **Zoom** icon ![](assets/zoom-icon-updates.png).

   The recipients that you notify can join the meeting after they receive their instant notification in Workfront or via email. For more information on notifying users, see the Notify section below.

   >[!NOTE]
   >
   >* The Zoom integration is available only if your Workfront administrator enabled it, as explained in [Install the Zoom integration](../../administration-and-setup/configure-integrations/enable-zoom-integration.md).
   >* The first time you use this integration, you need to follow the prompts requesting you to connect Zoom to Workfront. You need to do this only once.
   >* Although the integration uses your Zoom account, the Zoom meeting ID that you add to your update is a unique meeting URL, not your personal Zoom meeting room URL.

1. (Optional) To attach an image to your update, click the **Image** icon ![](assets/addimageicon-35x32.png)&nbsp;and browse to the image on your computer.  
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
      <td role="rowheader">Notify</td> 
      <td>Identify users who need to be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commit Date</td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condition</td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>Click the arrow beside&nbsp;the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a&nbsp;work item&nbsp;does not automatically change the status of a project. Depending on how your project is set up, you might need to make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p>Note: You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Completion Bar</td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private to my company</td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update will be posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page.

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

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

Depending on the access&nbsp;your Workfront administrator gives you, you might be able to delete updates you added on the Updates tab of an object. For more information, see&nbsp; [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) in the article [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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

The Updates tab for a Workfront object displays two types of information:

* **User updates:** User updates are comments that you and other users in your system enter.

  ![](assets/user-update-cl-350x277.png)

* **System updates:** System updates record removing assets, adding or deleting versions, attaching or removing an approval request, as well as any edits or changes made to the documents on the object.

  ![](assets/system-updates-cl-350x277.png)

Depending on your Workfront license, system updates might be enabled&nbsp;by default. Workfront administrators can determine what is tracked in system updates,&nbsp;as explained in [System-tracked updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). You can also filter out&nbsp;system updates or activities so that you see&nbsp;only user updates for all objects.

For more information about the difference between user and system updates, see [System-tracked updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

To enable or disable system updates:

1. Click the **Updates** tab on an&nbsp;object.
1. Click **Show System Updates** to slide the switch left (disabled) or right (enabled).

   ![](assets/show-system-updates-qs-350x55.png)

   This option&nbsp;is persistent across all objects throughout Workfront and remains in the position you select, even if you log out of Workfront.

