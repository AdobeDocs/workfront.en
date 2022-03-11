---
filename: receive-workfront-notifications-in-slack
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Receive Adobe Workfront notifications in Slack
description: After you have installed Adobe Workfront for Slack, you can receive Workfront notifications in Slack. For information about installing Workfront for Slack, see Configure Adobe Workfront for Slack.
---

# Receive Adobe Workfront notifications in Slack

After you have installed Adobe Workfront for Slack, you can receive Workfront notifications in Slack.  
For information about installing Workfront for Slack, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

You can enable a select number of notifications that appear in the notifications bubble in the Workfront interface, to also be delivered in Slack.

Email notifications work independently from Workfront interface notifications. You or your Workfront administrator can disable email notifications, whereas interface notifications cannot be disabled in Workfront.  
You can, however, disable Workfront notifications that you might receive in Slack, if you want to focus on those notifications only inside the Workfront interface.&nbsp;

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
  </tr> <!--
   Adobe Workfront licenses overview* Plan
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.\

## Prerequisites

Before you can receive Workfront notifications in Slack, you must

* Configure Workfront for Slack  
  For instructions on configuring Workfront for Slack, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configure Workfront notifications for Slack

<ol> 
 <li value="1">(Conditional) After Workfront has been added to your Slack instance, log into Workfront from Slack.<br>For information about logging into Workfront from Slack, see <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md" class="MCXref xref">Access Adobe Workfront from Slack</a>.</li> 
 <li value="2">From any channel, start typing one of the following commands in the message field:&nbsp;<br><pre>/workfront settings</pre> Or<br><pre>/wf settings</pre><pre><img src="assets/slack-configuring-settings-350x302.png" style="width: 350;height: 302;"></pre><br></li> 
 <li value="3">All notifications are enabled, by default. <br>Disable any of the following notifications:&nbsp; 
  <ul>
   <li>I'm assigned to a new task or issue</li>
   <li>My team is assigned to a new task or issue</li>
   <li>I receive a new approval or access request</li>
   <li>Someone includes me on a directed update</li>
   <li>Someone comments on a thread I'm in</li>
   <li>An update is made to a task, issue or project I am subscribed to</li>
   <li>Someone comments on one of my work items</li>
   <li>Someone comments on my help request. </li>
  </ul>The changes you make to the notifications options take effect immediately.<br>The notifications you have enabled are delivered in the Workfront Slack channel. When you disable notifications here, they are only disabled for Slack, and not for the Workfront interface. You continue to receive them in the Workfront notifications bubble in the upper right of the interface.&nbsp;</li> 
</ol>

## Manage Workfront notifications from Slack

You can receive and respond to Workfront notifications from Slack.&nbsp;

You can disable email notifications for notifications that you enable in Slack, to ensure that you do not receive duplicate notifications.  
For information about configuring your email notifications, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Enabling or disabling Workfront notifications in Slack does not affect the notifications you receive inside the Workfront interface.  
Notifications inside the Workfront interface cannot be disabled.&nbsp;

To manage your Workfront notifications for Slack:&nbsp;

<ol> 
 <li value="1">Log in to Slack.</li> 
 <li value="2">Log in to Workfront from Slack.<br>For information about logging in to Workfront from Slack, see the "Logging in to Workfront from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md" class="MCXref xref">Access Adobe Workfront from Slack</a>.</li> 
 <li value="3">Ensure that your Workfront notifications for Slack are enabled.<br>For more information about which Workfront notifications can be configured to also be sent to Slack, see <a href="#configuring-notifications-for-slack" class="MCXref xref">Configure Workfront notifications for Slack</a>.</li> 
 <li value="4">Go to the <span class="bold">Workfront</span> channel to find your Workfront notifications.&nbsp;</li> 
 <li value="5"> (Conditional and optional) Do any of the following:&nbsp; 
  <ul>
   <li>Click <span class="bold">Work on it</span> to accept to work on a task.<br><!--
    --><br></li>
   <li>(Conditional and optional) Click <span class="bold">Reply in Workfront</span> to reply to a comment, type your reply, and click <span class="bold">Reply</span>.<br><img src="assets/slack-tagged-in-a-comment-notification.png" alt="slack_tagged_in_a_comment_notification.png"><br></li>
   <li>(Conditional and optional) Click <span class="bold">Approve</span> or <span class="bold">Reject</span> to approve or reject a task, issue, or project that are pending your approval.<br><img src="assets/slack-approve-task-notification-350x105.png" alt="slack_approve_task_notification.png" style="width: 350;height: 105;"><br></li>
   <li>(Conditional and optional) Click <span class="bold">Approve</span>, <span class="bold">Changes</span>, or <span class="bold">Reject</span>, to approve, approve with changes, or reject a document.<br><img src="assets/slack-approve-a-document-350x362.png" alt="slack_approve_a_document.png" style="width: 350;height: 362;"><br>You can also mouse over the thumbnail of the document and click the magnifying glass icon to view a larger preview of the document, before you approve it.<br>Only the approved Slack <a href="https://api.slack.com/types/file">file types</a> can be previewed.&nbsp;</li>
   <li>(Conditional and optional) Click <span class="bold">Grant</span> or <span class="bold">Ignore</span> to grant or ignore the request for more access from another user.<br><img src="assets/slack-access-approvals-list-350x213.png" style="width: 350;height: 213;"><br>You receive a confirmation that your action has been completed in Workfront, for every decision you make within your notifications.&nbsp;&nbsp;</li>
  </ul></li> 
</ol>

