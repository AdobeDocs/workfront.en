---
filename: enable-email-issues-into-projects
product-area: requests
navigation-topic: create-requests
title: Enable users to email an issue into a Request Queue project
description: You can configure a project to allow users to add issues to the project via email. You can allow for issues to be emailed into a project only if the project is designated as a Request Queue. For more information about creating a Request Queue project, see Create a Request Queue.
---

# Enable users to email an issue into a Request Queue project

You can configure a project to allow users to add issues to the project via email. You can allow for issues to be emailed into a project only if the project is designated as a Request Queue. For more information about creating a Request Queue project, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Request</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.<br></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

The following prerequisites are required to configure a project to allow users to add issues to the project via email.

These conditions must be met, before enabling this feature:

<ul> 
 <li> Users who are emailing issues to this account must be active users with a license for <em>Workfront</em>.<br></li> <note type="note">
   External Users cannot email issues to a request queue because they do not have access to create issues.
 </note> 
 <li> Users who are emailing issues to this account must have Add Issue permissions on the project. </li> 
 <li> The emails coming from the email address associated with an active <em>Workfront</em> user are the only emails allowed to send issues to the project. </li> 
 <li> The project is set up as a Request Queue. </li> 
 <li> The email account associated with the project is not linked to a <em>Workfront</em> user account. </li> 
</ul>

## Configure the project in *Workfront*

Keep the following in mind when enabling email queue settings:

* Workfront allows one unique email per request queue across all clusters. If you choose to disable your request queue, you'll retain the email address you created as long as it is still in the Intake Email Address box. If you choose to discontinue use of the intake email, you must delete it from the Intake Email Field so it can be available for future use.

<ol> 
 <li value="1">Go to the project that you want to enable to receive issues via email.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Queue Details</span> in the left panel. You might need to click <span class="bold">Show More</span> first.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Queue Details</span> in the left panel. You might need to click <span class="bold">Show More</span> first.</p> </li> 
 <li value="3">In the <span class="bold">Queue Type</span> area, select <span class="bold">Publish as Help Request Queue</span>.</li> 
 <li value="4">Scroll down to the <span class="bold">Email Queue Settings</span> area, then select <span class="bold">Enable Request intake via email</span>.</li> 
 <li value="5"> <p>Enter the beginning of the email address in the <span class="bold">Intake Email Address</span> box. You must create a unique email address. We recommend using your company name as part of your intake email address.</p> 
  <div class="warning" data-mc-autonum="<b>Warning: </b>">
   <span class="autonumber"><span><b>Warning: </b></span></span> 
   <ul class="warning"> 
    <li>This email address cannot be recovered from the recycle bin if the project containing the request queue is deleted.</li> 
    <li>Because this email address must be unique, it may not be available in the future if deleted.</li> 
    <li>Emails forwarded to this email address are not added as issues to the project in&nbsp;<em>Workfront</em>. Only emails created from this email address are added as issues.</li> 
   </ul> 
  </div> </li> 
 <li value="6">(Optional) Select the <span class="bold">Forward all issues that fail to submit via email</span>, then enter a forwarding email address in the box below. This email address receives information about emails that failed to submit to the project.</li> 
 <li value="7"> <p>Click <span class="bold">Save</span>. Now, when users with an active <em>Workfront</em> account send an email to this email address, an issue is created in the <em>Workfront</em> project.</p> <note type="note">
    Users must have access to create issues in the project in order to submit via email. You can grant this access in the Sharing dialog box under Advanced Settings.
   <br>
   <br>External Users cannot email issues to a request queue because they do not have access to create issues.
  </note> </li> 
</ol>

## Receive the issue in *Workfront*

When a *Workfront* user sends an email to *Workfront*, the following things happen:

* The Subject line of the email becomes the Issue Name.
* The body of the email becomes the Description of the Issue.
* If there are any documents attached to the email, those documents are attached to the issue in *Workfront*.
* The user who is sending the email becomes the Primary Contact of the new issue in *Workfront*.
* The body text of the email cannot exceed 4,000 characters.
* Email attachments cannot exceed 7 MB total.

