---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Edit proof settings
description: You can edit proof settings any time after you create a proof.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
---
# Edit proof settings

You can edit proof settings any time after you create a proof.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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
   <td role="rowheader">Proof Role</td> 
   <td>Author or Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Edit proof settings

Some settings may be locked if your Workfront administrator disabled them at the account level.

1. Go to the project, task, or issue where you want the proof, then click the **Documents** tab.
1. Mouse over the proof, then click **Document Details**.
1. In the left panel, click **Proofing Viewer Settings**. 
1. Adjust the following settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Require login. This proof cannot be shared with guest users</td> 
      <td> <p>If you require higher levels of security for your review and approval process, you can use require login to the proof. This means that only Workfront&nbsp;users can be added to the proof. They must enter their email and password before they can access it.</p> <p>Note: <em style="font-style: normal;">If Login required is enabled, Subscriptions cannot be enabled.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require decisions to be electronically signed</td> 
      <td> <p>You can require an electronic signature of any reviewer who makes a decision on the proof. When&nbsp;a reviewer makes a decision, a prompt appears asking them to input their email and password and to confirm their decision. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock proof when all required decisions are made</td> 
      <td> <p>You can set a proof state to lock when the final Approver makes their decision. This is useful if you want to make sure that your reviewers won't be able to go back to the proof and add additional comments or change their decisions.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow downloading the original file</td> 
      <td> <p>You can allow reviewers on a proof to download the original file from which a proof was created. This is enabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow sharing proof via public URL or embed code</td> 
      <td>You can allow users to share the proof with a public URL or embed code. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow subscribing to proof via public URL or embed code</td> 
      <td> <p>Enabling subscription on the proof allows people who have not been added explicitly to the proof to subscribe themselves to the proof (i.e. add themselves to the proof). They will then be assigned the role and email alert that you select for them in the Subscription settings.</p> <p>If Subscription has been enabled on a proof, the fields below will become active:</p> 
       <ul> 
        <li><strong>Subscriber validation required</strong> - Subscriber must click a link in an email to access a proof<br>Selecting this option means that the person subscribing will not get immediate access to the proof, but will get a link to the proof in an email. The purpose of subscriber validation is to ensure that the person has entered a correct email address to which they have access.</li> 
        <li><strong>Default role for new subscribers -</strong> This is the default proof role that will be assigned to all reviewers that subscribe themselves to the proof.</li> 
        <li><strong>Default email alert for new subscribers</strong>&nbsp;- This the default email alert that will be assigned to all reviewers that subscribe themselves to the proof.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

&nbsp;
