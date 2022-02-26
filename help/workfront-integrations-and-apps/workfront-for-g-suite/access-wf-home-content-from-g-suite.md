---
filename: access-wf-home-content-from-g-suite
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Access Adobe Workfront Home content from G Suite
description: You can access your Adobe Workfront Home content, including all tasks, issues, approvals, and access requests assigned to you, without leaving G Suite.
---

# Access *Adobe Workfront* Home content from G Suite

You can access your *Adobe Workfront* Home content, including all tasks, issues, approvals, and access requests assigned to you, without leaving G Suite.

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

Before you can access Home content from G Suite, you must

* Install *Workfront* for G suite  
  For instructions, see [Install Adobe Workfront for G Suite](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Access *Workfront* Home from G Suite

<ol> 
 <li value="1">Make sure you are logged in to <em>Workfront</em>.</li> 
 <li value="2">If the <em>Workfront for G Suite</em> panel is not displayed, click the&nbsp;<em>Workfront</em> icon <img src="assets/wf-lion-icon.png"> in the G Suite add-ons sidebar at the far-right of the page. </li> 
 <li value="3"> <p>If you see a left arrow at the top of Workfront for G&nbsp;Suite, click the arrow to go to the Home area. </p> <p> <img src="assets/left-arrow-to-home.png" class="NotAThumbnail"> </p> </li> 
 <li value="4"> <p>In the <span class="bold">Sort by</span> area, click the expand arrow <img src="assets/dropdown-arrow.png">, then click an option to specify how you want to group your work items so you can find the one you want.</p> <p> <img src="assets/sort-by-area.png"> </p> <p>When you sort by <span class="bold">Commit date</span> or <span class="bold">Planned completion</span> date, the oldest work items are at the top.</p> <p>When you sort by <span class="bold">Project</span>, work items appear in the order of their parent projects, listed alphabetically from A to Z. Work items without a parent project display under <span class="bold">No Project</span>.</p> </li> 
 <li value="5"> <p>Click the expand arrow <img src="assets/dropdown-arrow.png"> for the grouping you want to view.</p> <p>The number of items contained within each group displays in parenthesis. When you click the expand arrow, all the work items in the group display.</p> <p>Work items appear as follows:</p> 
  <ul> 
   <li> <img src="assets/task-icon.png"> <span class="bold"> Tasks</span> display the parent project name, task name, and planned completion date.</li> 
   <li> <img src="assets/issue-icon.png"> <span class="bold"> Issues</span> display the parent project name, issue name, and planned completion date.</li> 
   <li><span class="bold"><img src="assets/document-icon.png"> Approvals</span> display the requester's name, document name, and submission date.</li> 
   <li><span class="bold">Access requests</span> display the requester's name, object name, and submission date. The icon for the object type displays on the left.</li> 
  </ul> </li> 
 <li value="6"> <p>Click anywhere on a work item to see its details, updates, and documents.</p> </li> 
</ol>

