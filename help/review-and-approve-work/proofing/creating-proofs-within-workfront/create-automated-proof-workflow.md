---
filename: create-automated-proof-workflow
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
---



# Create an advanced proof with an Automated workflow {#create-an-advanced-proof-with-an-automated-workflow}

An Automated Workflow makes it easier to manage the review process if your process is complex, or if you send content for review to the same people regularly. The *`proof`* moves from stage to stage and *`Adobe Workfront`* notifies each user when it is their turn to review it. For more information about Automated workflows, see [Automated Workflow overview](automated-workflow.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Higher</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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


## Create an advanced proof with an Automated workflow {#create-an-advanced-proof-with-an-automated-workflow-1}




1.  Go to the project, task, or issue where you want the *`proof`*, then click the `Documents` tab.
1.  Click `Add new` > *`Proof`*, upload the content, then work through the sections listed below.


   or


   Hover over an existing document, then click the `Create Proof` > `Advanced *`Proof`*` and work through the sections listed below. 





## Configure the *`proof`* Stages {#configure-the-proof-stages}




1. In the Workflow type section, choose `Automated`.
1.  (Optional) If you want to use an Automated Workflow template that your *`Workfront administrator`* created and shared with you, click `Add template`, select the template in the box that appears, then click `Add template`.


   >[!NOTE]
   >
   >Consider the following when you use an Automated Workflow template: &nbsp;    >
   >    
   >    
   >    * An Automated Workflow template's settings determine what you can do with the Automated Workflow for a *`proof`*. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the *`proof`*. 
   >    
   >    * When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the *`proof`*, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. 
   >    * Your ability to modify an Automated Workflow template depends on the template settings configured by the *`Workfront administrator`*, as described in [Create and manage Automated Workflow templates](create-manage-automated-workflow-templates.md). If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.
   >    
   >    
   >    




1. Configure the first stage of the Automated Workflow:
    
    
    1. (Optional) If you want to create a name for the first stage, click `Stage 1`, then type the name.
    1. In the `Recipients` section for the stage, add reviewers to the stage.
    
    
       >[!NOTE]
       >
       >Consider the following when&nbsp;adding reviewers to a stage:       >
       >    
       >    
       >    * You can add external users to a stage with an email address.
       >    * After you add a user to a stage, you can configure settings for that user on the *`proof`*.
       >    * You can drag users directly to another stage, or you can drag users to a stage on the `Stages` diagram. To select multiple users, press Shift+Ctrl (on Windows) or Shift+Command (on Mac).
       >    * You can add a reviewer to a *`proof`* only once, which means that you cannot add the same person to more than one stage on the *`proof`*.
       >    
       >    * Reviewers who are not added to a private stage cannot see that stage on the *`proof`* or comments made in that stage.
       >    * By default, adding a user to a stage grants that user access to view the *`proof`* from the moment the *`proof`* is created.  

       >    
       >    
       >      Your *`Workfront administrator`* can restrict users from accessing the *`proof`* until the workflow enters the stage where the user was added. For more information, see&nbsp; [Configure sharing settings for your users](configure-sharing-settings-users.md)&nbsp;in&nbsp; [Configure sharing settings for your users](configure-sharing-settings-users.md).
       >    
       >    
       >    

    
    
    
    1. Click `Stage settings`.
    1. Click an `Activate stage` option to indicate how you want the stage to activate.
    
    
       For the first stage, you can select only `On proof creation`, `On a specific date and time`, or `Manually`. 
    
    1. (Conditional) If you selected `On a specific date and time` in the previous step, select the date and time when you want to activate the stage in the `Activate on` box that appears.
    
    1. Use any of the options below to further configure the stage.
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Set stage deadline</td>
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Transfer primary decision rights to</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select the Primary decision maker on the stage (available only after you add&nbsp;at least one person to the stage who has a Proof role of Approver or higher). If you select a Primary decision maker, the <span class="bold">Only one decision required</span> option is disabled on this stage.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Require only one decision for this stage</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Ends the entire review process when one of the decision makers makes a decision.<p>This option is not available if you designated a user in the&nbsp;<span class="bold">Primary decision maker&nbsp;</span>drop-down menu.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Make this stage private</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Allows only the following people to view comments and decisions made during this stage: Supervisors, <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, and <span class="mc-variable WFVariables.AdminWFP-plur variable varname">Workfront Proof administrators</span></td>
  </tr>
 </tbody>
</table>    
    
    
    
    
1. To add and configure another stage:
    
    
    1. Click `New stage`.
    1. (Optional) If you want to create a name for the first stage, click `Stage 2` (or `Stage 3`, `Stage 4`, and so on), then type the name.
    
    1. Click the `Activate stage`, then select an option to specify whether the stage is activated automatically or manually.
    
    
       In addition to the options `On proof creation`, `On a specific date and time`, or `Manually`, you can select an option that is dependent on what occurred in the previous step: 
    
    
       ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)    
    

    
    1. If you selected an Activate stage option that is dependent on what occurred in the previous step, use the options that appear to configure the activation setting. 
    
    
       For example, if you selected `When previous stage status changes`, select the `Previous stage`, then select the status in the `Status changed to` box.
    
    
    
