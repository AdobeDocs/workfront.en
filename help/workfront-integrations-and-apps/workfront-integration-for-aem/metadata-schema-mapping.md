

# `Workfront Tools for AEM User Guide : Metadata Schema Mapping`

## Asset Metadata Mapping

Metadata mapping between Adobe Workfront Documents and AEM Assets is defined within AEM Metadata Schemas. Metadata Schemas should be created and configured as usual in AEM. Workfront Tools adds configuration options to the Settings configuration tab of each metadata schema form field. These options will allow you to specify to which Workfront field each AEM property should be mapped to.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> <!--
   Adobe Workfront license* Work or higher
  --> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have a license to Adobe Experience Manager</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

* You must install Workfront Tools for Adobe Experience Manager before you can map metadata schemas.

  For instructions, see [Workfront Tools for AEM User Guide: Installation Guide 1.x.x](../../workfront-integrations-and-apps/workfront-integration-for-aem/installation-guide.md)

## Configure metadata schema mappings

Follow these steps to configure the mappings:

<ol> 
 <li value="1"> <p>Navigate to <span class="uitext">Tools → Assets → Metadata Schemas</span>.</p> <p> <img src="assets/metadata-schema-350x242.png" style="width: 350;height: 242;"> </p> </li> 
 <li value="2"> <p>Select the metadata schema form you wish to edit and click <span class="uitext">Edit </span>or create a new metadata schema from scratch.</p> <p> <img src="assets/edit-schema-350x242.png" style="width: 350;height: 242;"> </p> </li> 
 <li value="3"> <p>Select the metadata schema form field you wish to edit and select <span class="uitext">Settings </span>tab on the right panel.</p> </li> 
 <li value="4"> <p>In <span class="uitext">Workfront Custom Form Field</span> select the name of the Workfront field that you wish to map to the selected AEM property. Available options are:</p> 
  <ol> 
   <li value="1"> <p>Document custom form fields</p> </li> 
   <li value="2"> <p>Project custom form fields</p> </li> 
   <li value="3"> <p>Issue custom form fields</p> </li> 
   <li value="4"> <p>Task custom form fields</p> </li> 
   <li value="5"> <p>Project Overview fields (ID, Name, Description or Reference Number)&nbsp;</p> </li> 
  </ol> </li> 
 <li value="5"> <p>In the case where the Workfront field selected in <span class="uitext">Workfront Custom Form Field</span> is a Workfront User type-ahead field, it will be necessary to specify which Workfront User field you wish to map. To do so, check <span class="uitext">Get value from Workfront referenced object field</span> and then specify the name of the Workfront User Custom Form Field from which to retrieve the value to be mapped.</p> <p> <img src="assets/metadata--project-id-schema-350x242.png" style="width: 350;height: 242;"> </p> </li> 
</ol>

## Folder Metadata Mapping

Metadata mapping between Workfront Projects and AEM Folders is defined within AEM Folder Metadata Schemas. Folder Metadata Schemas should be created and configured as usual in AEM. Workfront Tools adds an autocomplete dropdown to the Settings configuration tab of each folder metadata schema form field. This autocomplete drop-down menu will allow you to specify to which Workfront field each AEM folder property should be mapped to.

Follow these steps to configure the mappings:

<ol> 
 <li value="1"> <p>Navigate to <span class="uitext">Tools → Assets → Folder Metadata Schemas</span>.</p> <p> <img src="assets/folder-schema-mapping-350x242.png" style="width: 350;height: 242;"> </p> </li> 
 <li value="2"> <p>Select the folder metadata schema form you wish to edit and click <span class="uitext">Edit</span>.</p> <p> <img src="assets/edit-folder-schema-350x104.png" style="width: 350;height: 104;"> </p> </li> 
 <li value="3"> <p>Select the folder metadata schema form field you wish to edit and select <span class="uitext">Settings </span>tab on the right panel.</p> </li> 
 <li value="4"> <p>In <span class="uitext">Mapped from Workfront Field</span> select the name of the Workfront field that you wish to map to the selected AEM folder property. Available options are:</p> 
  <ol> 
   <li value="1"> <p>Project custom form fields</p> </li> 
   <li value="2"> <p>Project Overview fields (ID, Name, Description, Reference Number, Planned Completion Date, Project Owner, Project Sponsor, Portfolio or Program)&nbsp;</p> </li> 
  </ol> <p> <img src="assets/folders---project-id-schema-350x242.png" style="width: 350;height: 242;"> </p> </li> 
</ol>

