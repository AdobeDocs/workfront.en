---
filename: create-routing-rules
product-area: requests
navigation-topic: create-and-manage-request-queues
---



# Create Routing Rules {#create-routing-rules}

Routing Rules control what *`Adobe Workfront`* does with issues when they are submitted to a Request Queue. For more information about creating Request Queues, see [Create a Request Queue](create-request-queue.md).


Routing Rules send issues to specific users or job roles best equipped&nbsp;to resolve the submitted issue or request. Routing rules are usually associated with queue topics,&nbsp;which are used to control which routing rule will be applied to the issue or request.



## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*


## Create a Routing Rule {#create-a-routing-rule}




1. Go to the project which you want to add the routing rules for your requests. 
1.  Click `Routing Rules` in the left panel. You might need to click `Show More`, then  `Routing Rules`.
1. Click `New Routing Rules`&nbsp;to add the new rule.&nbsp; 
1.  Specify the following information for the Routing Rule:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 175px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <thead> 
  <tr> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadH-Column1-">&nbsp;</th> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadG-Column2-">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Name</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The name of the&nbsp;Routing Rule. You can see the Routing Rule if you have access to see this information on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Description</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Add a description for the Routing Rule.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Default Assignee*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Add an active user or <span>an </span><span data-mc-edit-date="2021-05-27T11:52:45.4165986-04:00" data-mc-editor="alinawilson" data-mc-comment="yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-05-25T13:04:12.7687137-04:00">active</span> job role&nbsp;to whom the new issues should be assigned. You can only have one default assignee in this field. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Default Team*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Add an active team to whom the new issue should be assigned. You can only have one team assigned to the issue. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Route to Project</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">This is the project where the issue is added.</td> 
  </tr> 
 </tbody> 
</table>



   >[!NOTE]
   >
   >&#42;If a user, `job role`, or team are deactivated after they are associated with a routing rule, the requests continue to be routed to them. You must periodically take an inventory of all routing rules and replace deactivated assignments with active ones. 


   When you route an issue to a project, users with permissions on the issue receive the permissions set on that project. For information about setting permissions on projects, see [Share a project in Adobe Workfront](share-a-project.md).

1. Select `Save`&nbsp;when done.  
   This process only defines the Routing Rule. To ensure that the issue is routed when it is submitted to the Request Queue, you must select the routing rule on the `Queue Details` tab under  `Default Route`. For information about adding a Default Route to a Request Queue, see [Create a Request Queue](create-request-queue.md).  
   If you want to associate multiple routing rules with the Request Queue, you must create multiple Queue Topics and associate each one with a separate Routing Rule. For more information about creating a queue topic, see [Create Queue Topics](create-queue-topics.md).



