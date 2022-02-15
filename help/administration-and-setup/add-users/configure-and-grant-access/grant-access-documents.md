---
filename: grant-access-documents
title: Grant access to documents
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
---



# Grant access to documents {#grant-access-to-documents}

As an *`Adobe Workfront administrator`*, you can use an access level to define a user’s access to *`documents`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></MadCap:conditionalText>`, as explained in [Access levels overview](access-levels-overview.md).&nbsp;


The access a user receives for documents in their access levels also applies to document folders.


>[!NOTE]
>
>When someone shares a *`document`* with another user, the recipient’s rights on it are determined by a combination of two things:
>
>
>
>* The recipient’s access level setting for *`documents`*
>* Any permissions that the sharer granted for the *`document`* 
>
>
>For information about permissions users can grant on a document when sharing it, see [Share a document in Adobe Workfront](document-permissions.md).





##  

For information about using custom access levels to manage users' access to objects in *`Workfront`*, including *`documents`*, see&nbsp; [Create or modify custom access levels](create-modify-access-levels.md).


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



## Configure user access to documents using a custom access level {#configure-user-access-to-documents-using-a-custom-access-level}




1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](create-modify-access-levels.md).
1.  Click the gear icon ![](assets/gear-icon-settings.png) on the `View` or `Edit` button to the right of *`Documents`*, then select the abilities you want to grant under **Fine-tune your settings**.


   ![document_access.png](assets/document-access-350x171.png)




   You can allow users to do the following on projects, tasks, and issues that they have access to:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Create</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Upload documents.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Delete</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Remove uploaded documents.</p> <p>The <b>Create</b> option is automatically enabled when this option is enabled.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Share</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Share documents with specific users, job roles, teams.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Share Documents Publicly</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Share documents with external users (don't have a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license).</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Share System-wide</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Make documents available to everyone in your Workfront instance.</p> <p>Anyone in the system can see a document shared this way if:</p> 
    <ul> 
     <li> <p>You send them a link to the Documents page where it's uploaded.</p> </li> 
     <li> <p>They search for it in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></p> </li> 
    </ul> <p>The <b>Share</b> option is automatically enabled when this option is enabled.</p> </td> 
  </tr> 
 </tbody> 
</table>



   >[!NOTE]
   >
   >Users don’t inherit access to objects from higher-ranking objects. For example, you can restrict a user from deleting *`projects`* in their access level, but this does not restrict them from deleting *`documents`*, which are lower-ranking than *`projects`*. For more information about the hierarchy of objects, see the section [Interdependency and hierarchy of objects](understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in&nbsp;the article [Understand objects in Adobe Workfront](understand-objects.md).
   >
   >
   >For more information about the hierarchy of objects, see the section [Interdependency and hierarchy of objects](understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in&nbsp;the article [Understand objects in Adobe Workfront](understand-objects.md).




1.  (Optional) To restrict inherited permissions for documents from higher ranking objects, click `Set additional restrictions`, then select `Never inherit document access from projects, tasks, issues, etc`.
1.  (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](_configure-access.md), such as [Grant access to tasks](grant-access-tasks.md) and [Grant access to financial data](grant-access-financial.md).
1.  When you are finished, click **Save**.


   After the access level is created, you can assign it to a user. For more information, see [Edit a user's profile](edit-a-users-profile.md).  






## Document access by license type {#document-access-by-license-type}

This table lists what a *`Workfront administrator`* can allow users with each license type to do with *`documents`*. For information about the *`Workfront`* license types, see [Adobe Workfront licenses overview](wf-licenses.md).

&#42;&#42; This action is shared by both documents and document folders.


&#42; This action is available only to document folders.
