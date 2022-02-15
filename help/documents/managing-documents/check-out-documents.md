---
filename: check-out-documents
product-area: documents
navigation-topic: manage-documents
---



# Check out documents {#check-out-documents}

You can check out a document to prevent other users from deleting it or uploading a new version of it. Only one user can check out a document at a time. You can check out any document uploaded to *`Adobe Workfront`* as well as documents linked to third-party document providers (Box, Dropbox, Google Drive, Webdam, *`Workfront DAM`*, SharePoint, or any other custom provider).&nbsp;


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage access to the Document</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Actions allowed on&nbsp;checked out documents {#actions-allowed-on-checked-out-documents}

Users with manage access to the document&nbsp;can do the following:



* Edit&nbsp;the document (document name, description, custom data)
* Move the document
* Share the document
* Preview the document
* Download the document  


  >[!TIP] {type="tip"}
  >
  >&nbsp;Although a user can download a document when it is checked out by another user, we&nbsp;recommend that users wait until the document has been checked back in before downloading it. When a document is checked out, it often indicates that work is still being done on the document. Waiting until a document is checked back in to download it ensures the user has the most recent version.



* Approve a document or apply an approval to the document.
*  Review the document in the *`proofing viewer`*


  For more information about *`proofing`*, see [Proofing](_proofing.md)





## Check a document out {#check-a-document-out}

If you have manage permissions to a document, you can check it out to forbid&nbsp;certain actions on the document.&nbsp;



1.  Go to the area where your document is stored, then select the document.&nbsp;


   For information about adding documents, see [Add documents to Adobe Workfront from your file system](add-documents-from-file-system.md).

1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Check Out</span> icon <img src="assets/check-out-25x23.png" style="width: 25;height: 23;">. </MadCap:conditionalText>`   
   <![CDATA[ ]]>
1.  A lock icon ![](assets/lock-icon-locked-qs.png) displays to the right of the document name. The document stays checked out after you log out of *`Workfront`*.
1. Only the user who checked out the document or the *`Workfront administrator`* can check&nbsp;the document in.




## Manage checked out documents {#manage-checked-out-documents}

Consider the following about checked out documents:



* Before you can delete an object where a checked out document is stored, you must first check the document back in.&nbsp;
* If the *`Workfront administrator`* deletes a user who checked out a document they didn't own, *`Workfront`* automatically checks in the document.

* If the *`Workfront administrator`* deletes a user who checked out a document they own, and the document is uploaded on an object, the document remains checked out. Only a *`Workfront administrator`* can check it back in.

*  If the *`Workfront administrator`* deletes a user who checked out a document they own, and the document is uploaded only in the Documents area (not on an object), the document is deleted with the user. 


  For information about deleting users, see [Delete users](delete-a-user.md).

* If the *`Workfront administrator`* deactivates a user, any documents they have checked out remain checked out. Only a *`Workfront administrator`* can check them back in.&nbsp;





## Check a document in {#check-a-document-in}

You must check a document back in before you can upload a new version or delete it.&nbsp;


To check in a document:



1.  Go to the area where your document is stored and select the document.&nbsp;


   A lock icon ![](assets/lock-icon-locked-qs.png) displays to the right of the document name.

1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Check In</span> icon  <img src="assets/check-in-25x22.png" style="width: 25;height: 22;">.</MadCap:conditionalText>`   



