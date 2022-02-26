---
filename: turn-issue-status-from-awf-to-inp-automatically
product-area: projects
navigation-topic: manage-issues
title: Automatically update issue statuses from Awaiting Feedback to In Progress
description: When the Primary Contact of an issue makes an update to the issue by either updating a field (including a custom field) or adding a comment, the issue status updates to In Progress automatically.
---

# Automatically update issue statuses from Awaiting Feedback to In Progress

When the Primary Contact of an issue makes an update to the issue by either updating a field (including a custom field) or adding a comment, the issue status updates to In Progress automatically.

In order for this automatic status change to occur, the following is required:

<ul> 
 <li> <p>The issue must be entered through a request queue.</p> <p>For information about creating request queues, see the <a href="../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md" class="MCXref xref" xrefformat="{para}">Create and manage Request Queues</a> section. For information about creating requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref" xrefformat="{para}">Create and submit Adobe Workfront requests</a>.</p> </li> 
 <li> <p>The Queue Details in the request queue must have these settings:<br><span class="bold">When someone makes a request, automatically grant</span> is set to <span class="bold">Contribute Access</span><br><span class="bold">Change Status</span> is selected under Advanced Settings</p> <p> <img src="assets/queuedetails-contributeaccess-changestatus.png" alt="Queue Details give Contribute Access and Change Status is selected."> </p> <p>For more information about Queue Details, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref" xrefformat="{para}">Create a Request Queue</a>.</p> </li> 
 <li>The issue must be in Awaiting Feedback status.</li> 
 <li> <p>There must be an Awaiting Feedback (AWF) status available for issues at the system level. </p> <p>For more information about system-level statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref" xrefformat="{para}">Create or edit a status</a>.</p> </li> 
</ul>

