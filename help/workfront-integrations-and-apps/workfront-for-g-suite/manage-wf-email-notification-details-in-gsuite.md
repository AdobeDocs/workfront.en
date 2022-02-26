---
filename: manage-wf-email-notification-details-in-gsuite
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Manage Adobe Workfront notification details from G Suite
description: In G Suite, when you open a notification email Adobe Workfront has sent, you can view the associated work item details and respond without leaving your Inbox. If actions are available, such as approving a request, you can perform those actions directly from Workfront for G Suite.
---

# Manage *Adobe Workfront* notification details from G Suite

In G&nbsp;Suite, when you open a notification email *Adobe Workfront* has sent, you can view the associated work item details and respond without leaving your Inbox. If actions are available, such as approving a request, you can perform those actions directly from *Workfront for G Suite*.

>[!NOTE]
>
>*Workfront* for G&nbsp;Suite supports almost every type of email notification you can receive from *Workfront* (about 120 different types). Daily digest emails sent from *Workfront* do not appear in *Workfront* for G&nbsp;Suite. For information about the *Workfront* email notification types, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Work, Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: Edit access to Documents
      </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: Edit access to Documents
     </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: View access or higher on Documents
      </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[Insert permissions needed and specify the object] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: View access or higher on Documents
     </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

Before you can manage notification details from G Suite, you must

* Install *Workfront* for G suite  
  For instructions, see [Install Adobe Workfront for G Suite](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Manage *Adobe Workfront* notification details from G Suite

<ol> 
 <li value="1">If the <em>Workfront for G Suite</em> panel is not displayed, click the&nbsp;<em>Workfront</em> icon <img src="assets/wf-lion-icon.png"> in the G Suite add-ons sidebar at the far-right of the page. </li> 
 <li value="2">In G&nbsp;Suite, open a <em>Workfront</em> notification email.</li> 
 <li value="3">Click <span class="bold">View all updates</span> if it is displayed near the top of the panel.</li> 
 <li value="4"> <p>Click <span class="bold">Details</span>.</p> </li> 
 <li value="5"> <p>Click any available options.</p> <p>The options that might display relate to the type of email notification you have opened. For example, if it's an email notification asking you to approve a task, you see <span class="bold">Approve</span> and <span class="bold">Reject</span> instead of options such as <span class="bold">Work on It</span> or <span class="bold">Done</span>:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Type of email notification</th> 
     <th>Action</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td>Task or issue</td> 
     <td><span class="bold">Approve</span> it, <span class="bold">Reject</span> it, <span class="bold">Grant</span> access to it, <span class="bold">Ignore</span> a request for access to it, <span class="bold">Work on it</span>, or click an option to indicate that you are <span class="bold">Done</span> with it</td> 
    </tr> 
    <tr> 
     <td>Project</td> 
     <td><span class="bold">Approve</span> it, <span class="bold">Reject</span> it, <span class="bold">Grant</span> access to it, or <span class="bold">Ignore</span> a request for access to it</td> 
    </tr> 
    <tr> 
     <td>Document</td> 
     <td><span class="bold">Approve</span> it, <span class="bold">Reject</span> it, <span class="bold">Grant</span> access to it, or <span class="bold">Ignore</span> a request for access to it</td> 
    </tr> 
    <tr> 
     <td>Update </td> 
     <td> <p>View any part of the entire list of updates for the item so that you have the context you need to <span class="bold">Post</span> a new update or a <span class="bold">Reply</span>. You can click <span class="bold">Notify</span> to alert particular users about your reply. </p> <p>For more information, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Reply to a Adobe Workfront update notification from G Suite</a>.</p> </td> 
    </tr> 
    <tr> 
     <td>Approval request</td> 
     <td><span class="bold">Approve</span> or <span class="bold">Reject</span> it (you can change your mind by clicking the other option), download it, view its owner, or view its reference number</td> 
    </tr> 
    <tr> 
     <td>A change in a project's status</td> 
     <td> View all the current information about the project, including any custom forms. </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

