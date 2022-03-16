---
filename: update-linked-items-between-jira-wf
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Update linked items between Jira and Adobe Workfront
description: When you link Jira issues to Adobe Workfront tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application.
---

# Update linked items between Jira and Adobe Workfront

When you link Jira issues to Adobe Workfront tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application.&nbsp;

For more information about linking items between Workfront and Jira, see [Link items between Adobe Workfront and Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

As you are setting up Workfront for Jira, as a Jira system administrator, you can configure certain fields from one application to synchronize with fields from linked items in the other application.

For more information about synchronizing fields between linked Jira and Workfront items, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and Workfront to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you can link items between Workfront and Jira, you must

* Install Workfront for Jira.

  For instructions on installing Workfront for Jira, see [Install Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configure Workfront for Jira.

  For instructions on configuring Workfront for Jira, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Link items between Workfront and Jira.

  For instructions, see [Link items between Adobe Workfront and Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Update linked items in Workfront

If you work primarily in Workfront, you can update your work items in Workfront and their counterparts in Jira also update. This update happens through the integration of Workfront for Jira which does not require you to have a Jira license.&nbsp;

As long as your Workfront administrator has configured Workfront for Jira to synchronize the fields between linked items, certain fields that you update in Workfront also update for the linked Jira issue. For more information about updating items in Workfront, see [Edit issues](../../manage-work/issues/manage-issues/edit-issues.md) and [Edit tasks](../../manage-work/tasks/manage-tasks/edit-tasks.md).

The following list shows which Workfront fields synchronize with Jira fields on linked items:&nbsp;

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Updated Workfront field&nbsp;</span> </th> 
   <th><span class="bold">Synchronized Jira field/ update</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Issue or Task name</td> 
   <td> <p>Issue name</p> <p>A comment about the Name change is added to the <span class="bold">Workfront</span> tab of the Jira issue.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Issue or Task Description</td> 
   <td> <p> Issue Description</p> <p>A comment about the updated Description is added to the <span class="bold">Workfront</span> tab of the Jira issue.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> Uploaded Documents</p> <p>Note: Documents which are linked to Workfront items from an external server are not transferred&nbsp;to Jira issues. Only documents uploaded directly to Workfront items are also updated to the linked Jira issues.&nbsp;</p> </td> 
   <td> <p> Attachments</p> <p>A comment about the uploaded attachments is added to the <span class="bold">Workfront</span> tab of the Jira issue.<br></p> </td> 
  </tr> 
  <tr> 
   <td>Planned Completion Date</td> 
   <td> <p>Due Date</p> <p>A comment about the Due Date having changed is added to the Workfront tab of the Jira issue.&nbsp;</p> <p>Note: You must enable <span class="bold">Due Date</span> for your Jira issues to be able to see this field updated in Jira.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Custom Forms and Custom Fields</td> 
   <td> <p> Display in the Workfront right panel of the Jira issue. <br>Only the Custom Fields that have an actual value display in the panel.<br><img src="assets/custom-form-in-workfront-side-panel-274x309.png" alt="custom_form_in_workfront_side_panel.png" style="width: 274;height: 309;"></p> <p>Note: Custom Form sections are displayed with the access level of the Workfront administrator. </p> </td> 
  </tr> 
  <tr> 
   <td>Issue or Task Priority</td> 
   <td>Displays in the Workfront right panel of the Jira issue. <br>It does not update the issue <span class="bold">Priority</span> field in Jira.&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Log time&nbsp;</td> 
   <td> <p>A comment about the logged time is added in the <span class="bold">Workfront</span> tab of the Jira issue. This includes the name of the user who logs the time, as well as the user for whom the time is logged, in case they are different. No time is logged in the <span class="bold">Work log</span> tab in Jira.<br></p> </td> 
  </tr> 
  <tr> 
   <td>Comments</td> 
   <td> <p>The comment is added to the <span class="bold">Workfront</span> tab of the Jira issue. It is not added to the <span class="bold">Comments</span> tab of the Jira issue</p> <p>Note: When you link two existing items manually, the comments that were added to the Workfront item before linking it to Jira do not synchronize to the Jira issue.&nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>

## Update linked items in Jira

If you work primarily in Jira, you can update your work items in Jira and their counterparts in Workfront also update. You do not have to have a Workfront license for the Workfront items linked to your Jira issues to receive the updates you are making in Jira.&nbsp;

On condition that your Workfront administrator has configured Workfront for Jira to synchronize the fields between linked items, certain fields which you update in Jira also update for the linked Workfront item.&nbsp;

The following list shows which Jira fields synchronize with Workfront fields on linked items:&nbsp;

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Updated Jira Field&nbsp;</span> </th> 
   <th><span class="bold">Synchronized Workfront Field/ Update</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Issue Status</td> 
   <td> <p> Issue or Task Status</p> <p>Issue status in Jira syncs with the following statuses, or statuses that equate with the following statuses, in Workfront:</p> 
    <ul> 
     <li> <p>New (NEW)</p> </li> 
     <li> <p>In Progress (INP)</p> </li> 
     <li> <p>Closed/Complete (CLS/CPL)</p> </li> 
    </ul> <p>Note: The Jira status syncs with the first Workfront status that equates with the appropriate status.</p> <p>For more information about statuses of items in Workfront, see <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Issue Assignee</td> 
   <td> <p> Issue or Task Assignee</p> <p>Important: When you assign an item in Jira to a user who does not have a Workfront account, the integration creates a new active user in Workfront only when the <span class="bold">Automatically create a user in </span>Workfront<span class="bold"> if the Jira user does not have a </span>Workfront<span class="bold"> account</span> is set to <span class="bold">Always</span>. This user does not occupy a Workfront license. Active users can be assigned to work items in Workfront, but cannot be included in updates. For more information about configuring the automatic creation of Workfront users from Jira, see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuring Workfront for Jira</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Issue Attachments</td> 
   <td> Issue or Task Documents<br>A comment about uploading a new document in Jira is added to the Updates tab of the Workfront issue or task.&nbsp; </td> 
  </tr> 
  <tr> 
   <td>Due Date</td> 
   <td> <p> A comment about the change of the Due Date in Jira is added to the Updates tab of the Workfront issue or task.&nbsp;</p> <p>Note: No dates change on the Workfront issue or task.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> Log time in the Workfront right panel or from the More menu on the Jira issue<br></td> 
   <td> <p>Hours<br>In addition to adding the hours logged in Jira to the linked Workfront item, a comment about logging time is added to the Updates tab of the Workfront item.</p> <p>For more information about logging time on linked Jira issues, including updating the Jira user who is logging the time in Workfront, see <a href="#logging-time-for-linked-jira-and-workfront-items" class="MCXref xref">Log time for Linked Jira and Workfront items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comments&nbsp;<br><br></td> 
   <td> <p>Comments are added to the Updates tab of the Workfront issue or task if the <span class="bold">Comments</span> setting in the SYNCHRONIZE FROM JIRA TO WORKFRONT section of the Setup tab to <span class="bold">Always</span>.</p> <p>For information about configuring Workfront settings in Jira, see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuring Workfront for Jira</a>.</p> <p>For information about commenting on items from linked Jira issues, see <a href="#commenting-from-linked-jira-issues" class="MCXref xref">Comment from a linked Jira issue</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Log time from linked Jira issues

The time that you record for a Jira item in Jira will also transfer to the linked Workfront&nbsp;item, regardless of where in Jira you log the time.  
When you log time in Jira in the Workfront panel, the time is recorded only in Workfront.  
The time you record in Workfront does not affect the time of the linked issue in Jira.&nbsp;

>[!NOTE]
>
>If the time is added to a Jira item linked to a Workfront task, the Hour Type for the time in Workfront is Task Time. If the time is added to a Jira item linked to a Workfront issue, the Hour Type for the time in Workfront is Issue Time.

A comment is added to the `Workfront` tab in Jira and to the `Updates` tab of the item in Workfront to record logging the time.  
The time is also displayed in the `Hours` tab of the Workfront item.&nbsp;

* [Log time for Linked Jira and Workfront items](#logging-time-for-linked-jira-and-workfront-items)&nbsp;
* [Log time from Jira to a Workfront item](#logging-time-for-workfront-items-only)

### Log time for Linked Jira and Workfront items

You can log time from a Jira issue linked to a Workfront item, and the time is recorded both on the Jira issue as well as the Workfront item.&nbsp;

>[!IMPORTANT]
>
>If the user logging the time in Jira does not exist in Workfront, the integration creates a new active user in Workfront if the `Automatically create a user in`Workfront `if the Jira user does not have a`Workfront `account` is set to `Always`. This user does not occupy a Workfront license. You can assign active users to work items in Workfront, but you cannot include them in updates. For information about configuring the automatic creation of Workfront users from Jira, see [Configuring Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

To log time for an item in Jira and have it recorded both in Jira and Workfront:

1. Log into Jira.
1. Go to the Jira issue which is linked to the Workfront item.
1. Expand the `More` menu and click `Log work`.  
   ![log_time_from_More_menu_in_Jira.png](assets/log-time-from-more-menu-in-jira-239x232.png)  

1. In the `Time Spent` field, specify the amount of time spent working on this issue. You must specify the time using the following time periods:

  * Weeks (w)
  * Days (d)
  * Hours (h)

1. Continue adding information to your time entry, including a `Work Description`, then click `Log`.  
   The time is added to the `Work log` tab of the Jira item, as well as to the Workfront item linked to it.  
   The work description of the time entry is recorded as a note on the hour entry in Workfront.&nbsp;

### Log time from Jira to a Workfront item

You can log time just to the linked Workfront item from the Jira issue without recording this time to the Jira issue.&nbsp;

1. Log into Jira.
1. Navigate to a Jira issue which is linked to a Workfront item.

   The details of the Workfront item should display in the Workfront right panel of the issue.

1. Click the `Log Time` icon.

   ![Log_time_in_Jira.png](assets/log-time-in-jira.png)

1. Specify the amount of `Hours` and `Minutes` you want to log for the issue.

1. Click `Log Time`.

   The time is added to the Workfront item.

   This time is not added to the Work Log tab of the Jira issue.&nbsp;

## Comment from a linked Jira issue

When you comment on a Jira item from the Workfront right panel in Jira, the comment is also added to the Updates tab of the linked item in Workfront.&nbsp;

To comment from Jira to a Workfront item:

1. Log into Jira.
1. Navigate to a Jira issue which is linked to a Workfront item.

   The details of the Workfront item should display in the Workfront right panel of the issue.

1. Click the `Comments` icon in the Workfront panel or n the `Comments` tab. ![Jira_comments_icon.png](assets/jira-comments-icon.png)  

1. Start typing a comment, then click `Send`.

   The comment is added to the following:

  * The `Workfront` tab of the Jira issue.
  * The `Comments` tab of the Jira issue.
  * The `Updates` tab of the linked item in Workfront.

