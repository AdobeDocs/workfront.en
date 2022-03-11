---
filename: create-automated-proof-workflow
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Create an advanced proof with an Automated workflow
description: An Automated Workflow makes it easier to manage the review process if your process is complex, or if you send content for review to the same people regularly. The proof moves from stage to stage and Adobe Workfront notifies each user when it is their turn to review it. For more information about Automated workflows, see Automated Workflow overview.
---

# Create an advanced proof with an Automated workflow

An Automated Workflow makes it easier to manage the review process if your process is complex, or if you send content for review to the same people regularly. The proof moves from stage to stage and Adobe Workfront notifies each user when it is their turn to review it. For more information about Automated workflows, see [Automated Workflow overview](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Higher</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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

## Create an advanced proof with an Automated workflow

1. Go to the project, task, or issue where you want the proof, then click the `Documents` tab.
1. Click `Add new` > Proof, upload the content, then work through the sections listed below.

   or

   Hover over an existing document, then click the `Create Proof` > `Advanced Proof` and work through the sections listed below.

## Configure the proof Stages

<ol> 
 <li value="1">In the Workflow type section, choose <span class="bold">Automated</span>.</li> 
 <li value="2"> <p>(Optional) If you want to use an Automated Workflow template that your Workfront administrator created and shared with you, click <span class="bold">Add template</span>, select the template in the box that appears, then click <span class="bold">Add template</span>.</p> <note type="note">
    Consider the following when you use an Automated Workflow template: &nbsp; 
   <ul>
    <li style="font-style: normal;">An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a proof. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the proof. </li>
    <li style="font-style: normal;">When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the proof, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. </li>
    <li style="font-style: normal;">Your ability to modify an Automated Workflow template depends on the template settings configured by the Workfront administrator, as described in <a href="../../../administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md" class="MCXref xref">Create and manage Automated Workflow templates</a>. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.</li>
   </ul>
  </note> </li> 
 <li value="3">Configure the first stage of the Automated Workflow:
  <ol>
   <li value="1">(Optional) If you want to create a name for the first stage, click <span class="bold">Stage 1</span>, then type the name.</li>
   <li value="2"><p>In the <span class="bold">Recipients</span> section for the stage, add reviewers to the stage.</p><note type="note">
     Consider the following when&nbsp;adding reviewers to a stage:
     <ul>
      <li><p>You can add external users to a stage with an email address.</p></li>
      <li>After you add a user to a stage, you can configure settings for that user on the proof.</li>
      <li><p>You can drag users directly to another stage, or you can drag users to a stage on the <span class="bold">Stages</span> diagram. To select multiple users, press Shift+Ctrl (on Windows) or Shift+Command (on Mac).</p></li>
      <li>You&nbsp;can add a reviewer to a proof only once, which means that you cannot add the same person to more than one stage on the proof.</li>
      <li>Reviewers who are not added to a private stage cannot see that stage on the proof or comments made in that stage.</li>
      <li><p>By default, adding a user&nbsp;to a stage grants&nbsp;that user access to view the proof from the moment the proof is created.<br></p><p>Your Workfront administrator can restrict users from accessing the proof until the workflow enters the stage where the user was added. For more information, see&nbsp;<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md" class="MCXref xref">Configure sharing settings for your users</a>&nbsp;in&nbsp;<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md" class="MCXref xref">Configure sharing settings for your users</a>.</p></li>
     </ul>
    </note></li>
   <li value="3">Click <span class="bold">Stage settings</span>.</li>
   <li value="4"><p>Click an <span class="bold">Activate stage</span> option to indicate how you want the stage to activate.</p><p>For the first stage, you can select only <span class="bold">On proof creation</span>, <span class="bold">On a specific date and time</span>, or <span class="bold">Manually</span>. </p></li>
   <li value="5">(Conditional) If you selected <span class="bold">On a specific date and time</span> in the previous step, select the date and time when you want to activate the stage in the <span class="bold">Activate on</span> box that appears.</li>
   <li value="6"><p>Use any of the options below to further configure the stage.</p>
    <table cellspacing="0">
     <col>
     <col>
     <tbody>
      <tr>
       <td role="rowheader">Set stage deadline</td>
       <td><p>To set a deadline for the stage, click an option in the <span class="bold">Deadline options</span> drop-down list. Then, under <span class="bold">Deadline</span>, do one of the following:</p>
        <ul>
         <li>If you chose <span class="bold">Set specific date</span>: Select the deadline date and time you want.</li>
         <li>If you chose <span class="bold">Calculate from stage activation date</span>: Select the number of business days you want to add to the stage activation date to determine the deadline.</li>
        </ul></td>
      </tr>
      <tr>
       <td role="rowheader">Lock stage</td>
       <td>Specify when the stage can be locked. </td>
      </tr>
      <tr>
       <td role="rowheader">Transfer primary decision rights to</td>
       <td><p>Select the Primary decision maker on the stage (available only after you add&nbsp;at least one person to the stage who has a Proof role of Approver or higher). If you select a Primary decision maker, the <span class="bold">Only one decision required</span> option is disabled on this stage.</p></td>
      </tr>
      <tr>
       <td role="rowheader">Require only one decision for this stage</td>
       <td>Ends the entire review process when one of the decision makers makes a decision.<p>This option is not available if you designated a user in the&nbsp;<span class="bold">Primary decision maker&nbsp;</span>drop-down menu.</p></td>
      </tr>
      <tr>
       <td role="rowheader">Make this stage private</td>
       <td>Allows only the following people to view comments and decisions made during this stage: Supervisors, Workfront administrators, and Workfront Proof administrators</td>
      </tr>
     </tbody>
    </table></li>
  </ol></li> 
 <li value="4">To add and configure another stage:
  <ol style="list-style-type: lower-alpha;">
   <li value="1">Click <span class="bold">New stage</span>.</li>
   <li value="2">(Optional) If you want to create a name for the first stage, click <span class="bold">Stage 2</span> (or <span class="bold">Stage 3</span>, <span class="bold">Stage 4</span>, and so on), then type the name.</li>
   <li value="3"><p>Click the <span class="bold">Activate stage</span>, then select an option to specify whether the stage is activated automatically or manually.</p><p>In addition to the options <span class="bold">On proof creation</span>, <span class="bold">On a specific date and time</span>, or <span class="bold">Manually</span>, you can select an option that is dependent on what occurred in the previous step: </p><p><img src="assets/activate-stage-options-for-stage-2-plus-350x177.png" style="width: 350;height: 177;"></p></li>
   <li value="4"><p>If you selected an Activate stage option that is dependent on what occurred in the previous step, use the options that appear to configure the activation setting. </p><p>For example, if you selected <span class="bold">When previous stage status changes</span>, select the <span class="bold">Previous stage</span>, then select the status in the <span class="bold">Status changed to</span> box.</p></li>
  </ol></li> 
 <li value="5"> <p>Repeat the previous step as needed to add more stages.</p> <p>As you add stages to the Automated Workflow, a diagram forms on the screen to represent them:</p> <p> <img src="assets/stages-diagram-350x213.png" style="width: 350;height: 213;"> </p> </li> 
</ol>

1. Continue with [Configure email settings for the proof](#configur2) below.

## Configure email settings for the proof

<ol> 
 <li value="1"> <p>In the <span class="bold">Email notification</span> section, select whether to send email notifications and a custom message to&nbsp;the users you selected in <a href="#workflow" class="MCXref xref">Create an advanced proof with an Automated workflow</a> earlier in this article:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Notify recipients about this proof</td> 
     <td>Select this option to send an email notification to users. When <span class="bold">Basic sharing</span> is selected in the <span class="bold">Workflow</span> section, an email notification is sent when the proof is created. When <span class="bold">Automated workflow</span> is selected in the <span class="bold">Workflow</span> section, an email notification is sent when the proof enters the stage of the Automated Workflow that the user is associated with.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Add custom message</td> 
     <td>Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

1. Continue with [Configure proof settings](#configur3) below.

## Configure proof settings

<ol> 
 <li value="1"> <p>In the <span class="bold">Proof settings</span> section, select any of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Require login - proof can only be shared with other users</td> 
     <td>When this option is disabled (default), anyone with the URL is able to view the proof. <br>When this option is selected:
      <ul>
       <li>Only Workfront Proof&nbsp;users are able to view the proof.</li>
       <li>Users cannot sign in to the proof unless they have been added to the proof.</li>
       <li>Subscriptions cannot be enabled.</li>
      </ul></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Only one decision required for this proof</td> 
     <td>When this option is selected, the review is completed after one of the decision makers makes their decision.<br>This option is disabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Require decisions to be electronically signed</td> 
     <td>Users are required to specify their user name and password at the time that they make a decision on&nbsp;a proof.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock proof when all required decisions are made</td> 
     <td>When this setting is enabled, the proof state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.<br>This option is disabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Download original file</td> 
     <td>When this option is selected, reviewers are able to download the original file from which the proof was created.<br>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Share proof via public URL or embed code</td> 
     <td>When this option is selected, the proof can be shared via a public URL or embed code.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Subscribe to proof via public URL or embed code</td> 
     <td>When this option is selected, people who have not been added explicitly to the proof can subscribe to the proof. The person subscribing to the proof is granted the role and email that you define in the following settings:
      <ul>
       <li><span class="bold">Subscriber role:</span>&nbsp;The default proof role that is&nbsp;assigned to all reviewers that subscribe to the proof.&nbsp;</li>
       <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the proof.</li>
      </ul><p>
       <ul>
        <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the proof. You can select <span class="bold">No email</span> (email link is not required to access the proof), <span class="bold">Proof notification email only</span> (subscriber receives a link to the proof via email without any verification), or <span class="bold">Validation and proof notification emails</span> (subscriber receives a link to the proof via email and must click the link to access a proof, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
       </ul><note type="note">
        &nbsp;If the proofs have Automated Workflow attached all subscriptions will generate confirmation emails to the proof Owners, so they could decide which stage the person should be added to.
        <br>
       </note></p></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>Click <span class="bold">Create Proof</span>.</p> <p>Workfront&nbsp;begins generating a proof of the selected documents or websites.&nbsp;Depending on the file size and type, the lag time on a document upload can vary. Be patient as bigger files take longer to generate. You can navigate away from the page and Workfront&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.<br></p> </li> 
 <li value="3"> <p>After&nbsp;the proof is generated, click&nbsp;<span class="bold">Open proof</span>&nbsp;to launch the proofing viewer.</p> <p>  </p> <p>Users who do not have proofing enabled on their account&nbsp;are still able to view the document and make comments to the proof<a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md">.</a><br></p> </li> 
</ol>

