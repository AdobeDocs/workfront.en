---
filename: delete-a-user
title: Delete a user
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Delete users
description: The highlighted information on this page refers to functionality available only in the new Workfront experience beta.
---

# Delete users

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

When a user leaves your organization, can remove that user from *Adobe Workfront*.

>[!IMPORTANT]
>
>* Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see [Deactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b><img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a <em>group administrator</em> of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Deleting vs. deactivating a user

Deactivating a user causes the following things to happen:

<ul> 
 <li>Removes the user's licenses to both <em>Workfront</em> and <em>Workfront Proof</em> if the <em>Workfront Proof</em> component is associated with your <em>Workfront</em> account. For more information about <em>Workfront Proof</em>, see <a href="../../../workfront-proof/workfront-proof.md" class="MCXref xref">Workfront Proof</a>.</li> 
 <li>The user can no longer be assigned work.</li> 
 <li>The user can no longer be added to updates.</li> 
 <li>The user can no longer be added to teams or groups.</li> 
 <li>Objects can no longer be shared with the user.</li> 
 <li>Their association with the following objects remains intact:</li> 
 <ul> 
  <li>Tasks, issues, projects, portfolios</li> 
  <li> <p>Dashboards</p> <note type="note">
    If you deactivate a user and can no longer view the reports or dashboards associated with a user, you may need to update the 
    <span class="bold">Run this report with the Access Rights of:</span> field.
    <br>To learn more, see the 
    <a href="../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why" class="MCXref xref">Why can't I access a report owned by a deactivated user?</a> section of the 
    <a href="../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md" class="MCXref xref">Reports FAQs</a> article.
   </note> </li> 
  <li>Documents</li> 
  <li>Updates</li> 
  <li>Hours</li> 
 </ul> 
 <li>If the user has checked-out documents, the documents remain checked out when you deactivate them. Only a <em>Workfront administrator</em> can check them back in.For more information about checking out documents, see <a href="../../../documents/managing-documents/check-out-documents.md" class="MCXref xref">Check out documents</a>.</li> 
</ul>

Deleting a user causes the following things to happen:

<ul> 
 <li>Removes the user's licenses to both <em>Workfront</em> and <em>Workfront Proof</em>, if the <em>Workfront Proof</em> component is associated with your <em>Workfront</em> account. For more information about <em>Workfront Proof</em>, see <a href="../../../workfront-proof/workfront-proof.md" class="MCXref xref">Workfront Proof</a>.</li> 
 <li>The user can no longer be assigned work.</li> 
 <li>The user can no longer be added to updates.</li> 
 <li>The user can no longer be added to teams or groups.</li> 
 <li>Objects can no longer be shared with the user.</li> 
 <li>Deletes the association of that user with the following objects:</li> 
 <ul> 
  <li>Tasks, issues, projects, portfolio</li> 
  <li> <p>Dashboards</p> <note type="note">
    You also lose access to custom 
    <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      sections
     </MadCap:conditionalText>
    </draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     sections
    </MadCap:conditionalText> that contained dashboards associated to the deleted user.
    <br>To learn more, see the 
    <a href="../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how" class="MCXref xref">How do I access a dashboard that contains a report owned by a deleted user?</a> section of the 
    <a href="../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md" class="MCXref xref">Reports FAQs</a> article.
   </note> </li> 
  <li>Updates</li> 
  <li> <p>Hours</p> <note type="note">
     These objects remain in 
    <em>Workfront</em> but the owner of the object is now blank.
   </note> </li> 
 </ul> 
 <li>If the user uploaded any documents under the Documents area in the Global Navigation Bar, the documents are also deleted.</li> 
 <li>If the user has checked out documents that they own and the documents are uploaded in the main Documents area (accessed from the <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Main Menu
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Main Menu
  </MadCap:conditionalText>), the documents are deleted with the user. For more information about checking out documents, see <a href="../../../documents/managing-documents/check-out-documents.md" class="MCXref xref">Check out documents</a>.</li> 
</ul>

For more information about deactivating users, see [Deactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

You can permanently delete users one at a time, or you can permanently delete multiple users simultaneously. When you delete individual users, you must wait for the deletion process to complete prior to&nbsp;moving on to other activities in *Workfront*. The process of deleting multiple users simultaneously runs as a background process, so you can continue using *Workfront* as the users are deleted.

## Delete one or more users

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Users</span>.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Users</span>.</li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p> <draft-comment>
     <MadCap:conditionalText class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
      If you are using the Production environment, s
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
     If you are using the Production environment, s
    </MadCap:conditionalText>Select at least one user that you want to delete, then click <b>More</b> > <b>Delete</b>.</p> <draft-comment>
    <div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <p>Or</p> 
     <p>If you are using the Preview environment, select at least one user that you want to delete, click the More menu <img src="assets/more-icon.png">, then click <b>Delete</b>.</p> 
    </div>
   </draft-comment>
   <div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <p>Or</p> 
    <p>If you are using the Preview environment, select at least one user that you want to delete, click the More menu <img src="assets/more-icon.png">, then click <b>Delete</b>.</p> 
   </div> </li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p> <MadCap:conditionalText class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
    If you are using the Production environment, s
   </MadCap:conditionalText>Select at least one user that you want to delete, then click <b>More</b> > <b>Delete</b>.</p> 
  <div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <p>Or</p> 
   <p>If you are using the Preview environment, select at least one user that you want to delete, click the More menu <img src="assets/more-icon.png">, then click <b>Delete</b>.</p> 
  </div> </li> 
 <li value="4"> <p>In the box that appears, click <span class="bold">Delete Anyway</span><draft-comment>
    <b class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">Delete</b>
   </draft-comment><b class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">Delete</b> to confirm the deletion.</p> <p>The process of deleting users runs as a background process, so you can continue using <em>Workfront</em> as the user or users are deleted.</p> <p>Depending on the number of users you are deleting, the process can take several minutes or even a few hours.</p> <p>After receiving the confirmation in <em>Workfront</em> that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.</p> <p>At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.</p> </li> 
</ol>

