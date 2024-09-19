---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configure Default Proofing Roles
description: As an Adobe Workfront administrator, you can configure the default proofing roles for users and guest users who access proofs created in Workfront. Any person adding users to a proof can adjust these roles for them.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
---
# Configure default proofing roles

As an Adobe Workfront administrator, you can configure the default proofing roles for users and guest users who access proofs created in Workfront. Any person adding users to a proof can adjust these roles for them.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Configure default proofing roles

{{step-1-to-setup}}

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Click **Review and Approval** near the bottom of the list that appears on the left. 
1. In the **Roles for designated recipients of a document proof** section, select the default role for users and guest users who are added to a proof's workflow.

   See [Rights associated with proofing roles](#rights-associated-with-proofing-roles) below for a list of each proofing role and the rights associated with it.

   >[!NOTE]
   >
   >* This setting applies only to users who are created in the Workfront system after the role is set; not to existing users.
   >* The person adding users to the proof can adjust this role, as described in [Add users to a proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. In the **Roles for non-recipients that open a document proof** section, select the default role for users and guest users who can access a proof, but are not added to the proof's workflow.

   This situation occurs when users and guests have access to a document for which a proof has been created: even if they have not been added to the proof's workflow, they can open the proof.

   **Examples:** Here are examples of how you could use this setting:

   * You select **Read only** to limit all proof activity such as adding comments and making decisions to those who have been asked to do it.
   * You select **Reviewer** because you want any member of the team to be able to add markups and comments on a proof.

1. Click **Save**.

## Rights associated with proofing roles {#rights-associated-with-proofing-roles}

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
   <th> <p> </p> </th> 
   <th> <p><strong>View a proof</strong> </p> </th> 
   <th> <p><strong>Add markups</strong> </p> </th> 
   <th> <p><strong>Add comments</strong> </p> </th> 
   <th> <p><strong>Edit own comments if there are no replies</strong> </p> </th> 
   <th> <p><strong>Make a decision</strong> </p> </th> 
   <th> <p><strong>Delete comments made by others</strong> </p> </th> 
   <th>Resolve comments</th> 
   <th>Apply Actions to Comments</th> 
   <th> <p><strong>Edit the proof</strong> </p> </th> 
   <th>Share the proof with others</th> 
   <th>Create new version</th> 
   <th> <p><strong>View approval requests in the Home area</strong> </p> </th> 
   <th>Add new reviewers</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Read Only</strong> </p> </td> 
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
   <td> <p><strong>Reviewer</strong> </p> </td> 
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
   <td> <p><strong>Approver</strong> </p> </td> 
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
   <td> <p><strong>Reviewer &amp; Approver</strong> </p> </td> 
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
   <td> <p><strong>Author</strong> </p> </td> 
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
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderator</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
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
