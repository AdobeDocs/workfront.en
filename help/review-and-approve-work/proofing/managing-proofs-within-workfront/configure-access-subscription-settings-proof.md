---
filename: configure-access-subscription-settings-proof
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configure access and subscription settings for a proof
description: You can configure certain access and subscription settings for individual proofs, such as whether to require users to log in and whether to allow users to subscribe to the proof. You can set up access and subscription settings for a proof while you are creating it, or you can set them up for a proof that already exists in Workfront.
---

# Configure access and subscription settings for a *proof*

You can configure certain access and subscription settings for individual *proofs*, such as whether to require users to log in and whether to allow users to subscribe to the *proof*. You can set up access and subscription settings for a *proof* while you are creating it, or you can set them up for a *proof* that already exists in *Workfront*.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Proof Permission Profile</em> </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *Proof Permission Profile* you have, contact your *Workfront* or *Workfront Proof administrator*.

## Configure access and subscription settings while creating a *proof*

To set up access and subscription settings for a *proof* while you are creating it:

<ol> 
 <li value="1">Begin the process for generating a <em>proof</em> on a document or website, as described in the <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a> articles.</li> 
 <li value="2">Scroll to the <span class="bold">Proof settings</span> section in the lower-right corner of the <span class="bold">New proof</span> page.</li> 
 <li value="3"> <p>Configure the following settings:<br></p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Allow sharing proof via public URL or embed code</span> </td> 
     <td>When this option is selected, the <em>proof</em> can be shared via a public URL or embed code.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Allow subscribing to proof via public URL or embed code</span> </td> 
     <td>When this option is selected, people who have not been added explicitly to the <em>proof</em> can subscribe to the <em>proof</em>. The person subscribing to the <em>proof</em> is granted the role and email that you define in the following settings:
      <ul>
       <li><p><span class="bold">Subscriber role:</span>&nbsp;The default <em>proof</em> role that is&nbsp;assigned to all reviewers that subscribe to the <em>proof</em>.&nbsp;</p><note type="important">
         If 
         <span class="bold">Allow Sharing With</span> is set to anything other than 
         <span class="bold">Everyone</span> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see 
         <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.
        </note></li>
       <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <em>proof</em>.</li>
      </ul><p>
       <ul>
        <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <em>proof</em>. You can select <span class="bold">No email</span> (email link is not required to access the <em>proof</em>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <em>proof</em> via email without any verification), or <span class="bold">Validation and <em>proof</em> notification emails</span> (subscriber receives a link to the <em>proof</em> via email and must click the link to access a <em>proof</em>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
       </ul><note type="note">
        &nbsp;If the 
        <em>proofs</em> have Automated Workflow attached all subscriptions will generate confirmation emails to the 
        <em>proof</em> Owners, so they could decide which stage the person should be added to.
        <br>
       </note></p></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">Continue creating your proof.</li> 
</ol>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver">Configure access and subscription settings for an existing proof</h2>
-->

## Configure access and subscription settings for an existing proof

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">To set up access and subscription settings&nbsp;for a <em>proof</em>&nbsp;that already exists in <em>Workfront</em>:</p>
-->

To set up access and subscription settings&nbsp;for a *proof*&nbsp;that already exists in *Workfront*:

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<li value="1">Generate the <em>proof</em> (if you have not already done so) as described in the <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a> articles.</li>
<li value="2">In the Documents area, select the document that contains the <em>proof</em> you want to configure settings for,&nbsp;then click <span class="bold">Document Details</span>.</li>
<li value="3">In the left panel, click <span class="bold">Proofing Viewer Settings</span>.</li>
<li value="4"> <p>Configure the following settings:<br></p>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><span class="bold">Allow sharing proof via public URL or embed code</span><span class="bold">e</span> </td>
<td>When this option is selected, the <em>proof</em> can be shared via a public URL or embed code.</td>
</tr>
<tr>
<td role="rowheader"><span class="bold">Allow subscribing to proof via public URL or embed code</span> </td>
<td>When this option is selected, people who have not been added explicitly to the <em>proof</em> can subscribe to the <em>proof</em>. The person subscribing to the <em>proof</em> is granted the role and email that you define in the following settings:
<ul>
<li><p><span class="bold">Subscriber role:</span>&nbsp;The default <em>proof</em> role that is&nbsp;assigned to all reviewers that subscribe to the <em>proof</em>.&nbsp;</p><note type="important">
If
<span class="bold">Allow Sharing With</span> is set to anything other than
<span class="bold">Everyone</span> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see
<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.
</note></li>
<li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <em>proof</em>.</li>
</ul><p>
<ul>
<li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <em>proof</em>. You can select <span class="bold">No email</span> (email link is not required to access the <em>proof</em>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <em>proof</em> via email without any verification), or <span class="bold">Validation and <em>proof</em> notification emails</span> (subscriber receives a link to the <em>proof</em> via email and must click the link to access a <em>proof</em>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
</ul><note type="note">
&nbsp;If the
<em>proofs</em> have Automated Workflow attached all subscriptions will generate confirmation emails to the
<em>proof</em> Owners, so they could decide which stage the person should be added to.
<br>
</note></p></td>
</tr>
</tbody>
</table> </li>
<li value="5">Click <span class="bold">Save</span>.</li>
</ol>
-->

<ol data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
 <li value="1">Generate the <em>proof</em> (if you have not already done so) as described in the <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a> articles.</li> 
 <li value="2">In the Documents area, select the document that contains the <em>proof</em> you want to configure settings for,&nbsp;then click <span class="bold">Document Details</span>.</li> 
 <li value="3">In the left panel, click <span class="bold">Proofing Viewer Settings</span>.</li> 
 <li value="4"> <p>Configure the following settings:<br></p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Allow sharing proof via public URL or embed code</span><span class="bold">e</span> </td> 
     <td>When this option is selected, the <em>proof</em> can be shared via a public URL or embed code.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Allow subscribing to proof via public URL or embed code</span> </td> 
     <td>When this option is selected, people who have not been added explicitly to the <em>proof</em> can subscribe to the <em>proof</em>. The person subscribing to the <em>proof</em> is granted the role and email that you define in the following settings:
      <ul>
       <li><p><span class="bold">Subscriber role:</span>&nbsp;The default <em>proof</em> role that is&nbsp;assigned to all reviewers that subscribe to the <em>proof</em>.&nbsp;</p><note type="important">
         If 
         <span class="bold">Allow Sharing With</span> is set to anything other than 
         <span class="bold">Everyone</span> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see 
         <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.
        </note></li>
       <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <em>proof</em>.</li>
      </ul><p>
       <ul>
        <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <em>proof</em>. You can select <span class="bold">No email</span> (email link is not required to access the <em>proof</em>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <em>proof</em> via email without any verification), or <span class="bold">Validation and <em>proof</em> notification emails</span> (subscriber receives a link to the <em>proof</em> via email and must click the link to access a <em>proof</em>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
       </ul><note type="note">
        &nbsp;If the 
        <em>proofs</em> have Automated Workflow attached all subscriptions will generate confirmation emails to the 
        <em>proof</em> Owners, so they could decide which stage the person should be added to.
        <br>
       </note></p></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

