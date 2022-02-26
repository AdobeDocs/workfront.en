---
filename: manage-your-work-and-approvals-from-slack
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Manage your work and approvals from Slack
description: After you have installed Adobe Workfront for Slack, you can do the following:
---

# Manage your work and approvals from Slack

After you have installed *Adobe Workfront* for Slack, you can do the following:

* Access lists of your Home items from Slack
* Review and accept to work on tasks and issues from Slack
* Review and make decisions on approvals from Slack

For more information about configuring *Workfront* with Slack, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
    <td> <p>Plan</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.\

## Prerequisites

Before you can manage your work and approvals from Slack, you must

* Configure *Workfront* for Slack  
  For instructions on configuring *Workfront* for Slack, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Manage your work from Slack

<ol> 
 <li value="1"> Log in to your Slack instance and log in to <em>Workfront</em> from Slack.<br>For more information about logging in to <em>Workfront</em> from Slack, see the "Logging In to <em>Workfront</em> from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md" class="MCXref xref">Access Adobe Workfront from Slack</a>.</li> 
 <li value="2"> <p>From any channel, start typing the following command in the message field:&nbsp;<br><code>/workfront home</code></p> <note type="note"> 
   <ul> 
    <li>Commands are case sensitive. </li> 
    <li>You can start your command with /<code>wf</code> instead of <code>/workfront</code>.</li> 
   </ul> 
  </note> <p>The buttons from which you can access lists of your tasks, issues, and approvals display. Clicking one of the buttons displays the first 20 items of each list in Slack.<br><img src="assets/slack-home-buttons-350x80.png" style="width: 350;height: 80;">&nbsp;<br></p> </li> 
 <li value="3"> <p>(Optional) Click <span class="bold">Tasks</span>&nbsp;to display all your tasks.</p> <p>For more information about managing tasks in Slack, see <a href="#managing-working-on-list">Managing Your Tasks from Slack</a>.</p> </li> 
 <li value="4"> <p>(Optional) Click <span class="bold">Issues</span> to display all your issues.</p> <p>For more information about managing issues in Slack, see <a href="#manahing-work-requests">Managing Your Issues from Slack</a>.<br></p> </li> 
 <li value="5">(Optional) Click <span class="bold">Approvals</span> to display all the approvals waiting for your decision.<br>For more information about managing your approvals in Slack, see <a href="#managing-approvals" class="MCXref xref">Manage your approvals from Slack</a>.</li> 
</ol>

## Manage your tasks from Slack

<ol> 
 <li value="1"> Log in to your Slack instance and log in to <em>Workfront</em> from Slack.<br>For information about logging in to <em>Workfront</em> from Slack, see the "Logging In to <em>Workfront</em> from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md" class="MCXref xref">Access Adobe Workfront from Slack</a>.</li> 
 <li value="2"> <p>From any channel, start typing either of the following commands in the message field:&nbsp;<br><em><code>/workfront home</code>,&nbsp;</em>then click <span class="bold">Tasks</span></p> <p>Or</p> <p><code>/workfront tasks</code> </p> <note type="note"> 
   <ul> 
    <li>Commands are case sensitive.</li> 
    <li>You can start your command with '/wf' instead of '/workfront.'</li> 
   </ul> 
  </note> <p>The first 20 tasks on your list display.<br><img src="assets/slack-two-tasks-350x286.png" style="width: 350;height: 286;"></p> </li> 
 <li value="3"> <p>Click <span class="bold">+<remaining number> more</span>&nbsp;to display additional tasks.</p> </li> 
 <li value="4"> <p>Consider reviewing the following information about your work items:</p> 
  <ul> 
   <li><span class="bold">Name</span> </li> 
   <li><span class="bold">Project Name</span> or <span class="bold">Parent Object Name</span></li> 
   <li><span class="bold">Planned Completion Date</span> of the work item.</li> 
   <li><span class="bold">Assigned By Name</span>: this is the name of the user who assigned the task to you.</li> 
   <li><span class="bold">Status</span> </li> 
  </ul> </li> 
 <li value="5"> <p>(Optional) Click the name of an item to open it in <em>Workfront</em> in a separate browser tab.</p> </li> 
 <li value="6"> <p>(Optional) In the <span class="bold">Status</span> field, select a new Status.</p> </li> 
 <li value="7"> <p>(Optional) Click <span class="bold">Log Time</span>, then select an <span class="bold">Hour Type</span> and an hour amount to log time on the item.</p> <note type="note"> 
   <ul> 
    <li>You can only log hours in increments of a full or half hour, up to 12 hours and 30 minutes.</li> 
    <li>The hours you log have an Entry Date of today. You cannot log time for a passed or future date from Slack.</li> 
   </ul> 
  </note> <p>You receive a confirmation that the time has been logged.</p> </li> 
 <li value="8"> <p>(Optional) Click <span class="bold">Work on it</span> to accept to work on a task. The Work on it button disappears.</p> </li> 
</ol>

## Manage your issues from Slack

