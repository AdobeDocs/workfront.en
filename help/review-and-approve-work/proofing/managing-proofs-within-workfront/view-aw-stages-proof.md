---
filename: view-aw-stages-proof
product-area: documents
navigation-topic: manage-proofs-within-workfront
---



# View Automated Workflow stages on a *`proof`* {#view-automated-workflow-stages-on-a-proof}

You can conveniently track the progress of a *`proof`* configured with an Automated Worklow. You can view, modify, add, start, and lock the work already done on stages on the *`proof`*.


For information about adding stages and users to a proof with an Automated Workflow, see [Add stages and users to an Automated Workflow on a proof](add-stages-users-to-automated-workflow-proof.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Current plan: <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span></p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.proofPermissionProfile variable varname">Proof Permission Profile</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Manager or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## View the Automated Workflow diagram {#view-the-automated-workflow-diagram}




1.  In a document list that contains the document, hover over the row containing the document, then click `Proofing Workflow`.


   The diagram for the Automated Workflow displays just below the Workflow title.


   The stages on the diagram are marked as follows:


   ![dot.png](assets/dot.png) Active stage


   ![grey_dot.png](assets/grey-dot.png) Inactive stage  
   ![sbw-key-icon.png](assets/sbw-key-icon.png)&nbsp; Private stage


   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)&nbsp; Locked stage


   The lines between the stages depict the dependencies between the stages. The lines leading to inactive stages are dotted until the stage is activated.


   You can hover over a stage in the diagram to display its progress. If the stage is not active and you have edit rights on the stage, you can click the Activate stage button ![](assets/activate-stage-btn.png) to start the stage. If the stage is active and you have edit rights on the stage, you can lock it. ![](assets/lock-stage-btn.png) For more information about the Progress bar (S, O, C, D) , see&nbsp; [View the Progress and Status of a Proof in Workfront Proof](view-progress-and-status-of-proof.md).





## View a stage {#view-a-stage}




1. In a document list that contains the document, hover over the row containing the document, then click `Proofing Workflow`.
1.  On the diagram, click the stage that you want to view.


   ![](assets/view-stage-diagram-350x204.png)



1.  To expand the details for a stage, click the sideways arrow below its name.


   ![](assets/stage-details-caret-350x167.png)







## View all stages {#view-all-stages}

To view all stages in an Automated Workflow:



1.  Click the Change View button at t the top of the page ![](assets/change-view-btn.png), then click `View all stages`.


   All of the stages of the Automated Workflow are listed in the section, however the details are hidden.

1.  To expand the details of a stage, click the sideways arrow below its name.




## View all stages in detail {#view-all-stages-in-detail}

To view all stages of your Automated Workflow with their details expanded:



1.  Click the Change View button at t the top of the page ![](assets/change-view-btn.png), then click `View all stages in detail`.
1. To view the details of a stage, click the down arrow below its name.