1.  Repeat the previous step as needed to add more stages.


   As you add stages to the Automated Workflow, a diagram forms on the screen to represent them:


   ![](assets/stages-diagram-350x213.png)








1. Continue with [Configure email settings for the proof](#configur2) below.




## Configure email settings for the proof {#configure-email-settings-for-the-proof}




1.  In the `Email notification` section, select whether to send email notifications and a custom message to&nbsp;the users you selected in [Create an advanced proof with an Automated workflow](#workflow) earlier in this article:







1.  Continue with [Configure proof settings](#configur3) below.




## Configure *`proof`* settings {#configure-proof-settings}




1.  In the `Proof settings` section, select any of the following options:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Require login - proof can only be shared with other users</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">When this option is disabled (default), anyone with the URL is able to view the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. <br>When this option is selected:
    <ul>
     <li>Only <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>&nbsp;users are able to view the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li>
     <li>Users cannot sign in to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> unless they have been added to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li>
     <li>Subscriptions cannot be enabled.</li>
    </ul></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Only one decision required for this <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span></td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">When this option is selected, the review is completed after one of the decision makers makes their decision.<br>This option is disabled by default.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Require decisions to be electronically signed</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Users are required to specify their user name and password at the time that they make a decision on&nbsp;a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Lock <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> when all required decisions are made</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">When this setting is enabled, the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.<br>This option is disabled by default.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Download original file</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">When this option is selected, reviewers are able to download the original file from which the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> was created.<br>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Share <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via public URL or embed code</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">When this option is selected, the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can be shared via a public URL or embed code.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Subscribe to <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via public URL or embed code</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">When this option is selected, people who have not been added explicitly to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. The person subscribing to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is granted the role and email that you define in the following settings:
    <ul>
     <li><span class="bold">Subscriber role:</span>&nbsp;The default <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> role that is&nbsp;assigned to all reviewers that subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.&nbsp;</li>
     <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li>
    </ul><p>
     <ul>
      <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. You can select <span class="bold">No email</span> (email link is not required to access the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via email without any verification), or <span class="bold">Validation and <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> notification emails</span> (subscriber receives a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via email and must click the link to access a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
     </ul><p>Note: &nbsp;If the <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> have Automated Workflow attached all subscriptions will generate confirmation emails to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> Owners, so they could decide which stage the person should be added to.<br></p></p></td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Create Proof`.


   *`Workfront`* begins generating a *`proof`* of the selected documents or websites. Depending on the file size and type, the lag time on a document upload can vary. Be patient as bigger files take longer to generate. You can navigate away from the page and *`Workfront`*&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.  


1.  After the *`proof`* is generated, click  `Open proof` to launch the *`proofing viewer`*.


   ![](assets/open-proof-350x132.png)




   Users who do not have *`proofing`* enabled on their account&nbsp;are still able to view the document and make comments to the proof [.](config-time-logged-hrs-days.md)  




