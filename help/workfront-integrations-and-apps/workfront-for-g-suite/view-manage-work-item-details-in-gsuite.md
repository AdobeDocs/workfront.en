---
filename: view-manage-work-item-details-in-gsuite
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: View and manage Adobe Workfront object details from G Suite
description: You can view and manage the details of a work item without leaving G Suite. For example, you can read a task's description, view its parent object, change its status, and mark it as complete, all within Adobe Workfront for G Suite.
---

# View and manage *Adobe Workfront* object details from G Suite

You can view and manage the details of a work item without leaving G Suite. For example, you can read a task's description, view its parent object, change its status, and mark it as complete, all within *Adobe Workfront* for G&nbsp;Suite.

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

Before you can view and manage work item details in G Suite, you must

* Install *Workfront* for G suite  
  For instructions, see [Install Adobe Workfront for G Suite](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## View and manage work item details in G Suite

<ol> 
 <li value="1">If the <em>Workfront for G Suite</em> panel is not displayed, click the&nbsp;<em>Workfront</em> icon <img src="assets/wf-lion-icon.png"> in the G Suite add-ons sidebar at the far-right of the page. </li> 
 <li value="2"> <p>Go to the <em>Workfront</em> task or issue within G Suite, as described in <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md" class="MCXref xref">Access Adobe Workfront Home content from G Suite</a>.</p> <p>When you select a task or issue, the <span class="bold">Details</span> tab is open. The area above the <span class="bold">Details</span> tab displays the name of the parent object, the name of the task or issue, and the Due date (if it's a task) or Priority date (if it's an issue).</p> <p> <img src="assets/details-tab.png"> </p> <p>You can do various tasks on this tab without leaving G Suite, including the following: </p> 
  <ul> 
   <li> <p>View the object's <span class="bold">Description</span> and other details, such as the users assigned to the object, the <span class="bold">Priority</span>, the requester, the <span class="bold">Planned completion date</span>, and any custom fields and forms attached to the object. </p> <p>Custom forms display only fields where information has been added.</p> </li> 
   <li> <p>Click the <span class="bold">Parent project</span> area to view the details of the parent object. </p> <note type="tip">
     This can be helpful when you have tasks and issues with the same name and you need to differentiate them.
    </note> </li> 
   <li>Accept work assigned to you by clicking <span class="bold">Work on it</span>.</li> 
   <li> <p>Edit various options, such as <span class="bold">Done</span> option, the <span class="bold">Status</span>, and the <span class="bold">Percent complete</span>. </p> <p>Under <span class="bold">Percent complete</span>, type numbers and (optionally) the percentage sign % to indicate your progress on an item. </p> </li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="bold">Log time</span> on a work item.</li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="bold">Log time</span> on a work item.</li> 
   <li>View information about an approval request, including the owner, size, and any attachments. </li> 
   <li><span class="bold">Approve</span> or <span class="bold">Reject</span> approval requests and documents.</li> 
   <li><span class="bold">Grant</span> or <span class="bold">Ignore</span> access requests.</li> 
  </ul> </li> 
 <li value="3">(Optional) Click <span class="bold">View in Workfront</span> to go to the current work item in <em>Workfront</em>.</li> 
</ol>

`<li>For information about using the Updates tab in <em>Workfront for G Suite</em>, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md" class="MCXref xref">Update a Adobe Workfront object from G Suite</a>.</li>` `<li>For information about using the Documents tab in <em>Workfront for G Suite</em>, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md" class="MCXref xref">View and manage documents from G&nbsp;Suite</a>.</li>`  