---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Create or edit an Automated Workflow for an existing proof
description: Automated Workflows make it easier to manage the review process if your process is complex or if you regularly send content for review to the same groups of people. When you create a proof with an Automated Workflow, the proof moves from stage to stage until final approval. Participants are notified when it's their turn to review the document.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
---
# Create or edit an Automated Workflow for an existing proof

Automated Workflows make it easier to manage the review process if your process is complex or if you regularly send content for review to the same groups of people.&nbsp;When you create a proof with an Automated Workflow, the proof moves from stage to stage&nbsp;until final approval. Participants are notified when it's their turn to review the document.

For information about creating an Automated Workflow for a new proof, see [Create an advanced proof with an Automated workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

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

## Create or edit an Automated Workflow for an existing proof:

1. Hover over the document in the Documents area, then click Proofing Workflow.

   Or

   If you are reviewing the proof in the proofing viewer, click **Workflow** ![](assets/workflow-icon-proofing-viewer.png) in the left panel, then click the Edit icon ![](assets/edit-icon-proofing-viewer.png) to open the Automated Workflow settings for the proof.

1. (Conditional) If the proof currently is currently using a basic workflow (without stages), click **Convert to Automated Workflow** in the screen that appears.

   >[!NOTE]
   >
   >You cannot edit the first stage when you convert from a basic workflow to an Automated Workflow, but you can add and configure new stages.

1. Conditional)&nbsp;To use an Automated Workflow template that your Adobe Workfront administrator created and shared with you, click **Add template**, select the template in the box that appears, then click **Add template**.

   For more information, see [About using Automated Workflow templates](#about-using-automated-workflow-templates) in this article.

1. Add a stage to the Automated Worfklow:

   1. Click **New stage** near the upper-right corner.
   1. In the box that appears, type a&nbsp;**Name** for the stage.
   1. (Optional) Set a deadline for the stage. 
   1. In the **Activate stage** section, choose how you want the stage to activate:

      
      <table>
      <tbody>
      <tr>
      <td><strong>On proof creation</strong></td>
      <td>The stage becomes active automatically because the proof has already been created.</td>
      </tr>
      <tr>
      <td><strong>When previous stage deadline passes</strong></td>
      <td>Click the previous stage in the <strong>Parent stage</strong> drop-down list .</td>
      </tr>
      <tr>
      <td><strong>On a specific date &amp; time</strong></td>
      <td>Click the <strong>On</strong> box to select the date, then click the box to the right to select the time.</td>
      </tr>
      <tr>
      <td><strong>All decisions are Approved or Approved with changes on parent stage</strong></td>
      <td>Click the parent stage in the <strong>Parent stage</strong> drop-down list.</td>
      </tr>
      <tr>
      <td><strong>All decisions are Approved on parent stage</strong></td>
      <td>Click the parent stage in the <strong>Parent stage</strong> drop-down list.</td>
      </tr>
      <tr>
      <td><strong>All decisions are made</strong></td>
      <td>Click the parent stage in the <strong>Parent stage</strong> drop-down list.</td>
      </tr>
      </tbody>
      </table> 


   1. Enter a contact name or email address, and configure settings for reviewers for the stage.

      For information about adding reviewers, see [About adding reviewers to a stage](#about-adding-reviewers-to-a-stage) in this article.
   
   1. Use any of the following options to further configure the stage:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Deadline options</strong> </td>
         <td><p>To set a deadline for the stage, click an option in the <strong>Deadline options</strong> drop-down list. Then, under <strong>Deadline</strong>, do one of the following:</p>
          <ul>
           <li>If you chose <strong>Set specific date</strong>: Select the deadline date and time you want.</li>
           <li>If you chose <strong>Calculate from stage activation date</strong>: Select the number of business days you want to add to the stage activation date to determine the deadline.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Lock stage</td>
         <td>Specify when the stage can be locked. </td>
        </tr>
        <tr>
         <td role="rowheader">Primary decision maker</td>
         <td><p>Select the Primary decision maker on the stage (available only after you add&nbsp;at least one person to the stage who has a Proof role of Approver or higher). If you select a Primary decision maker, the <strong>Only one decision required</strong> option is disabled on this stage.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Only one decision required</td>
         <td>Ends the entire review process when one of the decision makers makes a decision.<p>This option is not available if you designated a user in the&nbsp;<strong>Primary decision maker</strong> drop-down menu.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Private stage</td>
         <td>Allows only the following people to view comments and decisions made during this stage: Supervisors, Adobe Workfront administrators, and Workfront Proof administrators</td>
        </tr>
        <tr>
         <td role="rowheader">Notify people by email</td>
         <td>Alerts reviewers with an email notification when it's their turn to work on the proof.</td>
        </tr>
       </tbody>
      </table>

   1. Click **Add stage**.

1. Repeat the previous step as needed to add more stages.

   As you add stages to the Automated Workflow, a diagram forms on the screen to represent them:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. When you are finished adding stages, click **Done**.

## About using Automated Workflow templates {#about-using-automated-workflow-templates}

Consider the following when you use an Automated Workflow template:

1. An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a proof. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the proof. 
1. When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the proof, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. 
1. Your ability to modify an Automated Workflow template depends on the template settings configured by the Workfront administrator, as described in . If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.

## About adding reviewers to a stage {#about-adding-reviewers-to-a-stage}

Consider the following when&nbsp;adding reviewers to a stage:

* After you add a user to a stage, you can configure settings for that user on the proof, such as the proof role and any additional permissions they should have and the type of email alerts they will receive when people make comments and decisions on the proof. 
* You can drag one or more users from one stage to another. You can drag users directly to another stage, or you can drag users to a stage on the **Stages** diagram. To select multiple users, press Shift+Ctrl (on Windows) or Shift+Command (on Mac).
* You&nbsp;can add a reviewer to a proof only once, which means that you cannot add the same person to more than one stage on the proof.
* Reviewers who are not added to a private stage cannot see that stage on the proof or comments made in that stage.
* By default, adding a user&nbsp;to a stage grants&nbsp;that user access to view the proof from the moment the proof is created.

  Your Workfront administrator can restrict users from accessing the proof until the workflow enters the stage where the user was added. For more information, see&nbsp;&nbsp;in&nbsp;.
