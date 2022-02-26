---
filename: create-edit-automated-workflow-existing-proof
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Create or edit an Automated Workflow for an existing proof
description: Automated Workflows make it easier to manage the review process if your process is complex or if you regularly send content for review to the same groups of people. When you create a proof with an Automated Workflow, the proof moves from stage to stage until final approval. Participants are notified when it's their turn to review the document.
---

# Create or edit an Automated Workflow for an existing *proof*

Automated Workflows make it easier to manage the review process if your process is complex or if you regularly send content for review to the same groups of people.&nbsp;When you create a *proof* with an Automated Workflow, the *proof* moves from stage to stage&nbsp;until final approval. Participants are notified when it's their turn to review the document.

For information about creating an Automated Workflow for a new proof, see [Create an advanced proof with an Automated workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

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

## Create or edit an Automated Workflow for an existing proof:

<ol> 
 <li value="1"> <p>Hover over the document in the Documents area, then click <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Proofing Workflow
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Proofing Workflow
   </MadCap:conditionalText>.</p> <p>Or</p> <p>If you are reviewing the proof in the proofing viewer, click <span class="bold">Workflow</span> <img src="assets/workflow-icon-proofing-viewer.png"> in the left panel, then click the Edit icon <img src="assets/edit-icon-proofing-viewer.png"> to open the Automated Workflow settings for the <em>proof</em>.</p> </li> 
 <li value="2"> <p>(Conditional) If the proof currently is currently using a basic workflow (without stages), click <span class="bold">Convert to Automated Workflow</span> in the <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     screen
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    screen
   </MadCap:conditionalText> that appears.</p> <note type="note">
   You cannot edit the first stage when you convert from a basic workflow to an Automated Workflow, but you can add and configure new stages.
  </note> </li> 
 <li value="3"> <p>Conditional)&nbsp;To use an Automated Workflow template that your <em>Adobe Workfront administrator</em> created and shared with you, click <span class="bold">Add template</span>, select the template in the box that appears, then click <span class="bold">Add template</span>.</p> <p>For more information, see <a href="#adding-additional-template-to-existing-workflow" class="MCXref xref">About using Automated Workflow templates</a> in this article.</p> </li> 
 <li value="4">Add a stage to the Automated Worfklow:
  <ol>
   <li value="1">Click <span class="bold">New stage</span> near the upper-right corner.</li>
   <li value="2">In the box that appears, type a&nbsp;<span class="bold">Name</span> for the stage.</li>
   <li value="3">(Optional) Set a deadline for the stage. </li>
   <li value="4"><p>In the <span class="bold">Activate stage</span> section, choose how you want the stage to activate:</p>
    <table cellspacing="0">
     <col>
     <col>
     <tbody>
      <tr>
       <td role="rowheader">On proof creation</td>
       <td>The stage becomes active automatically because the proof has already been created. </td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">When previous stage deadline passes</span></td>
       <td>Click the previous stage in the <span class="bold">Parent stage</span> drop-down list .</td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">On a specific date & time</span></td>
       <td>Click the <span class="bold">On</span> box to select the date, then click the box to the right to select the time.</td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">All decisions are Approved or Approved with changes on parent stage</span></td>
       <td>Click the parent stage in the <span class="bold">Parent stage</span> drop-down list.</td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">All decisions are Approved on parent stage</span></td>
       <td>Click the parent stage in the <span class="bold">Parent stage</span> drop-down list.</td>
      </tr>
      <tr>
       <td role="rowheader">All decisions are made</td>
       <td>Click the parent stage in the <span class="bold">Parent stage</span> drop-down list.</td>
      </tr>
     </tbody>
    </table></li>
   <li value="5"><p>Enter a contact name or email address, and configure settings for reviewers for the stage.</p><p>For information about adding reviewers, see <a href="#about" class="MCXref xref">About adding reviewers to a stage</a> in this article.</p></li>
   <li value="6"><p>Use any of the following options to further configure the stage: </p>
    <table cellspacing="0">
     <col>
     <col>
     <tbody>
      <tr>
       <td role="rowheader"><span class="bold">Deadline options</span> </td>
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
       <td role="rowheader">Primary decision maker</td>
       <td><p>Select the Primary decision maker on the stage (available only after you add&nbsp;at least one person to the stage who has a Proof role of Approver or higher). If you select a Primary decision maker, the <span class="bold">Only one decision required</span> option is disabled on this stage.</p></td>
      </tr>
      <tr>
       <td role="rowheader">Only one decision required</td>
       <td>Ends the entire review process when one of the decision makers makes a decision.<p>This option is not available if you designated a user in the&nbsp;<span class="bold">Primary decision maker&nbsp;</span>drop-down menu.</p></td>
      </tr>
      <tr>
       <td role="rowheader">Private stage</td>
       <td>Allows only the following people to view comments and decisions made during this stage: Supervisors, <em>Adobe Workfront administrators</em>, and <em>Workfront Proof administrator</em>s</td>
      </tr>
      <tr>
       <td role="rowheader">Notify people by email</td>
       <td>Alerts reviewers with an email notification when it's their turn to work on the <em>proof</em>.</td>
      </tr>
     </tbody>
    </table></li>
   <li value="7">Click <span class="bold">Add stage</span>.</li>
  </ol></li> 
 <li value="5"> <p>Repeat the previous step as needed to add more stages.</p> <p>As you add stages to the Automated Workflow, a diagram forms on the screen to represent them:</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/workflow-diagram-existing-proof-qs-350x215.png" style="width: 350;height: 215;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/workflow-diagram-existing-proof-qs-350x215.png" style="width: 350;height: 215;"> </p> </li> 
 <li value="6">When you are finished adding stages, click <span class="bold">Done</span>.</li> 
</ol>

## About using Automated Workflow templates

Consider the following when you use an Automated Workflow template:

1. `<li style="font-style: normal;">An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a <em>proof</em>. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the <em>proof</em>. </li>` `<li style="font-style: normal;">When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the <em>proof</em>, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. </li>` `<li style="font-style: normal;">Your ability to modify an Automated Workflow template depends on the template settings configured by the <em>Workfront administrator</em>, as described in <a href="../../../administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md" class="MCXref xref">Create and manage Automated Workflow templates</a>. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.</li>`

## About adding reviewers to a stage

Consider the following when&nbsp;adding reviewers to a stage:

* After you add a user to a stage, you can configure settings for that user on the *proof*, such as the proof role and any additional permissions they should have and the type of email alerts they will receive when people make comments and decisions on the proof. 
* You can drag one or more users from one stage to another. You can drag users directly to another stage, or you can drag users to a stage on the `Stages` diagram. To select multiple users, press Shift+Ctrl (on Windows) or Shift+Command (on Mac).
* You&nbsp;can add a reviewer to a *proof* only once, which means that you cannot add the same person to more than one stage on the *proof*.

* Reviewers who are not added to a private stage cannot see that stage on the *proof* or comments made in that stage.
* By default, adding a user&nbsp;to a stage grants&nbsp;that user access to view the *proof* from the moment the *proof* is created.

  Your *Workfront administrator* can restrict users from accessing the *proof* until the workflow enters the stage where the user was added. For more information, see&nbsp; [Configure sharing settings for your users](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md)&nbsp;in&nbsp; [Configure sharing settings for your users](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

