---
content-type: reference
navigation-topic: notifications
title: 'Notifications: Unified approvals'
description: The following notifications alert you about approval activities for the Unified Approvals experience. For information about configuring which notifications you receive, see Modify your own email notifications.
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Notifications: Unified approvals

{{highlighted-preview}}

Use the following notifications to stay informed about activity for Unified review and approvals. For information about configuring which email notifications you receive, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>These notifications are available only as instant notifications and are not available in a daily digest.
>
>In the Fields included column, an asterisk (*) indicates a field that appears only when it applies.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>Fields included</th> 
   <th>Default status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Approval finished – Approved</strong> </p> <p>A document approval finishes with a final decision of Approved.</p> <p>The subject of the instant notification email is: <em>Final decision: (Document) is approved</em></p> </td> 
   <td> Final decision<br>Document<br>Approval requested date<br>Due date<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approval finished – Approved with changes</strong> </p> <p>A document approval finishes with a final decision of Approved with changes.</p> <p>The subject of the instant notification email is: <em>Final decision: (Document) is approved with changes</em></p> </td> 
   <td> Final decision<br>Document<br>Approval requested date<br>Due date<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approval finished – Needs work</strong> </p> <p>A document approval finishes with a final decision of Needs work.</p> <p>The subject of the instant notification email is: <em>Final decision: (Document) needs work</em></p> </td> 
   <td> Final decision<br>Document<br>Approval requested date<br>Due date<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Deadline approaching</strong> </p> <p>A document approval you are part of is approaching its deadline.</p> <p>The subject of the instant notification email is: <em>Approval deadline approaching for (Document)</em></p> </td> 
   <td> Requester<br>Your role<br>Team<br>Document preview*<br>Custom message*<br>Approval requested date<br>Due date<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Deadline passed</strong> </p> <p>A document approval you are part of passes its deadline without a final decision.</p> <p>The subject of the instant notification email is: <em>Approval deadline passed for (Document)</em></p> </td> 
   <td> Fixed headline<br>Approval requested date<br>Due date<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, All recipients (no Project) </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Review completed</strong> </p> <p>A reviewer completes their review on a document approval.</p> <p>The subject of the instant notification email is: <em>(Document) has been reviewed</em></p> </td> 
   <td> Reviewer<br>Document<br>Document preview*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Video approval limit approaching (80%)</strong> </p> <p>A video approval reaches 80% of its plan's video approval limit.</p> <p>The subject of the instant notification email is: <em>You're close to your annual video approval request limit in Workfront</em></p> </td> 
   <td> Headline and body text<br>Video approvals requested (current usage)<br>Cap total (the limit)<br>Other recipients<br>"View in Workfront" button<br>"Upgrade to FIO enterprise" button </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Video approval limit reached</strong> </p> <p>A video approval reaches its plan's video approval limit.</p> <p>The subject of the instant notification email is: <em>You've reached your annual video approval request limit in Workfront</em></p> </td> 
   <td> Headline and body text<br>Video approvals requested (current usage)<br>Cap total (the limit)<br>Other recipients<br>"View in Workfront" button<br>"Upgrade to FIO enterprise" button </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decision made – Approved</strong> </p> <p>An approver makes a decision of Approved on a document approval.</p> <p>The subject of the instant notification email is: <em>(Document) approved by (Name)</em></p> </td> 
   <td> Decision maker<br>Decision<br>Document and version<br>Document preview*<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decision made – Approved with changes</strong> </p> <p>An approver makes a decision of Approved with changes on a document approval.</p> <p>The subject of the instant notification email is: <em>(Document) approved with changes by (Name)</em></p> </td> 
   <td> Decision maker<br>Decision<br>Document and version<br>Document preview*<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decision made – Needs work</strong> </p> <p>An approver makes a decision of Needs work on a document approval.</p> <p>The subject of the instant notification email is: <em>(Document) needs work by (Name)</em></p> </td> 
   <td> Decision maker<br>Decision<br>Document and version<br>Document preview*<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documents added to or removed from a grouped approval</strong> </p> <p>Documents are added to or removed from a grouped document approval you are part of.</p> <p>The subject of the instant notification email is: <em>A document was added to or removed from an approval you are part of</em></p> </td> 
   <td> <p><strong>Added:</strong> Requester, Group name, Thumbnail preview, Custom message*, Dates, "Go to review" button, Details block: Group name, Number of assets, Project*, All recipients</p> <p><strong>Removed:</strong> Requester, Group name, Thumbnail preview (no button or Details block)</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>All reviews completed</strong> </p> <p>Every reviewer completes their review on a document approval.</p> <p>The subject of the instant notification email is: <em>All reviews are complete on (Document)</em></p> </td> 
   <td> Document<br>Approval requested date<br>Due date<br>Custom message*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Reminder - 24 hours</strong> </p> <p>You have 24 hours left to review and approve the document.</p> <p>The subject of the instant notification email is: <em>Reminder: Your approval is needed on (Document)</em></p> </td> 
   <td> Requester<br>Your role<br>Team<br>Document preview*<br>Custom message*<br>Approval requested date<br>Due date<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Reminder - 72 hours</strong> </p> <p>You have 72 hours left to review and approve the document.</p> <p>The subject of the instant notification email is: <em>Reminder: Your approval is needed on (Document)</em></p> </td> 
   <td> Requester<br>Your role<br>Team<br>Document preview*<br>Custom message*<br>Approval requested date<br>Due date<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Added as approver or reviewer</strong> </p> <p>You are added as an approver or reviewer on a document approval.</p> <p>The subject of the instant notification email is: <em>Your approval is needed on (Document)</em></p> </td> 
   <td> Requester<br>Your role<br>Team<br>Document preview*<br>Custom message*<br>Approval requested date<br>Due date<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Removed as approver or reviewer</strong> </p> <p>You are removed as an approver or reviewer from a document approval.</p> <p>The subject of the instant notification email is: <em>Your approval is no longer needed on (Document)</em></p> </td> 
   <td> Requester<br>Document and version<br>Role<br>Team<br>Document preview*<br>Custom message* (no button or Details block) </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Role changed</strong> </p> <p>Your approver or reviewer role changes on a document approval.</p> <p>The subject of the instant notification email is: <em>Your role on (Document) has changed</em></p> </td> 
   <td> Requester<br>Document and version<br>Direction of the role change<br>Document preview*<br>"Go to review" button<br>Details block: Document name, Document details, Stage*, Project*, All recipients </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
