---
filename: delete-templates
product-area: templates
navigation-topic: templates-navigation-topic
title: Delete project templates
description: We recommend that you deactivate templates that you are no longer using, instead of deleting them so that you can keep historic information about your projects over time. For information about deactivating a template, see Edit project templates.
---

# Delete project templates

We recommend that you deactivate templates that you are no longer using, instead of deleting them so that you can keep historic information about your projects over time. For information about deactivating a template, see [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>When you delete a template, the projects that are using that template are not modified in any way. However, you can no longer see the name of the original template in the Template field on the project. Additionally, you can no longer view the names of the template tasks for the tasks on the project in a task view. The Template field on the project and the Template Task field on the tasks remain blank after the template originally associated with the project is deleted.

##

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations for deleting templates

* The tasks which were added to projects when the template was attached remain on the projects. However, the template task information associated with the tasks is deleted. 
* The name of the template is no longer listed in the `Template` field on the `Overview` sub-tab of the project. 

* You can recover a recently deleted template from the Recycle Bin. For information about recovering items from the Recycle Bin, see [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Delete a template

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From the 
    <span class="bold">Main Menu</span>
    <img src="assets/main-menu-icon.png"> click 
    <span class="bold">Templates</span>. This opens a list of templates
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   From the 
   <span class="bold">Main Menu</span>
   <img src="assets/main-menu-icon.png"> click 
   <span class="bold">Templates</span>. This opens a list of templates
  </MadCap:conditionalText></li> 
 <li value="2"> <p>Select the template that you want to delete by clicking the checkbox to the left of the template name, then click <span class="bold">Delete > Yes, Delete It</span> to confirm the deletion.</p> <p>Or</p> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the name of a template to access it, then click the 
     <span class="bold">More</span> menu 
     <img src="assets/qs-more-icon-on-an-object.png"> , then 
     <span class="bold">Delete Template > Yes, Delete it</span>. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the name of a template to access it, then click the 
    <span class="bold">More</span> menu 
    <img src="assets/qs-more-icon-on-an-object.png"> , then 
    <span class="bold">Delete Template > Yes, Delete it</span>. 
   </MadCap:conditionalText></p> <p>The template is no longer available to be associated with a project. </p> </li> 
</ol>

