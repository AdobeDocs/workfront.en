---
filename: setup-asset-essentials
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configure the Experience Manager Assets Essentials integration
description: Connect your work with your content in Experience Manager Assets Essentials:
---

# Configure the `Experience Manager Assets Essentials` integration

Connect your work with your content in `Experience Manager Assets Essentials`​:

* Push assets and metadata from `Adobe Workfront` to `Experience Manager Assets Essentials`​
* Link assets from `Experience Manager Assets Essentials` to your projects and tasks in `Workfront`​
* Facilitate versioning workflows for assets pushed to `Experience Manager Assets Essentials`

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> licenses*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have <span>Experience Manager Assets Essentials</span>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For information on <span>Workfront administrators</span>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Set up the integration

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</p> </li> 
 <li value="2"> <p>Select <img src="assets/document-icon.png"> <span class="bold">Documents</span> in the left panel, then select <span class="bold">Experience Manager Integration</span>.</p> </li> 
 <li value="3"> <p>Select <span class="bold">Add Experience Manager Integration</span>.</p> </li> 
 <li value="4"> <p>Specify the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td>Enter the name you want users to see in the Add new button in the Documents area.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Navigation&nbsp;URL</td> 
     <td>The system automatically populates the Navigation URL. This URL is used to link to your organization's <span>Assets Essentials</span> instance from the Main Menu for quick access.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">IMS&nbsp;Org</td> 
     <td> <p>The system automatically populates your IMS Org. You can modify this field if desired.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>(Optional) Set up metadata mapping:</p> <p>Documents with the native or custom fields automatically map to the specified fields the first time an asset is sent to <span>Experience Manager Assets Essentials</span>:</p> 
  <ol> 
   <li value="1"> <p>In the <span class="bold">Workfront Source Field</span> column, choose a native or custom <span>Workfront</span> field.</p> </li> 
   <li value="2"> <p>In the <span class="bold">Experience Manager Target Field</span>, choose an <span>Experience Manager Assets Essentials</span> field. </p> </li> 
   <li value="3"> <p>Repeat steps a. and b. as needed.</p> <note type="note">
     You can map metadata only in one direction: from 
     <span>Workfront</span> to 
     <span>Assets Essentials</span>. Metadata for documents linked to 
     <span>Workfront</span> from 
     <span>Assets Essentials</span> cannot be transferred to 
     <span>Workfront</span>.
    </note> </li> 
  </ol> </li> 
 <li value="6"> <p>Select <span class="bold">Save</span>.</p> </li> 
</ol>

