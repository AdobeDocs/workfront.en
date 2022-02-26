---
filename: set-up-metadata-mapping
title: Set up metadata mapping
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Set up metadata mapping
description: Metadata is descriptive information associated with a document. You can set up Adobe Workfront to include metadata with documents sent to Workfront applications.
---

# Set up metadata mapping

Metadata is descriptive information associated with a document. You can set up *Adobe Workfront* to include metadata with documents sent to *Workfront* applications.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## About *Workfront* metadata

Metadata for documents in *Workfront* can include information such as the related project name, task description, or Planned Completion Date. As a *Workfront administrator*, you can configure *Workfront* to include metadata with documents sent from *Workfront* to the following *Workfront* applications:

* *Workfront Library* 
* *Workfront DAM*

Before metadata can be sent with documents, you must first specify, or map, the metadata that you want included. You can map any field used in *Workfront*. Once you set up metadata mapping, all documents uploaded to a *Workfront* application will include the mapped metadata.

When a user sends a document from *Workfront* to a *Workfront* application, mapped metadata is transferred along the document. While the version of the document in the *Workfront* application is linked to *Workfront*, changes made to the document's metadata in *Workfront* are not reflected in the metadata of the document in the *Workfront* application. If a mapped field in *Workfront* is changed, you must send a new version of the document with the updated metadata to the *Workfront* application.

>[!NOTE]
>
>You can map metadata only in one direction: from *Workfront* to *Workfront DAM* or *Workfront Library*. Metadata for documents linked to *Workfront* from *Workfront Library* or *Workfront DAM* cannot be transferred to *Workfront*.

You can map the same *Workfront* field to various metadata fields in *Workfront Library* or *Workfront DAM*, but you cannot use a metadata field in either of those applications for multiple *Workfront* metadata fields.

To configure multiple *Workfront* fields to export to one metadata field in a *Workfront* application, first create a calculated custom field in *Workfront* to display all the individual custom fields of an object. Then, map the calculated *Workfront* field to a metadata field in the *Workfront* application. For more information about calculated custom fields, see [Add calculated data to a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Before you can map fields for the metadata mapping process, you must enable the application in *Workfront* . For more information, see [Configure document integrations](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configure *Workfront* to send metadata

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> <p> In the left panel, click <span class="bold">Documents</span> > <span class="bold">Metadata Mapping</span>. </p> <p> <img src="assets/metadata-mapping-350x193.png" style="width: 350;height: 193;"> </p> </li> 
 <li value="3"> In the <span class="bold">Select Source Field for Mapping</span> box, begin typing the name of the <em>Workfront</em> field you want to map to <em>Workfront Library</em> or <em>Workfront DAM</em>, then select it when you see it in the list.</li> 
 <li value="4">In the <span class="bold">Select Target Field for Mapping</span> box, select the field you want to populate with the information in the selected <em>Workfront</em> field.<br></li> 
 <li value="5"> <p>Click <span class="bold">Add Mapping</span>.</p> <p>The mapped field displays in the mapped fields listed at the bottom of the page.</p> </li> 
 <li value="6">Repeat Steps 5 and 6 until you add all the desired <em>Workfront</em> fields and their corresponding <em>Workfront Library</em> or <em>Workfront DAM</em> fields.</li> 
</ol>

## Delete mapped fields

<ol> 
 <li value="1">Log in to <em>Workfront</em> as the administrator.</li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="3">In the left panel click <span class="bold">Documents</span> > <span class="bold">Metadata Mapping</span>.</li> 
 <li value="4">In the list of mapped fields, select the fields you want to remove from metadata mapping.</li> 
 <li value="5"> <p>Click <span class="bold">Delete</span>.</p> <p>The designated fields are no longer mapped. Now when a user sends a document from <em>Workfront</em> to <em>Workfront Library</em> or <em>Workfront DAM</em>, the metadata contained within the deleted fields is not transferred with the document. </p> <p>A document sent prior to you deleting the mapped fields retains the original metadata sent with it, including the metadata for the deleted fields.</p> </li> 
</ol>