<ol> 
 <li value="1"> Log in to your Slack instance and log in to <em>Workfront</em> from Slack.<br>For more information about logging in to <em>Workfront</em> from Slack, see the <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront">Logging In to <em>Workfront</em> from Slack</a> section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md" class="MCXref xref">Access Adobe Workfront from Slack</a>.</li> 
 <li value="2">From any channel, start typing either of the following commands in the message field:&nbsp;<br><em><code>/workfront home</code>,&nbsp;</em>then click <span class="bold">Issues</span> <br>Or<br><code>/workfront issues</code><br><note type="note">
   Commands are case sensitive. You can start your command with 
   <code>/wf</code> instead of 
   <code>/workfront</code>.
   <br>
  </note>The first 20 issues in your list display.<br><img src="assets/slack-two-issues-350x323.png" style="width: 350;height: 323;"><br></li> 
 <li value="3">Click <span class="bold">+ remaining <number> more</span> to display additional items.</li> 
 <li value="4">Consider reviewing the following information about your work items:<br>
  <ul>
   <li><span class="bold">Name</span></li>
   <li><span class="bold">Project</span> Name or Parent Object Name</li>
   <li><span class="bold">Due on</span> Date: This is the Planned Completion Date of the work item.</li>
   <li><span class="bold">Requested by</span> Name: This is the Primary Contact (for issues) or the user who made the assignment (for tasks).&nbsp;</li>
  </ul></li> 
 <li value="5">(Optional) Click the name of the issue to open it in <em>Workfront</em> in a separate browser tab.</li> 
 <li value="6"> <p>(Optional) Click <span class="bold">Work on it</span> to start working on issues you have not accepted yet.</p> <p>The Work on it button disappears.</p> </li> 
</ol>

## Manage your approvals from Slack

<ol> 
 <li value="1"> Log in to your Slack instance and log in to <em>Workfront</em> from Slack.<br>For more information about logging in to <em>Workfront</em> from Slack, see the "Logging In to <em>Workfront</em> from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md" class="MCXref xref">Access Adobe Workfront from Slack</a>.</li> 
 <li value="2"> <p>From any channel, start typing either of the following commands in the message field:&nbsp;<br><em><code>/workfront home</code>,&nbsp;</em>then click <span class="bold">Approvals</span>&nbsp;<br>Or<br><code>/workfront approvals</code></p> <note type="note"> 
   <ul> 
    <li>Commands are case sensitive. </li> 
    <li>You can start your command with <code>/wf</code> instead of <code>/workfront</code>. </li> 
   </ul> 
  </note> <p>The first 20 items on your <span class="bold">Approvals</span> list display. Additional information about the items also displays, like the name of the user who requested it or the name of the project the item belongs to.&nbsp;</p> </li> 
 <li value="3">Click <span class="bold">+ remaining <number> more</span> to display additional items.<br><draft-comment>
   <img src="assets/slack-project-approvals-list-350x106.png" alt="slack_project_approvals_list.png" style="width: 350;height: 106;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
  </draft-comment><img src="assets/slack-project-approvals-list-350x106.png" alt="slack_project_approvals_list.png" style="width: 350;height: 106;" data-mc-conditions="QuicksilverOrClassic.Draft mode"><br><img src="assets/slack-access-approvals-list-350x213.png" alt="slack_access_approvals_list.png" style="width: 350;height: 213;"><br><img src="assets/slack-approve-a-document-350x362.png" style="width: 350;height: 362;"><img src="assets/slack-approve-task-notification-350x105.png" style="width: 350;height: 105;"></li> 
 <li value="4">Consider managing approvals for the following objects:&nbsp;<br>
  <ul>
   <li><span class="bold">Projects</span><br>Click <span class="bold">Approve</span> or <span class="bold">Reject</span> to accept or reject the status change of a project.</li>
   <li><span class="bold">Tasks</span><br>Click <span class="bold">Approve</span> or <span class="bold">Reject</span> to accept or reject the status change of a task.</li>
   <li><span class="bold">Issues</span><br>Click <span class="bold">Approve</span> or <span class="bold">Reject</span> to accept or reject the status change of an issue.</li>
   <li><span class="bold">Documents</span><br>Click <span class="bold">Approve</span> to approve a document, <span class="bold">Reject</span> to reject it, or <span class="bold">Changes</span> to indicate that you approve it, but that the document needs additional changes.<br>(Optional) Mouse over the document thumbnail to click the magnifying glass and preview the document.&nbsp;</li>
   <li><span class="bold">Proofs<br></span>Click the <em>proof</em> name to open it in <em>Workfront</em> in a separate tab and manage the approval.&nbsp;</li>
   <li><span class="bold">Access Requests</span><br>Click <span class="bold">Grant Access</span> to give enhanced permissions to the requested object, or <span class="bold">Ignore</span> to ignore the request for more access.</li>
  </ul></li> 
 <li value="5">(Optional) Click the name of the object submitted for approval to open it in <em>Workfront</em> in a new browser tab.&nbsp;</li> 
</ol>

