---
filename: configure-document-integrations
title: Configure document integrations
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configure document integrations
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Configure document integrations

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

As an *Adobe Workfront administrator*, you can configure document integrations to manage documents in *Workfront*. You can also configure *Workfront* so that documents are stored only in document services applications and not in *Workfront* itself. For more information, see [Update and link a document from Workfront to an external cloud provider](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>To allow open communication between *Workfront Proof* and the *Workfront* servers, you might need to add certain IP addresses to your allowlist. For more information, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Supported integrations

You can configure the following integrations for managing documents:

<ul> 
 <li> <p>Workfront Library</p> </li> 
 <li> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver"><em>Experience Manager Assets Essentials</em> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver"><em>Experience Manager Assets Essentials</em> </p> </li> 
 <li> <p><em>Workfront DAM</em> <br> </p> </li> 
 <li> <p><em>Workfront Proof</em> <br> </p> <p>Linking <em>proofs</em> from <em>Workfront Proof</em> allows you to make <em>proofs</em> that were originally created within <em>Workfront Proof</em> available within <em>Workfront</em>. A Pro <em>Workfront</em> Plan or higher is required to use this feature. For more information about the various plans available, see <a href="https://www.workfront.com/plans"><em>Workfront</em> Plans.</a></p> </li> 
 <li> <p>Microsoft SharePoint<br></p> <p>For information about integrating with SharePoint, see <a href="../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md" class="MCXref xref">Configure the SharePoint integration</a>.</p> </li> 
 <li>Third party cloud document providers: 
  <ul>
   <li>Box</li>
   <li>Dropbox</li>
   <li class="preview">Dropbox Business </li>
   <li>WebDAM</li>
   <li>Microsoft OneDrive</li>
   <li>Google Drive</li><draft-comment>
    <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Quip</li>
   </draft-comment>
   <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Quip</li>
  </ul><note type="tip">
   You can 
   <em>proof</em> and approve documents linked from an external cloud provider the same way you 
   <em>proof</em> and approve documents uploaded directly to 
   <em>Workfront</em>.
  </note></li> 
 <li> <p>Other document providers (through custom document integrations).</p> <p>A Pro <em>Workfront</em> Plan or higher is required to use this feature. For more information about the various plans available, see <a href="https://www.workfront.com/plans"><em>Workfront</em> Plans.</a></p> </li> 
</ul>

In addition, you can enhance your *Workfront* document experience with a native Digital Asset Management (DAM) system, or with third-party DAM integrations. Administrators must enable these features in order for users to link the service to their *Workfront* account. For more information about Workfront DAM, see [Managing Documents with Adobe Workfront DAM](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configure integrations to manage documents

<ol> 
 <li value="1">Log in to <em>Workfront</em> as the administrator.</li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="3">In the left panel, click <span class="bold">Documents</span> > <span class="bold">Cloud Providers.</span></li> 
 <li value="4">(Optional) To stored documents in a document services application and not in <em>Workfront</em>, select <span class="bold">Prevent Users From Storing Documents in Workfront.</span><br></li> 
 <li value="5">Select the integrations you want enabled.</li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

If you are setting up integrations with *Workfront Library* or *Workfront DAM*, you can enable Workfront to include metadata with documents. For information about mapping metadata, see [Set up metadata mapping](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configure custom document integrations

A custom document integration allows *Workfront* users to link files into *Workfront* from practically any system, provided that the system is made to work with *Workfront*.

To make the custom integration available to users, you first need to build the integration. For information about how to build integrations to be used with *Workfront*, see [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

After the custom document integration is built, you can make it available to users on your site.

<ol> 
 <li value="1">Log in to <em>Workfront</em> as the administrator.</li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="3">In the left panel, click <span class="bold">Documents</span> > <span class="bold">Custom Integration.</span></li> 
 <li value="4">Click <span class="bold">Add Custom integration</span>.</li> 
 <li value="5"> <p>Specify the following information to configure the integration:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td>The name of the custom integration. This is the name users see when using the integration within <em>Workfront</em>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Base API URL </td> 
     <td>The base HTTP or secure HTTP URL for API calls. For example, <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Authentication Type</td> 
     <td> <p>The authentication method to use when making authorized API calls to the custom integration.</p> 
      <ul> 
       <li>If you choose <span class="bold">OAuth</span>, continue with Step 6.</li> 
       <li>If you choose <span class="bold">ApiKey</span>, continue with Step 7.</li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>(Conditional) If you selected <span class="bold">OAuth</span>&nbsp;authentication for the <span class="bold">Authentication Type</span>, specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Authentication URL</td> 
     <td>The full URL used for user authentication. <em>Workfront</em>&nbsp;navigates users to this address as part of the OAuth provisioning process.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Token Endpoint URL</td> 
     <td>The full API URL used to retrieve OAuth tokens.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client ID</td> 
     <td>The OAut&nbsp;Client ID for this integration.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client Secret</td> 
     <td>The OAut&nbsp;Client Secret for this integration.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Request Parameters</td> 
     <td> <p>Specify optional values to be appended to the query string of every API call. For example, access_type=offline.</p> <p>To add multiple request parameters, click <span class="bold">+Add Request Parameter</span>.</p> </td> 
    </tr> 
   </tbody> 
  </table> <note type="tip">
   The Workfront&nbsp;Redirect URI that displays at the bottom of the Custom Integration page lists the URI used to register this integration with the external document provider.
  </note> </li> 
 <li value="7"> <p>(Conditional) If you selected <span class="bold">ApiKey</span> authentication for the <span class="bold">Authentication Type</span>, specify the API key that was issued by the custom document provider.</p> <p><em>Workfront</em> uses this API key to make authorized API calls to the document provider.</p> </li> 
 <li value="8">Click <span class="bold">Save</span> to create the integration.</li> 
</ol>

## Use document integrations

For information about how users can use *Workfront Library*, see [Add a Workfront Library asset to Workfront](../../workfront-library/content-management/add-a-wf-library-asset.md).

For information about how users can use *Workfront DAM*, see [Managing Documents with Adobe Workfront DAM](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

For information about how users can use *Workfront Proof*, see [Generate a proof](../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md).

For information about how users can use third-party&nbsp;document integrations after you have configured them, see [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configure *Workfront* to send metadata to *Workfront* DAM

When sending a document from *Workfront* to *Workfront DAM*, you can also send information associated with that document. Information about the document is mapped to *Workfront DAM* as metadata.

Information is mapped one-way only, from *Workfront* to *Workfront DAM* and it is transferred only when the document is uploaded to *Workfront DAM*. Any future changes in the *Workfront* fields will not update metadata fields in *Workfront DAM* after the document has already been uploaded.  
You can map the same *Workfront* field to various *Workfront DAM* fields, but you cannot use the same *Workfront DAM* field for multiple *Workfront* fields.&nbsp;

If you must configure multiple *Workfront* fields to export to one *Workfront DAM* field, first create a calculated custom field in *Workfront* to display all the individual custom fields of an object. Then, map the calculated *Workfront* field to one *Workfront DAM* field.  
For more information about calculated custom fields, see [Add calculated data to a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

The mapping affects all the documents uploaded&nbsp;by any user from *Workfront* to *Workfront DAM*.

As a *Workfront administrator*, you must enable *Workfront DAM* in *Workfront* before you can map the fields for the metadata mapping process. For more information about how to&nbsp;enable *Workfront DAM*, see [Configure Workfront to send metadata to Workfront DAM](#configur2). &nbsp;

To configure *Workfront* to send metadata to *Workfront DAM*:

<ol> 
 <li value="1"><![CDATA[
        ]]>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> Click <span class="bold">Documents</span> > <span class="bold">Metadata Mapping</span>. <br></li> 
 <li value="3"> In the <span class="bold">Select Source Field for Mapping</span> field, begin&nbsp;typing the name of the <em>Workfront</em> field you want to map to <em>Workfront DAM</em>, then select it when you see it in the list.&nbsp;</li> 
 <li value="4"> <p>In&nbsp;the <span class="bold">Select Target Field for Mapping</span>, select the <em>Workfront DAM</em> field you want to populate with the information in the selected <em>Workfront</em> field.</p> <note type="note">
   &nbsp;All&nbsp;documents sent to 
   <em>Workfront DAM</em> by users who have the rights to do so have their metadata updated with the 
   <em>Workfront</em> fields mapped here, when they upload to 
   <em>Workfront DAM</em>.
  </note> </li> 
 <li value="5">Click <span class="bold">Add Mapping</span>.<br></li> 
 <li value="6">Continue adding more <em>Workfront</em> fields and&nbsp;corresponding <em>Workfront DAM</em> fields.&nbsp;</li> 
</ol>

### Delete mapped fields

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">Expand <span class="bold">Documents</span>, then click <span class="bold">Metadata Mapping</span>.</li> 
 <li value="3">In the list of fields, select any of the fields you want to remove from metadata mapping.</li> 
 <li value="4"> <p>Click <span class="bold">Delete</span>.<br></p> <p>The fields are removed from metadata mapping and the information contained in them is not transferred to <em>Workfront DAM</em> with the uploaded documents.&nbsp;</p> </li> 
</ol>

