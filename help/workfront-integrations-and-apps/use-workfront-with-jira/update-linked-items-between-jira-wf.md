---
filename: update-linked-items-between-jira-wf
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Update linked items between Jira and Adobe Workfront
description: When you link Jira issues to Adobe Workfront tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application.
---

# Update linked items between Jira and *Adobe Workfront*

When you link Jira issues to *Adobe Workfront* tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application.&nbsp;

For more information about linking items between *Workfront* and Jira, see [Link items between Adobe Workfront and Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

As you are setting up *Workfront* for Jira, as a Jira system administrator, you can configure certain fields from one application to synchronize with fields from linked items in the other application.

For more information about synchronizing fields between linked Jira and *Workfront* items, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and <em>Workfront</em> to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

Before you can link items between *Workfront* and Jira, you must

* Install *Workfront* for Jira.

  For instructions on installing *Workfront* for Jira, see [Install Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configure *Workfront* for Jira.

  For instructions on configuring *Workfront* for Jira, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Link items between Workfront and Jira.

  For instructions, see [Link items between Adobe Workfront and Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Update linked items in *Workfront*

If you work primarily in *Workfront*, you can update your work items in *Workfront* and their counterparts in Jira also update. This update happens through the integration of *Workfront* for Jira which does not require you to have a Jira license.&nbsp;

As long as your *Workfront administrator* has configured *Workfront* for Jira to synchronize the fields between linked items, certain fields that you update in *Workfront* also update for the linked Jira issue. For more information about updating items in *Workfront*, see [Edit issues](../../manage-work/issues/manage-issues/edit-issues.md) and [Edit tasks](../../manage-work/tasks/manage-tasks/edit-tasks.md).

The following list shows which *Workfront* fields synchronize with Jira fields on linked items:&nbsp;

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Updated <em>Workfront</em> field&nbsp;</span> </th> 
   <th><span class="bold">Synchronized Jira field/ update</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Issue or Task name</td> 
   <td> <p>Issue name</p> <p>A comment about the Name change is added to the <span class="bold"><em>Workfront</em></span> tab of the Jira issue.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Issue or Task Description</td> 
   <td> <p> Issue Description</p> <p>A comment about the updated Description is added to the <span class="bold"><em>Workfront</em></span> tab of the Jira issue.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> Uploaded Documents</p> <p>Note: Documents which are linked to <em>Workfront</em> items from an external server are not transferred&nbsp;to Jira issues. Only documents uploaded directly to <em>Workfront</em> items are also updated to the linked Jira issues.&nbsp;</p> </td> 
   <td> <p> Attachments</p> <p>A comment about the uploaded attachments is added to the <span class="bold"><em>Workfront</em></span> tab of the Jira issue.<br></p> </td> 
  </tr> 
  <tr> 
   <td>Planned Completion Date</td> 
   <td> <p>Due Date</p> <p>A comment about the Due Date having changed is added to the <em>Workfront</em> tab of the Jira issue.&nbsp;</p> <p>Note: You must enable <span class="bold">Due Date</span> for your Jira issues to be able to see this field updated in Jira.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Custom Forms and Custom Fields</td> 
   <td> <p> Display in the <em>Workfront</em> right panel of the Jira issue. <br>Only the Custom Fields that have an actual value display in the panel.<br><img src="assets/custom-form-in-workfront-side-panel-274x309.png" alt="custom_form_in_workfront_side_panel.png" style="width: 274;height: 309;"></p> <p>Note: Custom Form sections are displayed with the access level of the <em>Workfront administrator</em>. </p> </td> 
  </tr> 
  <tr> 
   <td>Issue or Task Priority</td> 
   <td>Displays in the <em>Workfront</em> right panel of the Jira issue. <br>It does not update the issue <span class="bold">Priority</span> field in Jira.&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Log time&nbsp;</td> 
   <td> <p>A comment about the logged time is added in the <span class="bold"><em>Workfront</em></span> tab of the Jira issue. This includes the name of the user who logs the time, as well as the user for whom the time is logged, in case they are different. No time is logged in the <span class="bold">Work log</span> tab in Jira.<br></p> </td> 
  </tr> 
  <tr> 
   <td>Comments</td> 
   <td> <p>The comment is added to the <span class="bold"><em>Workfront</em></span> tab of the Jira issue. It is not added to the <span class="bold">Comments</span> tab of the Jira issue</p> <p>Note: When you link two existing items manually, the comments that were added to the <em>Workfront</em> item before linking it to Jira do not synchronize to the Jira issue.&nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>

## Update linked items in Jira

If you work primarily in Jira, you can update your work items in Jira and their counterparts in *Workfront* also update. You do not have to have a *Workfront* license for the *Workfront* items linked to your Jira issues to receive the updates you are making in Jira.&nbsp;

On condition that your *Workfront administrator* has configured *Workfront* for Jira to synchronize the fields between linked items, certain fields which you update in Jira also update for the linked *Workfront* item.&nbsp;

The following list shows which Jira fields synchronize with *Workfront* fields on linked items:&nbsp;

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Updated Jira Field&nbsp;</span> </th> 
   <th><span class="bold">Synchronized <em>Workfront</em> Field/ Update</span> </th> 
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
    </ul> <p>Note: The Jira status syncs with the first Workfront status that equates with the appropriate status.</p> <p>For more information about statuses of items in <em>Workfront</em>, see <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Issue Assignee</td> 
   <td> <p> Issue or Task Assignee</p> <p>Important: When you assign an item in Jira to a user who does not have a <em>Workfront</em> account, the integration creates a new active user in <em>Workfront</em> only when the <span class="bold">Automatically create a user in </span><em>Workfront</em><span class="bold"> if the Jira user does not have a </span><em>Workfront</em><span class="bold"> account</span> is set to <span class="bold">Always</span>. This user does not occupy a <em>Workfront</em> license. Active users can be assigned to work items in <em>Workfront</em>, but cannot be included in updates. For more information about configuring the automatic creation of <em>Workfront</em> users from Jira, see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuring <em>Workfront</em> for Jira</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Issue Attachments</td> 
   <td> Issue or Task Documents<br>A comment about uploading a new document in Jira is added to the Updates tab of the <em>Workfront</em> issue or task.&nbsp; </td> 
  </tr> 
  <tr> 
   <td>Due Date</td> 
   <td> <p> A comment about the change of the Due Date in Jira is added to the Updates tab of the <em>Workfront</em> issue or task.&nbsp;</p> <p>Note: No dates change on the <em>Workfront</em> issue or task.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> Log time in the <em>Workfront</em> right panel or from the More menu on the Jira issue<br></td> 
   <td> <p>Hours<br>In addition to adding the hours logged in Jira to the linked <em>Workfront</em> item, a comment about logging time is added to the Updates tab of the <em>Workfront</em> item.</p> <p>For more information about logging time on linked Jira issues, including updating the Jira user who is logging the time in <em>Workfront</em>, see <a href="#logging-time-for-linked-jira-and-workfront-items" class="MCXref xref">Log time for Linked Jira and Workfront items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comments&nbsp;<br><br></td> 
   <td> <p>Comments are added to the Updates tab of the <em>Workfront</em> issue or task if the <span class="bold">Comments</span> setting in the SYNCHRONIZE FROM JIRA TO WORKFRONT section of the Setup tab to <span class="bold">Always</span>.</p> <p>For information about configuring <em>Workfront</em> settings in Jira, see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuring <em>Workfront</em> for Jira</a>.</p> <p>For information about commenting on items from linked Jira issues, see <a href="#commenting-from-linked-jira-issues" class="MCXref xref">Comment from a linked Jira issue</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Log time from linked Jira issues

The time that you record for a Jira item in Jira will also transfer to the linked *Workfront*&nbsp;item, regardless of where in Jira you log the time.  
When you log time in Jira in the *Workfront* panel, the time is recorded only in *Workfront*.  
The time you record in *Workfront* does not affect the time of the linked issue in Jira.&nbsp;

>[!NOTE]
>
>If the time is added to a Jira item linked to a *Workfront* task, the Hour Type for the time in *Workfront* is Task Time. If the time is added to a Jira item linked to a *Workfront* issue, the Hour Type for the time in *Workfront* is Issue Time.

A comment is added to the `*Workfront*` tab in Jira and to the `Updates` tab of the item in *Workfront* to record logging the time.  
The time is also displayed in the `Hours` tab of the *Workfront* item.&nbsp;

* [Log time for Linked Jira and Workfront items](#logging-time-for-linked-jira-and-workfront-items)&nbsp;
* [Log time from Jira to a Workfront item](#logging-time-for-workfront-items-only)

### Log time for Linked Jira and *Workfront* items

You can log time from a Jira issue linked to a *Workfront* item, and the time is recorded both on the Jira issue as well as the *Workfront* item.&nbsp;

>[!IMPORTANT]
>
>If the user logging the time in Jira does not exist in *Workfront*, the integration creates a new active user in *Workfront* if the `Automatically create a user in`*Workfront* `if the Jira user does not have a`*Workfront* `account` is set to `Always`. This user does not occupy a *Workfront* license. You can assign active users to work items in *Workfront*, but you cannot include them in updates. For information about configuring the automatic creation of *Workfront* users from Jira, see [Configuring *Workfront* for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

To log time for an item in Jira and have it recorded both in Jira and *Workfront*:

<ol> 
 <li value="1">Log into Jira.</li> 
 <li value="2">Go to the Jira issue which is linked to the <em>Workfront</em> item.</li> 
 <li value="3">Expand the <span class="bold">More</span> menu and click <span class="bold">Log work</span>.<br><img src="assets/log-time-from-more-menu-in-jira-239x232.png" alt="log_time_from_More_menu_in_Jira.png" style="width: 239;height: 232;"><br></li> 
 <li value="4"> In the <span class="bold">Time Spent</span> field, specify the amount of time spent working on this issue. You must specify the time using the following time periods:<br>
  <ul>
   <li>Weeks (w)</li>
   <li>Days (d)</li>
   <li>Hours (h)</li>
  </ul></li> 
 <li value="5">Continue adding information to your time entry, including a <span class="bold">Work Description</span>, then click <span class="bold">Log</span>.<br>The time is added to the <span class="bold">Work log</span> tab of the Jira item, as well as to the <em>Workfront</em> item linked to it.<br>The work description of the time entry is recorded as a note on the hour entry in <em>Workfront</em>.&nbsp;</li> 
</ol>

### Log time from Jira to a *Workfront* item

You can log time just to the linked *Workfront* item from the Jira issue without recording this time to the Jira issue.&nbsp;

<ol> 
 <li value="1">Log into Jira.</li> 
 <li value="2"> <p>Navigate to a Jira issue which is linked to a <em>Workfront</em> item.<br></p> <p>The details of the <em>Workfront</em> item should display in the <em>Workfront</em> right panel of the issue.</p> </li> 
 <li value="3"> <p>Click the <span class="bold">Log Time</span> icon.<br></p> <p> <img src="assets/log-time-in-jira.png" alt="Log_time_in_Jira.png"> </p> </li> 
 <li value="4">Specify the amount of <span class="bold">Hours</span> and <span class="bold">Minutes</span> you want to log for the issue.</li> 
 <li value="5"> <p>Click <span class="bold">Log Time</span>.<br></p> <p>The time is added to the <em>Workfront</em> item.</p> <p>This time is not added to the Work Log tab of the Jira issue.&nbsp;</p> </li> 
</ol>

## Comment from a linked Jira issue

When you comment on a Jira item from the *Workfront* right panel in Jira, the comment is also added to the Updates tab of the linked item in *Workfront*.&nbsp;

To comment from Jira to a *Workfront* item:

<ol> 
 <li value="1">Log into Jira.</li> 
 <li value="2"> <p>Navigate to a Jira issue which is linked to a <em>Workfront</em> item.<br></p> <p>The details of the <em>Workfront</em> item should display in the <em>Workfront</em> right panel of the issue.</p> </li> 
 <li value="3"> Click the <span class="bold">Comments</span> icon in the <em>Workfront</em> panel or n the <span class="bold">Comments</span> tab. <img src="assets/jira-comments-icon.png" alt="Jira_comments_icon.png"><br></li> 
 <li value="4"> <p>Start typing a comment, then click <span class="bold">Send</span>.</p> <p>The comment is added to the following:</p> 
  <ul> 
   <li>The <span class="bold"><em>Workfront</em></span> tab of the Jira issue.</li> 
   <li>The <span class="bold">Comments</span> tab of the Jira issue.</li> 
   <li>The <span class="bold">Updates</span> tab of the linked item in <em>Workfront</em>.</li> 
  </ul> </li> 
</ol>

