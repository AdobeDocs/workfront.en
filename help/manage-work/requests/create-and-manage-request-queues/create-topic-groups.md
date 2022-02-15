---
filename: create-topic-groups
product-area: requests
navigation-topic: create-and-manage-request-queues
---



# Create Topic Groups {#create-topic-groups}

Topic Groups are associated with Request Queues. They allow you to layer your Request Queues in multiple categories, depending on the nature of the requests. 



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
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


## Overview of Topic Groups {#overview-of-topic-groups}

For example, if you have a Request Queue for Marketing Requests, you can have a Topic Group of "Mother's Day Campaign", with a second-level Topic Group of "Digital Media", and an additional second-level Topic Group of "Print Media." Then, you can have multiple Queue Topics inside each Topic Group. For example, "Banner Ad" and "Blog" can be Queue Topics for the "Digital Media" Topic Group. 


For more information about how to create Request Queues, see [Create a Request Queue](create-request-queue.md).

` `**Tips: **`` 


* You can create up to 10 tiers of Topic Groups within a Request Queue.
* There is no limit to the number of Queue Topics that can be associated with a topic group. 
* Topic groups are a reportable object.




## Create Topic Groups {#create-topic-groups-1}

We recommend that you create Topic Groups before you create a Queue Topic. However, a Topic Group can be created within in the Queue Topic builder. For more information about creating Queue Topics, see [Create Queue Topics](create-queue-topics.md).


To create a Topic Group:



1.  Go to the project that you published as a Help Request Queue.  
   For more information about publishing a project as a Help Request Queue, see [Create a Request Queue](create-request-queue.md).

1.  Click `Topic Groups` in the left panel. You might need to click `Show More`, then `Topic Groups`. 
1.  Click `New Topic Group`.  
   ![](assets/10-350x170.png)


1.  Specify the following information: 
    
    
    * `Name`: The name is visible to users who submit requests to this request queue. 
    * `Description`: The description displays when users select the topic group in the process of submitting a new request. 
    * `Add to Topic Group`: You can add the new Topic Group to an existing Topic Group, or you can add it directly to the project published as a Help Request Queue. 
    
    
1.  Click `Save`.  
   This creates a new Topic Group in your Request Queue. You can now select additional categories from the first drop-down menu under a Request Queue.  
   For more information about submitting requests, see [Create and submit Adobe Workfront requests](create-submit-requests.md).



