---
filename: define-request-types-for-project
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
---



# Define Request Types for a project in *`Adobe Workfront`* {#define-request-types-for-a-project-in-adobe-workfront}

You can organize the kind of issues or requests that are logged in *`Adobe Workfront`* by Request Types. 


This organization is useful for reporting reasons and for helping users understand what kind&nbsp;of unexpected work&nbsp;might occur during the lifetime of a project.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you begin, you must



*  Have or create a project


  For information about creating projects, see [Create a project](create-project.md). 





## Considerations about Request Types {#considerations-about-request-types}




*  You can specify the type of issues or requests that can be logged on a project when you configure the `Queue Details`&nbsp;area for the project.
*  You don't have to enable the project to be a request queue to be able to define Request&nbsp;Types for a project. Any issues logged for a project can be labeled with a different Request&nbsp;Type. 
*  If you add Queue Topics to your project, you must define Request&nbsp;Types on each queue topic to display it when adding a new issue or request. For more information, see [Create Queue Topics](create-queue-topics.md). 




## Define the issue or request types for a project {#define-the-issue-or-request-types-for-a-project}




1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Projects</span> in the Main Menu.  <img src="assets/main-menu-icon.png"></MadCap:conditionalText>` 
1. Click the name of the project to open it.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the left panel, click  <span class="bold">Queue Details</span>.</MadCap:conditionalText>` 
1.  In the `Queue Properties` section, select the `Request Types` you want for the project.


   >[!NOTE]
   >
   >You must have at least one request type selected. You can select multiple request types.


   Select from the following types:

    
    
    * Bug Report
    * Change Order
    * Issue
    * Request
    
    


   >[!TIP] {type="tip"}
   >
   >Your *`Workfront administrator`* might have renamed some of these options. For information, see [Configure request types](configure-request-types.md). 



1.  Click `Save`.


   The request types you specified&nbsp;will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project, if the project is enabled as a request queue.



