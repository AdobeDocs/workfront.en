---
content-type: overview
product-area: documents
keywords: proof,permission
navigation-topic: proofing-overview
title: Proof Permission Profile overview
description: Proof Permission Profiles determine what overall permissions users have over all proofs in your account. Proof Permission Profiles are assigned to users in their User Profile. Proof Permission Profiles are different from proof roles.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
---
# Proof Permission Profile overview

Proof Permission Profiles determine what overall permissions users have over all proofs in your account. Proof Permission Profiles are assigned to users in their User Profile. 

Proof Permission Profiles are different from proof roles. For more information about proof roles, see [Proof Roles overview](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>If you are an Administrator, you can create custom profiles for users in your organization. For more information, see [Configure custom profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## Proof Permission Profiles

The following table displays the permissions available with each Proof Permission Profile.

<table>
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>Own Items</strong>
   </td>
   <td colspan="3" ><strong>Other users' items</strong>
   </td>
   <td><strong>Admin</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Add</strong>
   </td>
   <td><strong>View</strong>
   </td>
   <td><strong>Edit</strong>
   </td>
   <td><strong>Delete</strong>
   </td>
   <td><strong>View</strong>
   </td>
   <td><strong>Edit</strong>
   </td>
   <td><strong>Delete</strong>
   </td>
   <td><strong>Edit and Delete</strong>
   </td>
  </tr>
  <tr>
   <td>Admin
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Supervisor
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Manager
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Administrator

Administrators have access to [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) and have the following permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Administrators can:</td> 
   <td>Administrators can't:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Create proofs, upload files, and create folders</p> </li> 
     <li> <p>View, edit, and delete proofs and files they created</p> </li> 
     <li> <p>View, edit, and delete proofs and files created by all users in the organization</p> </li> 
     <li> <p>Delete the public folders of other Users</p> </li> 
     <li> <p>Edit all proofs created in the account</p> </li> 
     <li> <p>Be set as the Dropzone owner*</p> </li> 
     <li> <p>Access the Account Settings page and edit the account details</p> </li> 
     <li> <p>Empty the trash</p> </li> 
     <li> <p>Add, edit, and delete users</p> </li> 
     <li> <p>Create groups and add new contacts</p> </li> 
     <li> <p>Delete contacts</p> </li> 
     <li> <p>Edit proofs if there are no replies on them</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Edit proof replies.</p> </li> 
     <li> <p>Delete the private folders of other Users</p> </li> 
     <li> <p>Access the Billing page or edit the billing details</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Available only in the Workfront Proof standalone product.

### Supervisor

Supervisors have the following permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Supervisors can:</td> 
   <td>Supervisors can't:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Create proofs, upload files, and create folders</p> </li> 
     <li> <p>View, edit, and delete proofs and files they created</p> </li> 
     <li> <p>View, edit, and delete proofs and files created by all users in the organization</p> </li> 
     <li> <p>Delete the public folders of other users</p> </li> 
     <li> <p>Edit all proofs created in the account</p> </li> 
     <li> <p>Create groups and add new contacts</p> </li> 
     <li> <p>Delete contacts</p> </li> 
     <li> <p>Edit proofs if there are no replies on them</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Edit proof replies.</p> </li> 
     <li> <p>Delete the private folders of other users</p> </li> 
     <li> <p>Access the Billing page or edit the billing details</p> </li> 
     <li> <p>Add, edit, or delete users</p> </li> 
     <li> <p>Empty the trash</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Manager

Managers have the following permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Managers can:</td> 
   <td>Managers can't:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Create proofs, upload files, and create folders</p> </li> 
     <li> <p>View, edit, and delete proofs and files they created</p> </li> 
     <li> <p>See, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder)</p> </li> 
     <li> <p>Edit all proofs created in the account</p> </li> 
     <li> <p>Create groups and add new contacts</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>View, edit, or delete proofs and files created by other users in the organization. </p> </li><li><p>Edit proof replies.</p> </li> 
     <li> <p>Delete the private or public folders of other Users</p> </li> 
     <li> <p>Access the Billing page or edit the billing details</p> </li> 
     <li> <p>Add, edit, or delete users</p> </li> 
     <li> <p> Delete contacts</p> </li> 
     <li> <p>Empty the trash</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
