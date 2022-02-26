---
filename: setup-asset-essentials
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configure the Experience Manager Assets Essentials integration
description: Connect your work with your content in Experience Manager Assets Essentials:
---

# Configure the *Experience Manager Assets Essentials* integration

Connect your work with your content in *Experience Manager Assets Essentials*​:

* Push assets and metadata from *Adobe Workfront* to *Experience Manager Assets Essentials*​
* Link assets from *Experience Manager Assets Essentials* to your projects and tasks in *Workfront*​
* Facilitate versioning workflows for assets pushed to *Experience Manager Assets Essentials*

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> licenses*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have <em>Experience Manager Assets Essentials</em>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Set up the integration

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</p> </li> 
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
     <td>The system automatically populates the Navigation URL. This URL is used to link to your organization's <em>Assets Essentials</em> instance from the Main Menu for quick access.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">IMS&nbsp;Org</td> 
     <td> <p>The system automatically populates your IMS Org. You can modify this field if desired.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>(Optional) Set up metadata mapping:</p> <p>Documents with the native or custom fields automatically map to the specified fields the first time an asset is sent to <em>Experience Manager Assets Essentials</em>:</p> 
  <ol> 
   <li value="1"> <p>In the <span class="bold">Workfront Source Field</span> column, choose a native or custom <em>Workfront</em> field.</p> </li> 
   <li value="2"> <p>In the <span class="bold">Experience Manager Target Field</span>, choose an <em>Experience Manager Assets Essentials</em> field. </p> </li> 
   <li value="3"> <p>Repeat steps a. and b. as needed.</p> <note type="note">
     You can map metadata only in one direction: from 
     <em>Workfront</em> to 
     <em>Assets Essentials</em>. Metadata for documents linked to 
     <em>Workfront</em> from 
     <em>Assets Essentials</em> cannot be transferred to 
     <em>Workfront</em>.
    </note> </li> 
  </ol> </li> 
 <li value="6"> <p>Select <span class="bold">Save</span>.</p> </li> 
</ol>

