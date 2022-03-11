---
filename: create-new-proof-version
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Create a new version of a proof
description: Managing feedback across multiple versions or revisions of a piece of work can be a huge challenge. Workfront Proof simplifies this process by letting you create and compare multiple versions of a proof.
---

# Create a new version of a proof

Managing feedback across multiple versions or revisions of a piece of work can be a huge challenge. Workfront Proof simplifies this process by letting you create and compare multiple versions of a proof.

Consider the following information when you are creating a new version of a proof:

* There is no limit to the number of versions of a proof you can create. 
* You can give a user permission to see one version but not another. Conversely, if you share a later version with a user, that user cannot see earlier versions unless you go back and explicitly grant the user access to those previous versions. 
* To create a new version of a proof you must have Edit rights on the proof.

  See [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) and [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) to get more information on who has edit rights on a proof.

  For information about sharing proof versions, see&nbsp; [Share a Proof in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>If a proof is created within Adobe Workfront, any new versions created for that proof must also be created within Workfront. You cannot create a new version of a proof within Workfront Proof if that proof was created within Workfront. For information about how to create proof versions within Workfront, see [Create a new version of a proof](#).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Create a new version of a proof in Workfront

There are several ways to upload a new proof version in Workfront. Default proof settings may or may not carry over from the previous version depending on the method you choose:

|  Automatically generate proofs when uploading documents |Default proof settings do not carry over. If you have this setting enabled in your user profile, default proof settings do not carry over when you drag and drop a new version. |
|---|---|
| Create proof > Simple |Default proof settings do not carry over. If you choose Simple when creating a new proof version, default proof settings do not carry over from the previous version.  |
| Add new > Version > Proof |Default proof settings carry over from the previous version.  |
| Create proof > Advanced |Default proof settings carry over from the previous version.  |

1. Open the document list that contains the proof.
1. From your computer's file system, drag and drop a new file over the proof.

   Or

   Select the row where the proof is listed, click `Add new` > `Version`, then click the option you want to use to add the new version of the proof.

## Create a new version of a proof from the proofing viewer (Workfront Proof only)

If you are using the standalone Workfront Proof, you can create a new version of a proof containing a single file or web capture.&nbsp;

>[!NOTE]
>
>If your account is on an Enterprise plan and you upload multiple files or web captures, they will be automatically combined into a single new version. Please see [Create a multi-page proof](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) for more information.

To create a new version of a proof in Workfront Proof:

<ol> 
 <li value="1">Open the proof.</li> 
 <li value="2"> <p>Click the <span class="bold">Version</span> drop-down menu in the upper-left corner, then click <span class="bold">+ New version</span> in the box that appears.</p> <p>On the <span class="bold">New proof version of</span> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li> 
 <li value="3"> <p>Under <span class="bold">Add files</span>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <span class="bold">browse</span> and selecting the file you want. You can type a&nbsp;<span class="bold">Proof name</span>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
    Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
   <br>
  </note> </li> 
 <li value="4"> <p>Under <span class="bold">Workflow</span>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p> 
  <ul> 
   <li>Change the <span class="bold">Owner</span> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li> 
   <li> <p>Using the <span class="bold">Type contact name or email address to add a recipient box</span>, add reviewers to the version. You can specify a <span class="bold">Proof role</span> and an <span class="bold">Email alerts</span> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
     If the creator or owner of&nbsp;&nbsp;the proof has 
     <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see 
     <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also 
     <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and 
     <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
     <br>
    </note> </li> 
   <li>Set a proof deadline for the version.<br></li> 
   <li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li> 
  </ul> </li> 
 <li value="5">Under <span class="bold">Email notification</span>, do any of the following: 
  <ul>
   <li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Activity section of the Proof details page. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref">Manage Proof Details in Workfront Proof</a>.</li>
   <li>Add a custom subject and message.</li>
  </ul></li> 
 <li value="6">In the <span class="bold">Organization</span> section, do any of the following:&nbsp; 
  <ul>
   <li>Apply one or more tags to the proof. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md" class="MCXref xref">Create and Manage Tags in Workfront Proof</a>.<br>Note that tags are inherited from the previous version of the proof, as well. If you add a new tag&nbsp;to the new version, previous versions are also tagged.</li>
   <li>Add the version to a folder. See <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a> for more information.<span class="bold"><br></span>The folder&nbsp;will be copied from the previous version of the proof. If you select a different folder, the whole proof (all versions) will be moved.</li><note type="note">
    Billing administrators and Administrators can make the folder field mandatory across the whole account on the Settings tab. See 
    <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md" class="MCXref xref">Configure proof settings for your organization</a> for more information. 
   </note>
  </ul></li> 
 <li value="7">Under Proof settings, make any of the changes below: 
  <ul>
   <li>Require login on the proof</li>
   <li>Require electronic signatures on the proof (Enterprise plan only)</li>
   <li>Lock the proof when all decisions are made</li>
   <li>Allow or block download of original file</li>
   <li>Public sharing of the proof,&nbsp;including public sharing settings</li>
   <li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page (where some fields can be edited). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref">Manage Proof Details in Workfront Proof</a>.</li>
  </ul></li> 
</ol>

<!--
Create a new version of a proof from the proofing viewer
-->

<!--
To create a new version from the proofing viewer
-->

<!--
Open the proof. Click the Version drop-down menu in the upper-left corner, then click + New version in the box that appears. On the New proof version of page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page. Under Add files, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking browse and selecting the file you want. You can type a Proof name for the version or leave this box blank to use the same filename with a version number added on the end. Or Capture a web page as a new version of the proof by typing a URL Note: Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari. Under Workflow, make any of the following changes to specify the reviewers for this version of the proof. Reviewers from the previous version are replaced by the reviewers you add. Change the Owner of the version to another user in your account. For information about owner permissions, see Proof Permissions Profiles in Workfront Proof. Using the Type contact name or email address to add a recipient box, add reviewers to the version. You can specify a Proof role and an Email alerts type for each recipient. For information about adding groups to the proof, see Add Groups to a Proof. For information about roles, see Manage Proof Roles in Workfront Proof. Note: If the creator or owner of the proof has The Proof Made email disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see Configure email notification settings in Workfront Proof. See also The Proof Made email and New proof email. Set a proof deadline for the version. Hover over a reviewer's name to see any decisions he or she made on a previous version. Under Email notification, do any of the following: Specify whether you want to notify the reviewers of the new version. Your selection will be logged in the Proof activity section on the Proof details page. Add a custom subject and message. Under Proof settings, make any of the changes below: Require login on the proof Require electronic signatures on the proof (Enterprise plan only) Lock the proof when all decisions are made Allow or block download of original file Public sharing of the proof, including public sharing settings Subscription to the proof The selections made in this section will be shown in the Proof details page.
-->

## About the New Version message

If there was a custom subject/message included in the previous version of the proof, it will show by default on the New version page. You can:

<ul> 
 <li>Edit the subject and message.</li> 
 <li> <p>Unselect the Notify people by email box, meaning no email will be sent to your reviewers to notify them that they have a new version to review.</p> <note type="note">
   &nbsp;This is not impacted by any default custom subject/message saved in your personal settings.
  </note> </li> 
</ul>

If you have a default subject and message saved in your personal settings, this will impact on what message is shown by default on the New version page:

* If you chose to notify your reviewers by email for the previous version of the proof using the standard email (for example, no custom subject/message), your default custom subject/message (your personal settings) will be shown on the New version page. You can then edit the custom subject and message or unselect the Notify people by email box (meaning no email will be sent to your reviewers to notify them that they have a new version to review).
* If you chose not to notify your reviewers by email for the previous version of the proof (for example, no standard or custom email), the New version page will not include any message by default. To notify your reviewers of the new version, click the Send a Message link, which will show your default custom subject/message (per your personal settings). You can then edit the custom subject and message if needed.

If you do not have a default subject and message saved in your personal settings, the following will show on the New version page:

* If you chose to notify your reviewers by email for the previous version of the proof using the standard email (for example, no custom subject/message), the Notify people by email option will be selected by default on the New version page. To add a custom message click the link.
* If you chose not to notify your reviewers by email for the previous version of the proof (for example, no standard or custom email), the New version page will not include any message by default. To notify your reviewers of the new version, click the Send a Message link. You can then add a custom subject and message by clicking the Add Custom Message link.

