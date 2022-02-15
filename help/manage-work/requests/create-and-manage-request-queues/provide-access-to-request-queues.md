---
filename: provide-access-to-request-queues
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
---



# Provide access to request queues {#provide-access-to-request-queues}

When you provide access to a request queue, you determine who in your organization can view the request queue in the Requests area of *`Adobe Workfront`*. 


You can provide different users access to a Request Queue, depending on whether they are part of the project team, project group, or project company. You can also provide access to everyone in the system to a request queue.&nbsp;


This is useful in organizations that invite external stakeholders into *`Workfront`* and wish to limit the access of users to specific areas — in this case a request queue open just to the users associated with the company or group of the project limits visibility to external stakeholders. Giving access to anyone makes the request visible to both internal and external stakeholders. 



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


## Prerequisites {#prerequisites}

Before the request queue is available for users in the Requests area, you must create a project with the following settings: 



*  Designate it as a request queue. For more information about creating a Request Queue, see [Create a Request Queue](create-request-queue.md).
*  Update the Status of the project to Current.




## Provide access to a Request Queue {#provide-access-to-a-request-queue}




1.  Go to the project where you want to provide access to the request queues. 


   >[!NOTE]
   >
   >Only projects with a status of Current are visible in the Requests area. 



1.  Click  `Queue Details` in the left panel. You might need to click  `Show More`, then `Queue Details`. 
1.  Select `Publish as Help Request Queue`&nbsp;to designate the project as a Request Queue.
1.  Select from the following options:

    
    
    * `Anyone`: Any user can view and add requests to the request queue.
    * `People with view access to this project`:&nbsp;Users that have View permissions to the project can view and add requests to the request queue.&nbsp;
    * `People in this project's company`:&nbsp;Users associated with the project's Company&nbsp;can view and add requests. The Company associated with the project is listed in parentheses next to this option.&nbsp;
    *  `People in this project's group`:Users associated with the project's Group can view and add requests. The Group&nbsp;associated with the project is listed in parentheses next to this option.
    
    
      Group queues are useful when several departments share a *`Workfront`* account to achieve unique organizational goals. Each department may have its own queues that members of other groups should not be able to see.
    
    
      For information about who has permissions on a project see [Share a project in Adobe Workfront](share-a-project.md).  
      Groups and companies can be associated with the project when editing the project. For more information about editing projects, see [Edit projects](edit-projects.md).
    
    
    

1. Click `Save`.


