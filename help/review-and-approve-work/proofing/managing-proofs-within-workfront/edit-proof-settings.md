---
filename: edit-proof-settings
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Edit proof settings
description: You can edit proof settings any time after you create a proof.
---

# Edit proof settings

You can edit *proof* settings any time after you create a proof.

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
   <td role="rowheader">Proof Role</td> 
   <td>Author or Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *Proof Permission Profile* you have, contact your *Workfront* or *Workfront Proof administrator*.

## Edit proof settings

Some settings may be locked if your *Workfront administrator* disabled them at the account level.

<ol> 
 <li value="1"> <p>Go to the project, task, or issue where you want the <em>proof</em>, then click the <span class="bold">Documents</span> tab.</p> </li> 
 <li value="2"> <p>Mouse over the <em>proof</em>, then click <span class="bold">Document Details</span>.</p> </li> 
 <li value="3"> <p>In the left panel, click <span class="bold">Proofing Viewer Settings</span>. </p> </li> 
 <li value="4"> <p>Adjust the following settings:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Require login. This proof cannot be shared with guest users</td> 
     <td> <p>If you require higher levels of security for your review and approval process, you can use require login to the <em>proof</em>. This means that only <em>Workfront</em>&nbsp;users can be added to the <em>proof</em>. They must enter their email and password before they can access it.</p> <note type="note">
       <em style="font-style: normal;">If Login required is enabled, Subscriptions cannot be enabled.</em> 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Require decisions to be electronically signed</td> 
     <td> <p>You can require an electronic signature of any reviewer who makes a decision on the <em>proof</em>. When&nbsp;a reviewer makes a decision, a prompt appears asking them to input their email and password and to confirm their decision. <draft-comment>
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         For more information, see 
         <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
        </MadCap:conditionalText>
       </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        For more information, see 
        <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
       </MadCap:conditionalText></p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock proof when all required decisions are made</td> 
     <td> <p>You can set a <em>proof</em> state to lock when the final Approver makes their decision. This is useful if you want to make sure that your reviewers won't be able to go back to the <em>proof</em> and add additional comments or change their decisions.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Allow downloading the original file</td> 
     <td> <p>You can allow reviewers on a <em>proof</em> to download the original file from which a <em>proof</em> was created. This is enabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Allow sharing proof via public URL or embed code</td> 
     <td>You can allow users to share the <em>proof</em> with a public URL or embed code. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Allow subscribing to proof via public URL or embed code</td> 
     <td> <p>Enabling subscription on the <em>proof</em> allows people who have not been added explicitly to the <em>proof</em> to subscribe themselves to the <em>proof</em> (i.e. add themselves to the <em>proof</em>). They will then be assigned the role and email alert that you select for them in the Subscription settings.</p> <p>If Subscription has been enabled on a <em>proof</em>, the fields below will become active:</p> 
      <ul> 
       <li><span class="bold">Subscriber validation required</span> - Subscriber must click a link in an email to access a <em>proof</em><br>Selecting this option means that the person subscribing will not get immediate access to the <em>proof</em>, but will get a link to the <em>proof</em> in an email. The purpose of subscriber validation is to ensure that the person has entered a correct email address to which they have access.</li> 
       <li><span class="bold">Default role for new subscribers -</span> This is the default <em>proof</em> role that will be assigned to all reviewers that subscribe themselves to the <em>proof</em>.</li> 
       <li><span class="bold">Default email alert for new subscribers</span>&nbsp;- This the default email alert that will be assigned to all reviewers that subscribe themselves to the <em>proof</em>.</li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

&nbsp;
