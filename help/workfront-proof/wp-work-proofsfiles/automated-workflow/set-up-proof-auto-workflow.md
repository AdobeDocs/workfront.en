---
filename: set-up-proof-auto-workflow
product: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Set up a proof with an Automated Workflow in Workfront Proof
description: This repeats information found in Configuring proofs in Workfront. Consolidate here or there. Maybe better here.
---

# Set up a proof with an Automated Workflow in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

<!--
This repeats information found in Configuring proofs in Workfront. Consolidate here or there. Maybe better here.
-->

Automated Workflow&nbsp;makes it easier for you to manage content review and approval when you have complex review processes, or if you send content for review to the same groups of people regularly.&nbsp;

You create the proof, then it&nbsp;moves from stage to stage&nbsp;until final approval. The relevant users are notified any time they are required to make an approval.

![stages_diagram.png](assets/stages-diagram-350x81.png)

You can add an automated workflow to a proof when uploading the document, or after the document is uploaded.

## Create a proof with Automated Workflow

<ol> 
 <li value="1">Begin creating the proof as described in <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a>.</li> 
 <li value="2"> <p>In the <span class="bold">Share</span> section, click <span class="bold">Use Automated Workflow</span>.<br></p> <p>You can deselect this option to switch back to a standard workflow.<br></p> </li> 
 <li value="3"> <p>(Optional)&nbsp;If you want to use an Automated Workflow template that your Workfront administrator configured and shared with you, select it in the <span class="bold">Select a Workflow template</span> drop-down menu.</p> <note type="note">
   Your ability to modify the template depends on the template settings configured by the Workfront administrator. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.
  </note> <p>If you are a Workfront administrator and you want to create a new Automated Workflow template, you can do so as described in <a href="../../../administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md" class="MCXref xref">Create and manage Automated Workflow templates</a></p> </li> 
 <li value="4">Specify the following information to configure&nbsp;the first stage of the Automated Workflow:</li> 
 <ul> 
  <li><span class="bold">Name: </span>The stage name appears on the Workflow diagram and is included in the email notifications sent to reviewers.</li> 
  <li><span class="bold">Deadline:&nbsp;</span>The functionality of this field differs depending on what option you select in the <span class="bold">Deadline calculated from</span> drop-down list.</li> 
  <li><span class="bold">From proof creation:&nbsp;</span>Select the deadline date for the proof.</li> 
  <li><span class="bold">From stage activation:&nbsp;</span>Select the number of business days that will be added to the stage activation date to automatically set a deadline on the proof.</li> 
  <li><span class="bold">Activate stage:&nbsp;</span>For each stage of your Workflow, you can decide when it should be activated. For your first stage, the following options are available. 
   <ul> 
    <li>On proof creation</li> 
    <li>On a specific time and date</li> 
    <li>Manually<br>Additional options are available for subsequent stages. These options require a parent stage. They are:</li> 
    <li>After previous deadline is reached</li> 
    <li>All decisions are Approved or Approved with changes</li> 
    <li>All decisions are Approved</li> 
    <li>All decisions are made</li> 
   </ul></li> 
  <li><span class="bold">Deadline calculated from:&nbsp;</span>The option you select in this drop-down list affects what options are available in the&nbsp;<span class="bold">Deadline&nbsp;</span>field.</li> 
  <li><span class="bold">Proof creation:&nbsp;</span>In the&nbsp;<span class="bold">Deadline&nbsp;</span>field, select the deadline date for the proof.</li> 
  <li><span class="bold">Stage activation:&nbsp;</span>In the&nbsp;<span class="bold">Deadline&nbsp;</span>field, select the number of business days that will be added to the stage activation date to automatically set a deadline on the proof.</li> 
  <li><span class="bold">Lock stage:&nbsp;</span>Select when the stage can be locked. </li> 
  <li><span class="bold">Primary decision maker:&nbsp;</span>Select the Primary decision maker on the stage. Decision makers are available&nbsp;in the drop-down list only after you add&nbsp;reviewers to the stage.</li> 
  <li><span class="bold">Only one decision required:&nbsp;</span>Select this option for the review to be&nbsp;completed after one of the decision makers makes their decision.<br>This option is not available if you designated a user in the&nbsp;<span class="bold">Primary decision maker&nbsp;</span>drop-down menu.</li> 
  <li><span class="bold">Private stage:&nbsp;</span>When this option is selected,&nbsp;comments and decisions are not visible to people who are not added to this stage or are not Supervisors, Administrators, or Billing Administrators in the account</li> 
 </ul> 
 <li value="5">(Optional) Add reviewers to the stage.</li> 
 <p>Consider the following when&nbsp;adding reviewers:</p> 
 <ul> 
  <li>A&nbsp;reviewer can be added to a proof only once. (You cannot add the same person to more than one stage on the proof.)</li> 
  <li>Reviewers who are added to a private stage can see only the stage they are added to on the proof and&nbsp;comments made in that stage.</li> 
  <li>By default, adding a user&nbsp;to a stage grants&nbsp;that user access to view the proof from the moment the proof is created.<br>The system administrator can configure the proofing system to restrict users from accessing the proof until the workflow enters the stage where the user was added. For more information, see&nbsp;<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md" class="MCXref xref">Configure sharing settings for your users</a></li> 
 </ul> 
 <li value="6">(Optional) Click <span class="bold">New stage</span>, then repeat Step 4 and Step 5 to add multiple stages to the automated workflow.</li> 
 <li value="7">Continue creating the proof by specifying the necessary information in the Organize and More settings sections on the New Proof page, as described in <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a></li> 
</ol>

## Automated Workflow diagrams

