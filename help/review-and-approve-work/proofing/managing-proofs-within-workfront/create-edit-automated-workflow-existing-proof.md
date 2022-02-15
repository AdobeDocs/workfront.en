---
filename: create-edit-automated-workflow-existing-proof
product-area: documents
navigation-topic: manage-proofs-within-workfront
---



# Create or edit an Automated Workflow for an existing *`proof`* {#create-or-edit-an-automated-workflow-for-an-existing-proof}

Automated Workflows make it easier to manage the review process if your process is complex or if you regularly send content for review to the same groups of people. When you create a *`proof`* with an Automated Workflow, the *`proof`* moves from stage to stage&nbsp;until final approval. Participants are notified when it's their turn to review the document.  



For information about creating an Automated Workflow for a new proof, see [Create an advanced proof with an Automated workflow](create-automated-proof-workflow.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.proofPermissionProfile variable varname">Proof Permission Profile</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Manager or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Create or edit an Automated Workflow for an existing proof: {#create-or-edit-an-automated-workflow-for-an-existing-proof-1}




1.  Hover over the document in the Documents area, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Proofing Workflow</MadCap:conditionalText>`.


   Or


   If you are reviewing the proof in the proofing viewer, click `Workflow` ![](assets/workflow-icon-proofing-viewer.png) in the left panel, then click the Edit icon ![](assets/edit-icon-proofing-viewer.png) to open the Automated Workflow settings for the *`proof`*.

1.  (Conditional) If the proof currently is currently using a basic workflow (without stages), click `Convert to Automated Workflow` in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> screen</MadCap:conditionalText>` that appears.


   You cannot edit the first stage when you convert from a basic workflow to an Automated Workflow, but you can add and configure new stages.

1.  Conditional) To use an Automated Workflow template that your *`Adobe Workfront administrator`* created and shared with you, click `Add template`, select the template in the box that appears, then click `Add template`.


   For more information, see [About using Automated Workflow templates](#adding-additional-template-to-existing-workflow) in this article.

1. Add a stage to the Automated Worfklow:
    
    
    1. Click `New stage` near the upper-right corner.
    1. In the box that appears, type a  `Name` for the stage.
    1.  Click an `Activate stage` option to indicate how you want the stage to activate.
    1. If you chose one of the following options in step c, select an option in the setting that appears above the `Activate stage` drop-down menu to indicate when you want the stage to activate:
    
    
    
    1. In the boxes outlined in blue, add and configure settings for reviewers for the stage.
    
    
       For information about adding reviewers, see [About adding reviewers to a stage](#about) in this article.
    
    1. Use any of the following options to further configure the stage: 
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col style="width: 291px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Deadline options</span> </td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>To set a deadline for the stage, click an option in the <span class="bold">Deadline options</span> drop-down list. Then, under <span class="bold">Deadline</span>, do one of the following:</p>
    <ul>
     <li>If you chose <span class="bold">Set specific date</span>: Select the deadline date and time you want.</li>
     <li>If you chose <span class="bold">Calculate from stage activation date</span>: Select the number of business days you want to add to the stage activation date to determine the deadline.</li>
    </ul></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Lock stage</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Specify when the stage can be locked. </td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Primary decision maker</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select the Primary decision maker on the stage (available only after you add&nbsp;at least one person to the stage who has a Proof role of Approver or higher). If you select a Primary decision maker, the <span class="bold">Only one decision required</span> option is disabled on this stage.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Only one decision required</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Ends the entire review process when one of the decision makers makes a decision.<p>This option is not available if you designated a user in the&nbsp;<span class="bold">Primary decision maker&nbsp;</span>drop-down menu.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Private stage</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Allows only the following people to view comments and decisions made during this stage: Supervisors, <span class="mc-variable WFVariables.FullProdNameAdminWF-plur variable varname">Adobe Workfront administrators</span>, and <span class="mc-variable WFVariables.FullProdNameAdminWFP variable varname">Workfront Proof administrator</span>s</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Notify people by email</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">Alerts reviewers with an email notification when it's their turn to work on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</td>
  </tr>
 </tbody>
</table>    
    
    
    1. Click `Add stage`.
    
    
1.  Repeat the previous step as needed to add more stages.


   As you add stages to the Automated Workflow, a diagram forms on the screen to represent them:


   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)



1. When you are finished adding stages, click `Done`.




## About using Automated Workflow templates {#about-using-automated-workflow-templates}

Consider the following when you use an Automated Workflow template:



1.  `<li style="font-style: normal;">An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. </li>` `<li style="font-style: normal;">When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. </li>` `<li style="font-style: normal;">Your ability to modify an Automated Workflow template depends on the template settings configured by the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>, as described in <a href="create-manage-automated-workflow-templates.md" class="MCXref xref">Create and manage Automated Workflow templates</a>. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.</li>` 





## About adding reviewers to a stage {#about-adding-reviewers-to-a-stage}

Consider the following when&nbsp;adding reviewers to a stage:



* After you add a user to a stage, you can configure settings for that user on the *`proof`*, such as the proof role and any additional permissions they should have and the type of email alerts they will receive when people make comments and decisions on the proof. 
*  You can drag one or more users from one stage to another. You can drag users directly to another stage, or you can drag users to a stage on the `Stages` diagram. To select multiple users, press Shift+Ctrl (on Windows) or Shift+Command (on Mac).
* You can add a reviewer to a *`proof`* only once, which means that you cannot add the same person to more than one stage on the *`proof`*.

* Reviewers who are not added to a private stage cannot see that stage on the *`proof`* or comments made in that stage.
*  By default, adding a user to a stage grants that user access to view the *`proof`* from the moment the *`proof`* is created.  



  Your *`Workfront administrator`* can restrict users from accessing the *`proof`* until the workflow enters the stage where the user was added. For more information, see&nbsp; [Configure sharing settings for your users](configure-sharing-settings-users.md)&nbsp;in&nbsp; [Configure sharing settings for your users](configure-sharing-settings-users.md).




