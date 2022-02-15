---
filename: grant-access-resource-management
title: Grant access to Resource Management
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
---



# Grant access to Resource Management {#grant-access-to-resource-management}

As an *`Adobe Workfront administrator`*, you can use an access level to define a user’s access to *`Resource Management`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></MadCap:conditionalText>`, as explained in [Access levels overview](access-levels-overview.md).&nbsp;


>[!NOTE]
>
>When someone shares an object with another user, the recipient’s rights to budget or view resource allocation on it are determined by a combination of 3 things:
>
>
>
>* The recipient’s access level setting for Resource Management
>* The user’s access to financial data, as explained in [Grant access to financial data](grant-access-financial.md)
>* Any permissions to financial data that the sharer granted for the object
>
>
>For information about permissions users can grant to financial data on an object when sharing the object, see [Share financial permissions on an object in Adobe Workfront](share-financial-permissions-object.md).





## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Configure user access to Resource Management tools using a custom access level {#configure-user-access-to-resource-management-tools-using-a-custom-access-level}




1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](create-modify-access-levels.md).
1.  Click the gear icon ![](assets/gear-icon-settings.png) on the `View` or `Edit` button to the right of *`Resource Management`*, then select the abilities you want to grant under **Fine-tune your settings**.


   ![](assets/resource-management-details-of-edit-in-the-access-level-350x68.png)



<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Edit priorities and budget hours in the Planner</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allows users with this license to do the following:</p> <p>Prioritize projects in the Resource Planner.</p> <p>Budget allocation for resources in the Resource Planning tools (the Resource Planner and the Resource Budgeting section in the Business Case of a project.)</p> <p>This option is enabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Manage Resource Pools</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Allows users with this license to create, edit, and delete Resource Pools. This option is disabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span>Update Planned Hours in the Workload Balancer</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Allows users with this license to update the Planned Hours of work items when they update the user allocations in the Workload Balancer. The total number of allocated hours becomes the Planned Hours of the work items.</p> <p>This option is disabled by default.</p> <p> For more information, see <a href="manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](_configure-access.md), such as [Grant access to tasks](grant-access-tasks.md) and [Grant access to financial data](grant-access-financial.md).
1.  When you are finished, click **Save**.


   After the access level is created, you can assign it to a user. For more information, see [Edit a user's profile](edit-a-users-profile.md).





## Access to Resource Management by license type {#access-to-resource-management-by-license-type}

This table lists what a *`Workfront administrator`* can allow users with each license type to do with *`Resource Management`*. For information about the *`Workfront`* license types, see [Adobe Workfront licenses overview](wf-licenses.md).


Only users with a *`Plan`* license can have full access to *`Resource Management`*. Other license types can have limited or no access to Resource Management in *`Workfront`*. The Request and External User license types are not included here because they don't have access to *`Resource Management`*.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Action</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Planner</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Worker</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Reviewer</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Budget resources in the Resource Planning tools*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Create, edit, delete Resource Pools*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Attach Resource Pools to projects, templates, and users</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">View project priorities in the Resource Planner</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> ✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">View resource allocation in the Resource Planning tools</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> ✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">View Resource Pools</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> ✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span>Update Planned Hours in the Workload Balancer</span>**</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span>✓</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

&#42;These actions require additional access to Financial Data and permissions to project finances. If you grant Resource Management access to a Planner user who doesn't have access to Financial Data, the user can still see the hourly allocations in the Resource Planner, but can't switch to Cost view or view the Business Case. For more information, see [Grant access to financial data](grant-access-financial.md) and [Share financial permissions on an object in Adobe Workfront](share-financial-permissions-object.md).


&#42;&#42;This action requires permission to Contribute to the object, with Make Assignments enabled under Advanced Settings. For information, see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md).
