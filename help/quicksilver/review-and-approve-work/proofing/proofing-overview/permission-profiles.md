---
content-type: overview
product-area: documents
keywords: proof,permission
navigation-topic: proofing-overview
title: Proof Permission Profile overview
description: Proof Permission Profiles determine what overall permissions users have over all proofs in your account. Proof Permission Profiles are assigned to users in their User Profile. Proof Permission Profiles are different from proof roles. For more information about proof roles, see Proof Roles overview.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
---
# Proof Permission Profile overview

Proof Permission Profiles determine what overall permissions users have over all proofs in your account. Proof Permission Profiles are assigned to users in their User Profile. Proof Permission Profiles are different from proof roles. For more information about proof roles, see [Proof Roles overview](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>If you are an Administrator, you can create custom profiles for users in your organization. For more information, see [Configure custom profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the&nbsp;account settings&nbsp;and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in&nbsp;Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them.&nbsp;</li>
</ul>
-->

## Proof Permission Profiles

The following table displays the permissions available with each Proof Permission Profile.

| **Own Items** | | | | | **Other Users' Items** | | | **Admin** | **Billing** |
|---|---|---|---|---|---|---|---|---|---|
| &nbsp; |**Add** |**View** |**Edit** |**Delete** |**View** |**Edit** |**Delete** |**Edit and Delete** |**Edit** |
| Admin | ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| |
| Supervisor | ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)|&nbsp; |&nbsp; |
| Manager | ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)| ![](assets/cleaner2.png)|&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| Observer |&nbsp; | ![](assets/cleaner2.png)|&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

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
     <li> <p>Delete the public&nbsp;folders of other Users</p> </li> 
     <li> <p>Edit all proofs created in the account</p> </li> 
     <li> <p>Be set as the Dropzone owner*</p> </li> 
     <li> <p>Access the&nbsp;Account Settings page and edit the account details</p> </li> 
     <li> <p>Empty the&nbsp;trash</p> </li> 
     <li> <p>Add, edit, and delete users</p> </li> 
     <li> <p>Create groups and add new contacts</p> </li> 
     <li> <p>Delete contacts</p> </li> 
     <li> <p>Edit proofs&nbsp;if there are no replies on them</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Edit proof replies.</p> </li> 
     <li> <p>Delete the private&nbsp;folders of other Users</p> </li> 
     <li> <p>Access the&nbsp;Billing page or edit the billing details</p> </li> 
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
     <li> <p>Delete the public&nbsp;folders of other Users</p> </li> 
     <li> <p>Edit all proofs created in the account</p> </li> 
     <li> <p>Create groups and add new contacts</p> </li> 
     <li> <p>Delete contacts</p> </li> 
     <li> <p>Edit proofs&nbsp;if there are no replies on them</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Edit proof replies.</p> </li> 
     <li> <p>Delete the private&nbsp;folders of other Users</p> </li> 
     <li> <p>Access the&nbsp;Billing page or edit the billing details</p> </li> 
     <li> <p>Add, edit, or delete users</p> </li> 
     <li> <p>Empty the&nbsp;trash</p> </li> 
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
     <li> <p>View, edit, or delete proofs and files created by other users in the organization.&nbsp;</p> <p>Edit proof replies.</p> </li> 
     <li> <p>Delete the private&nbsp;or public folders of other Users</p> </li> 
     <li> <p>Access the&nbsp;Billing page or edit the billing details</p> </li> 
     <li> <p>Add, edit, or delete users</p> </li> 
     <li> <p> Delete contacts</p> </li> 
     <li> <p>Empty the&nbsp;trash</p> </li> 
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
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot&nbsp;create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs&nbsp;or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access&nbsp;the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a>&nbsp;and&nbsp;<a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the&nbsp;trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts.&nbsp;</p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited.&nbsp;</p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing </li>>
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
&nbsp;Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