While setting up the workflow for your proof, you will notice a diagram being created. Every stage you add to your proof will appear in the diagram, clearly indicating the dependencies between the stages. Private stages are marked with a key icon.

The diagram floats, which means that it will remain visible even if you scroll down the page.

If you don't need to see the diagram, you can hide it (1).

![Diagram.png](assets/diagram-350x93.png)

## Add a stage

You can add an additional stage to a workflow you are creating or modifying.

1. If you are adding a stage to an existing proof, go to the Proof details page, as described on [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. In the `Workflow` section, click  `New stage`.  

1. Specify information for the stage as in step 4 under the Creating a Proof with an Automated Workflow section in this article. 
1. Click `Add stage`, then click  `Done`.

## Delete a stage

<ol> 
 <li value="1">Click the trash icon available in the top right corner of the stage (1). <br>The icon appears when you hover over the stage.<br><img src="assets/deleting-a-stage-350x250.png" alt="deleting_a_stage.png" style="width: 350;height: 250;"></li> 
</ol>

## Stage settings

<ul> 
 <li><span class="bold">Stage name</span>: Appears on the Workflow diagram and is included in the email notifications sent to reviewers.</li> 
 <li><span class="bold">Activate stage</span>: For each stage of your Workflow, you can decide when it should be activated. For your first stage, the following options will be available: 
  <ul> 
   <li>On proof creation&nbsp;</li> 
   <li>On a specific time and date&nbsp;</li> 
   <li>Manually&nbsp;<br></li> <note type="note">
     Only these three options are available for your first stage. The other options will become available when you add a second stage; they require you to select a parent stage.&nbsp;
   </note> 
   <li>After previous deadline is reached (requires picking a parent stage)</li> 
   <li>All decisions are Approved or Approved with changes (requires picking a parent stage)</li> 
   <li>All decisions are Approved (requires picking a parent stage)</li> 
   <li>All decisions are made (requires picking a parent stage)</li> 
  </ul></li> 
 <li><span class="bold">Deadline:</span> You can decide how the deadline should be calculated on each stage of a workflow. The options are: 
  <ul> 
   <li>From proof creation: In the deadline field (9) you can select the deadline date for the proof.</li> 
   <li>From stage activation: In the deadline dropdown you select the number of business days that will be added to the stage activation date to automatically set a deadline on the proof.</li> 
  </ul></li> 
 <li><span class="bold">Lock:</span> There are a number of options that determine when a stage can be locked. The options include: 
  <ul> 
   <li>Manual lock</li> 
   <li>Never&nbsp;</li> 
   <li>When the next stage starts&nbsp;</li> 
   <li>When all decisions are made</li> 
  </ul></li> 
</ul>

`Primary decision maker`: You set the Primary decision maker on the stage. The available decision makers appear in the list only after you've added the reviewers to the stage.

>[!NOTE]
>
>If you pick a Primary decision maker, only one decision required option will no longer be available on this stage.

* `Only one decision required`: You can enable this option on a stage. This means that the review will be completed once one of the decision makers makes their decision.
* `Privacy:` Each stage can be made private. If a stage is private, the comments and decisions won't be visible to people who are not added to this stage or are not Supervisors, Administrators or Billing Administrators in the account. For more information, see [Automated Workflow overview](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Add reviewers to a stage

<ol> 
 <li value="1">Enter a contact name or email address in the field at the bottom of each stage.</li> 
 <li value="2">Click on the green plus icon to add them.</li> 
 <li value="3">Set the role on the proof.</li> 
 <li value="4">Set the email alert.</li> 
 <li value="5">When setting up the first stage, you also have the option to change the Owner of the proof.<br> <note type="note">  
   <ul> 
    <li>A reviewer can be added to a proof only once. You cannot add the same person to more than one stage on the proof.</li> 
    <li>Reviewers who are not added to a private stage cannot see the stage on the proof or comments made in that stage.</li> 
   </ul> 
  </note></li> 
</ol>

## Convert a proofto an Automated Workflow

You can convert a basic proof to Automated Workflow.

1. Click `Convert to Automated Workflow` on the Proof details page.  
   After&nbsp;the proof is reworked to Automated Workflow, all stages are active, public and their Lock stage option is set to Manual by default. All stages remain with users and their settings.

  * Activate stage is set to On proof creation in every stage.
  * Deadline calculated from option is set to Proof creation in every stage.
  * If only one decision option was selected on the basic proof, all stages have it selected.
  * If on basic proof Primary decision maker was selected then stages with that recipient are set to them and all other have it set to None.
  * Stage name remains the same.

## Add an additional template to an existing Automated Workflow

After a basic proof is converted to Automated Workflow, you can add additional template to it.

<ol> 
 <li value="1">On the Proof details page, in the Workflow section, click <span class="bold">Add template.</span></li> <note type="note">  
  <ul> 
   <li style="font-style: normal;">Template settings determine&nbsp;what can be done with a proof to which this template was added. For example, if the template has the Add a stage and Add people to stages options disabled, buttons to add stage and share proof will not be visible. </li> 
   <li style="font-style: normal;">If Add a stage option is disabled&nbsp;in the given&nbsp;template, after adding it the Add template button are not visible. </li> 
   <li style="font-style: normal;"> <p>When a person is added to a stage in an Automated Workflow template, but also already present on the proof then if this template is applied, the system will remove this person from the stage automatically. If there is no one else added to this particular stage, the following error will be shown, as the system will not allow to add an empty stage to the workflow. </p> <p> <img src="assets/error-when-adding-template-350x66.png" alt="error_when_adding_template.png" style="width: 350;height: 66;"><![CDATA[                    ]]></p> </li> 
  </ul> 
 </note> 
</ol>

