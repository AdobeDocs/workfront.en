---
filename: document-permissions
title: Document permissions
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
---



# Share a document in *`Adobe Workfront`* {#share-a-document-in-adobe-workfront}

Your *`Adobe Workfront administrator`* grants users access to view or edit documents when they assign access levels, as explained in [Grant access to documents](grant-access-documents.md).


The access level that the *`Workfront administrator`* grants to users allows them to either view or edit documents. In addition to this, other users can also grant others permissions to view or manage specific documents that they uploaded themselves or that they have access to share.


Permissions are specific to one item in *`Workfront`* and define what actions one can take on that item. For information about object permissions, see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md).


The user who uploads a document to *`Workfront`* has Manage permissions to it, by default.


For information about sharing an entire document folder, see [Share a document folder](share-a-document-folder.md).


## Considerations about sharing documents {#considerations-about-sharing-documents}

In addition to the considerations below, also see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md). 


>[!NOTE]
>
>A *`Workfront administrator`* can add or remove permissions to any items in the system, for all users, without being the owner of those items.





*  Sharing a document is similar to sharing any other object in *`Workfront`*. For information about how to share documents in *`Workfront`*, see [Share an object in Adobe Workfront](share-an-object.md). 
*   You can grant the following permissions to documents: 

    
    
    * View
    *   Manage
    
    






*  You can also share a document publicly or system-wide.  



  ` `**Warning: **``We recommend that you use caution when sharing an object containing confidential information with external users. This allows them to view information without being a *`Workfront`* user or part of your organization. 

*  You can share a document with someone who does not have a Workfront account, by adding their email address in the Give document access to field.
* When you share a document, users have the same access to all the document versions and all the document *`proofs`*.  
  For more information about *`proofing`* in *`Workfront`*, see the [Proofing](_proofing.md) section. 

*  You can inherit permissions to documents from the objects they are associated with. Your *`Workfront administrator`* can restrict the inheritance of permissions for documents in your access level.


  For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](create-modify-access-levels.md).  



  You can manually remove inherited permissions on documents.  
  For more information about removing inherited permissions from objects, see [Remove permissions from objects in Adobe Workfront](remove-permissions-from-objects.md)  






## Document permissions {#document-permissions}

The following table displays what permissions you can grant users when allowing them to view or manage documents:

<table style="height: 461px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" border="2" cellspacing="15" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Action</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Manage</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">View</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Create</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Edit Document Details</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Delete*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Download</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Checkout</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Add Approvers</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Approve Document</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Attach Custom Form</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Edit Custom Fields</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Move to (object)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Send To (integration)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Updates/ Comments</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Upload new version</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Delete Version</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">View Document(s)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Preview</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Proof**</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Generate Proof**</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Remove Proof**</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Share*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Share System-wide*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Share Documents Publicly*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Share with an external email address</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;"> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Add/ Remove</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Rename</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Link (with integration)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Unlink (with integration)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="text-align: center;">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray" style="text-align: center;"> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Action is shared by both Documents and Document Folders.


&#42;&#42; You must have a separate *`proofing`* license associated with your *`Workfront`* account to be able to *`proof`* documents. Contact your account manager about acquiring a *`proofing`* license. For more information about *`proofing`* in *`Workfront`*, see [Proofing](_proofing.md). 
