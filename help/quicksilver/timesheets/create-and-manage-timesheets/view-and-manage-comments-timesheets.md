---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: View and manage comments on a timesheet
description: You can make comments on timesheets, the work items included in the timesheets, as well as on every hour entry that you log. 
author: Alina
feature: Timesheets
exl-id: 6260d176-3cfb-4bc2-93cb-00687e030248
---
# View and manage comments on a timesheet

<!-- Audited: April, 2024-->

You can make comments on the following items in a timesheet:

* On the timesheet
* On the hour entries 
* On an individual item, like a task or an issue

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Light or higher </p>
   <p>Current: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>View access or higher to Tasks and Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## View hour entry comments on a timesheet {#view-hour-entry-comments-on-a-timesheet}

You can configure comments that are made on individual hour entries to be displayed in the timesheet. The option to show and hide comments does not affect comments made on the overall timesheet or comments made on individual items. For more information, see&nbsp; [Make comments on a timesheet](#make-comments-on-a-timesheet).

By default, comments are hidden the first time you access a timesheet.

To show comments on a timesheet:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Timesheets**.
1. Open the timesheet where you want to display comments.
1. Click **Show comments** in the upper-right corner of the timesheet.
   Comments display under the item where the hour entry and the comment were logged.

   ![](assets/comments-expanded-under-tasks-redesigned-timesheet.png)


## Make comments on a timesheet {#make-comments-on-a-timesheet}

* [Comment on the overall timesheet](#comment-on-the-overall-timesheet) 
* [Comment on an individual hour entry in a timesheet](#comment-on-an-individual-hour-entry-in-a-timesheet) 
* [Comment on a work item in a timesheet](#comment-on-a-work-item-in-a-timesheet)

### Comment on the overall timesheet {#comment-on-the-overall-timesheet}

You can make general comments about the timesheet. Commenting on the overall timesheet is similar to commenting on other objects. 

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available.

1. Click **Timesheets**.
1. Go to the timesheet where you want to make a comment.
1. Click **Updates** in the left panel, then click the **Comments** tab.
1. Start adding new comments or reply to existing ones, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Add people or teams in the **Tag people or teams** field to include others in your update. For more information, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
1. (Optional) Select the **Private to my company** option if you want only people from your company to view the update.
1. Type your comment, then click **Submit**.

   Your comment displays in the [!UICONTROL Updates] section of the timesheet, in the Comemnts tab.

1. (Optional) Click the **System Activity** tab to review system-generated updates

   Or 

   Click the **All** tab to view system activity and user comments in a chronological order. 
         
      >[!TIP]
      >
      >   The All tab is a read-only tab and you cannot reply to comments from there. 


   For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

### Comment on an individual hour entry in a timesheet {#comment-on-an-individual-hour-entry-in-a-timesheet}

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Timesheets**.
1. Go to the timesheet where you want to make a comment and click **Timesheet** in the left panel.
1. Click in the hour entry field where you want to make a comment and click **Comment** to add a comment for your hour entry. 

   >[!TIP]
   >
   >   When using a standard QWERTY keyboard after clicking the hour entry box, press the following set of keys to open the comment box:
   >   * Shift + F2 for both Windows and Mac computers. 

   Do one of the following:

   * Type a new comment and click **Done**.
   * Edit an existing comment and click **Done**, or click **Cancel** to discard the changes.
   * Click the **Delete** icon ![](assets/delete.png) to delete a saved comment.
   
      A blue marker appears in the upper-right corner of the hour entry box to indicate that there are comments logged with the time entry.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   When using a standard QWERTY keyboard, from inside the comment box, press the following set of keys to save the comment:
   >   * Ctrl + Enter for Windows computers.
   >   * Cmd + Return for Mac computers.
   

1. (Optional) To configure hour-entry comments to display in the timesheet, see the section [View hour-entry comments on a timesheet](#view-hour-entry-comments-on-a-timesheet) in this article.

### Comment on a work item in a timesheet {#comment-on-a-work-item-in-a-timesheet}

>[!TIP]
>
>You can comment on individual items in the timesheet, update their Actual Start Date or Condition. The update displays in the Updates area of the object associated with the logged time.


You can comment only on tasks and issues in a timesheet. You cannot comment on projects or general time. 

1. Click the [!UICONTROL **Main Menu**] icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.
1. Click [!UICONTROL **Timesheets**].
1. Go to the timesheet where you want to make a comment, and click [!UICONTROL **Timesheet**] in the left panel.
1. Click the row of a task or an issue, then click [!UICONTROL **Open Summary**]. 
1. Start typing an update in the [!UICONTROL **Updates**] area of the Summary panel, then click [!UICONTROL **Submit**].
The update displays in the Updates section of the task and issue.
1. (Optional) Click [!UICONTROL **Close Summary**] to close the Summary panel. 

   For more information about updating tasks and issues in the Summary panel, see [Summary overview](../../workfront-basics/the-new-workfront-experience/summary-overview.md).
