---
filename: configure-default-proofing-roles
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configure default proofing roles
description: As an Adobe Workfront administrator, you can configure the default proofing roles for users and guest users who access proofs created in Workfront. Any person adding users to a proof can adjust these roles for them.
---

# Configure default *proofing* roles

As an *Adobe Workfront administrator*, you can configure the default *proofing* roles for users and guest users who access *proofs* created in *Workfront*. Any person adding users to a *proof* can adjust these roles for them.

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
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Configure default *proofing* roles

<ol> 
 <li value="1"><![CDATA[
]]>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">In the left panel, click <span class="bold">Proofs</span> > <span class="bold">Proof roles</span>.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">In the left panel, click <span class="bold">Proofs</span> > <span class="bold">Proof roles</span>.</li> 
 <li value="3">Click <span class="bold">Review and Approval</span> near the bottom of the list that appears on the left. </li> 
 <li value="4"> <p>In the <span class="bold">Roles for designated recipients of a document <em>proof</em></span> section, select the default role for users and guest users who are added to a <em>proof</em>'s workflow.</p> <p>See <a href="#rights" class="MCXref xref">Rights associated with proofing roles</a> below for a list of each <em>proofing</em> role and the rights associated with it.</p> <note type="note">  
   <ul> 
    <li>This setting applies only to users who are created in the <em>Workfront</em> system after the role is set; not to existing users.</li> 
    <li>The person adding users to the <em>proof</em> can adjust this role, as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add" class="MCXref xref">Add users to a proof</a> in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md" class="MCXref xref">Share a proof within Adobe Workfront</a>.</li> 
   </ul> 
  </note> </li> 
 <li value="5"> <p>In the <span class="bold">Roles for non-recipients that open a document <em>proof</em></span> section, select the default role for users and guest users who can access a <em>proof</em>, but are not added to the <em>proof</em>'s workflow.</p> <p>This situation occurs when users and guests have access to a document for which a <em>proof</em> has been created: even if they have not been added to the <em>proof</em>'s workflow, they can open the <em>proof</em>.</p> 
  <div class="examples" data-mc-autonum="<b>Examples: </b>"> <span class="autonumber"><span><b>Examples: </b></span></span>Here are examples of how you could use this setting: 
   <ul> 
    <li>You select <span class="bold">Read only</span> to limit all <em>proof</em> activity such as adding comments and making decisions to those who have been asked to do it.</li> 
    <li>You select <span class="bold">Reviewer</span> because you want any member of the team to be able to add markups and comments on a <em>proof</em>.</li> 
   </ul> 
  </div> </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

## Rights associated with *proofing* roles

The following table shows each role and the rights associated with it:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>&nbsp;</p> </th> 
   <th> <p><span class="bold">View a <em>proof</em></span> </p> </th> 
   <th> <p><span class="bold">Add markups</span> </p> </th> 
   <th> <p><span class="bold">Add comments</span> </p> </th> 
   <th> <p><span class="bold">Edit own comments if there are no replies</span> </p> </th> 
   <th> <p><span class="bold">Make a decision</span> </p> </th> 
   <th> <p><span class="bold">Delete comments made by others</span> </p> </th> 
   <th>Resolve comments</th> 
   <th>Apply Actions to Comments</th> 
   <th> <p><span class="bold">Edit the <em>proof</em></span> </p> </th> 
   <th>Share the <em>proof</em> with others</th> 
   <th>Create new version</th> 
   <th> <p><span class="bold">View approval requests in the Home area</span> </p> </th> 
   <th>Add new reviewers</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Read Only</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Reviewer</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Approver</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td> <p>✓</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Reviewer &amp; Approver</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td> <p>✓</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Author</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Moderator</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><span class="bold">✓</span> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p>&nbsp;</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Users on new Workfront plans can grant author or moderator roles to any users in the system. Users on legacy plans can grant author or moderator roles to any user with a proof license in the system.

