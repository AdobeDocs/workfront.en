---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configure access and subscription settings for a proof
description: You can configure certain access and subscription settings for individual proofs, such as whether to require users to log in and whether to allow users to subscribe to the proof. You can set up access and subscription settings for a proof while you are creating it, or you can set them up for a proof that already exists in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
---
# Configure access and subscription settings for a proof

You can configure certain access and subscription settings for individual proofs, such as whether to require users to log in and whether to allow users to subscribe to the proof. You can set up access and subscription settings for a proof while you are creating it, or you can set them up for a proof that already exists in Workfront.

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
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Configure access and subscription settings while creating a proof

To set up access and subscription settings for a proof while you are creating it:

1. Go to the project, task, or issue where you want the proof, then click the **Documents** section.
1. Click **Add New** on the upper-right area.
1. Scroll to the **Proof settings** section in the lower-right corner of the **New proof** page.

1. Configure the following settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Allow sharing proof via public URL or embed code</strong> </td> 
      <td>When this option is selected, the proof can be shared via a public URL or embed code.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allow subscribing to proof via public URL or embed code</strong> </td> 
      <td>When this option is selected, people who have not been added explicitly to the proof can subscribe to the proof. The person subscribing to the proof is granted the role and email that you define in the following settings:
       <ul>
        <li><p><strong>Subscriber role:</strong>&nbsp;The default proof role that is&nbsp;assigned to all reviewers that subscribe to the proof.&nbsp;</p><p>Important: If <strong>Allow Sharing With</strong> is set to anything other than <strong>Everyone</strong> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</p></li>
        <li><strong>Email alert settings for subscribers:</strong>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the proof.</li>
       </ul><p>
        <ul>
         <li><strong>Proof access via email link required for:</strong>&nbsp;Configure whether the subscriber receives an email with a link to the proof. You can select <strong>No email</strong> (email link is not required to access the proof), <strong>Proof notification email only</strong> (subscriber receives a link to the proof via email without any verification), or <strong>Validation and proof notification emails</strong> (subscriber receives a link to the proof via email and must click the link to access a proof, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
        </ul><p>Note: &nbsp;If the proofs have Automated Workflow attached all subscriptions will generate confirmation emails to the proof Owners, so they could decide which stage the person should be added to.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue creating your proof.

## Configure access and subscription settings for an existing proof

To set up access and subscription settings&nbsp;for a proof&nbsp;that already exists in Workfront:

1. In the Documents area, select the document that contains the proof you want to configure settings for,&nbsp;then click **Document Details**.
1. In the left panel, click **Proofing Viewer Settings**.
1. Configure the following settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Allow sharing proof via public URL or embed code</strong><strong>e</strong> </td> 
      <td>When this option is selected, the proof can be shared via a public URL or embed code.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allow subscribing to proof via public URL or embed code</strong> </td> 
      <td>When this option is selected, people who have not been added explicitly to the proof can subscribe to the proof. The person subscribing to the proof is granted the role and email that you define in the following settings:
       <ul>
        <li><p><strong>Subscriber role:</strong>&nbsp;The default proof role that is&nbsp;assigned to all reviewers that subscribe to the proof.&nbsp;</p><p>Important: If <strong>Allow Sharing With</strong> is set to anything other than <strong>Everyone</strong> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</p></li>
        <li><strong>Email alert settings for subscribers:</strong>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the proof.</li>
       </ul><p>
        <ul>
         <li><strong>Proof access via email link required for:</strong>&nbsp;Configure whether the subscriber receives an email with a link to the proof. You can select <strong>No email</strong> (email link is not required to access the proof), <strong>Proof notification email only</strong> (subscriber receives a link to the proof via email without any verification), or <strong>Validation and proof notification emails</strong> (subscriber receives a link to the proof via email and must click the link to access a proof, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
        </ul><p>Note: &nbsp;If the proofs have Automated Workflow attached all subscriptions will generate confirmation emails to the proof Owners, so they could decide which stage the person should be added to.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.
