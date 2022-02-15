---
filename: share-a-template
title: Share a template
product-area: templates
navigation-topic: grant-and-request-access-to-objects
---



# Share a template overview {#share-a-template-overview}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


As an *`Adobe Workfront administrator`*, you can grant users access to view or edit templates when you assign their access level. A user must have a Plan license to have access to Edit templates.  



For more information about granting access to templates, see [Grant access to templates](grant-access-templates.md).


Along with the access level that you grant, a user can also receive permissions to View or Manage specific templates from other users who share them .


>[!NOTE]
>
>Permission levels work within Access levels. For example, a user cannot receive permissions to Manage a template, if their access level only allows them to View templates.


Permissions are specific to one item in *`Workfront`* and define what actions one can take on that item.  



## Considerations when sharing a template {#considerations-when-sharing-a-template}




* In addition to the considerations below, also see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md).
* The creator of a template, as well as the Template Owner have Manage permissions to the template, by default. For information about designating a user as the Template Owner, see [Edit project templates](edit-templates.md).
*  You can share the following when sharing a template:

    
    
    *  The template
    
    
      For more information about how to share a template, see [Share project templates](share-project-template.md).
    
    
      You can grant the following permissions to a template:
    
        
        
        *  View
        
        
          ![](assets/view-on-template-262x221.png)        
        

        
        *  Manage
        
        
          ![](assets/manage-on-template-225x280.png)        
        

        
        
        
    
    *  The future projects which are created using the template. You can give the same levels of permissions to projects created from a template as you would an individual project.&nbsp;
    
    
      For information about how to share a project from a template at the template level, see [Share project templates](share-project-template.md). 
    
    
    

*  When you share a template or a project which is created from the template, users inherit the same permissions to all the children objects associated with the template or the project, by default.


  For more information about the hierarchy of objects in *`Workfront`*, see&nbsp; [Understand objects in Adobe Workfront](understand-objects.md).

*  When you share a template, all the template tasks and documents, as well as the issues on the future project created from the template inherit the same permissions, unless otherwise specified.


  For information about managing the access to template tasks and issues on the project based on a user's permissions to the project, see the [Access](edit-templates.md#access) section in the article [Edit project templates](edit-templates.md).

* The *`Workfront administrator`* can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](create-modify-access-levels.md).





## Advanced Settings for template sharing {#advanced-settings-for-template-sharing}

The following table displays what permissions you can grant users when allowing them to View or Manage a template. For the instructions on sharing a template, see the section [Share a template](share-project-template.md#share) in the article [Share project templates](share-project-template.md).

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Actions</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Manage</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">View</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Copy</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Delete</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Edit Template Details</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">View Template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Share</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Share System-wide</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p><span class="preview">Add Documents</span> </p> <p>Tip: <span class="preview">Sometimes people add documents to a project template thinking that they’re adding them to a project. You can prevent this for your recipients by disabling this setting.</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"><span class="preview">✓</span> </td> 
  </tr> 
 </tbody> 
</table>

To understand the permissions you are granting users to projects that are created from a template, see [Share a project in Adobe Workfront](share-a-project.md).
