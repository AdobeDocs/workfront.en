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

As an Adobe Workfront administrator, you can configure document integrations to manage documents in Workfront. You can also configure Workfront so that documents are stored only in document services applications and not in Workfront itself. For more information, see [Update and link a document from Workfront to an external cloud provider](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>To allow open communication between Workfront Proof and the Workfront servers, you might need to add certain IP addresses to your allowlist. For more information, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Supported integrations

You can configure the following integrations for managing documents:

* Workfront Library
* Workfront DAM   

* Workfront Proof

  Linking proofs from Workfront Proof allows you to make proofs that were originally created within Workfront Proof available within Workfront. A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)

* Microsoft SharePoint

  For information about integrating with SharePoint, see [Configure the SharePoint integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Third party cloud document providers:

  * Box
  * Dropbox
  * Dropbox Business 
  * WebDAM
  * Microsoft OneDrive
  * Google Drive

    <!--  
    Quip  
    -->

  >[!TIP]
  >
  >You can proof and approve documents linked from an external cloud provider the same way you proof and approve documents uploaded directly to Workfront.

* Other document providers (through custom document integrations).

  A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)

In addition, you can enhance your Workfront document experience with a native Digital Asset Management (DAM) system, or with third-party DAM integrations. Administrators must enable these features in order for users to link the service to their Workfront account. For more information about Workfront DAM, see [Managing Documents with Adobe Workfront DAM](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configure integrations to manage documents

1. Log in to Workfront as the administrator.
1. Click `Setup` near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. In the left panel, click `Documents` > `Cloud Providers.`

1. (Optional) To stored documents in a document services application and not in Workfront, select `Prevent Users From Storing Documents in Workfront.`  

1. Select the integrations you want enabled.
1. Click `Save`.

If you are setting up integrations with Workfront Library or Workfront DAM, you can enable Workfront to include metadata with documents. For information about mapping metadata, see [Set up metadata mapping](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configure custom document integrations

A custom document integration allows Workfront users to link files into Workfront from practically any system, provided that the system is made to work with Workfront.

To make the custom integration available to users, you first need to build the integration. For information about how to build integrations to be used with Workfront, see [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

After the custom document integration is built, you can make it available to users on your site.

1. Log in to Workfront as the administrator.
1. Click `Setup` near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. In the left panel, click `Documents` > `Custom Integration.`

1. Click `Add Custom integration`.
1. Specify the following information to configure the integration:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>The name of the custom integration. This is the name users see when using the integration within Workfront.</td> 
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
   </table>

1. (Conditional) If you selected `OAuth` authentication for the `Authentication Type`, specify the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Authentication URL</td> 
      <td>The full URL used for user authentication. Workfront&nbsp;navigates users to this address as part of the OAuth provisioning process.</td> 
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
   </table>

   >[!TIP]
   >
   >The Workfront&nbsp;Redirect URI that displays at the bottom of the Custom Integration page lists the URI used to register this integration with the external document provider.

1. (Conditional) If you selected `ApiKey` authentication for the `Authentication Type`, specify the API key that was issued by the custom document provider.

   Workfront uses this API key to make authorized API calls to the document provider.

1. Click `Save` to create the integration.

## Use document integrations

For information about how users can use Workfront Library, see [Add a Workfront Library asset to Workfront](../../workfront-library/content-management/add-a-wf-library-asset.md).

For information about how users can use Workfront DAM, see [Managing Documents with Adobe Workfront DAM](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

For information about how users can use Workfront Proof, see [Generate a proof](../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md).

For information about how users can use third-party&nbsp;document integrations after you have configured them, see [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configure Workfront to send metadata to Workfront DAM

When sending a document from Workfront to Workfront DAM, you can also send information associated with that document. Information about the document is mapped to Workfront DAM as metadata.

Information is mapped one-way only, from Workfront to Workfront DAM and it is transferred only when the document is uploaded to Workfront DAM. Any future changes in the Workfront fields will not update metadata fields in Workfront DAM after the document has already been uploaded.  
You can map the same Workfront field to various Workfront DAM fields, but you cannot use the same Workfront DAM field for multiple Workfront fields.&nbsp;

If you must configure multiple Workfront fields to export to one Workfront DAM field, first create a calculated custom field in Workfront to display all the individual custom fields of an object. Then, map the calculated Workfront field to one Workfront DAM field.  
For more information about calculated custom fields, see [Add calculated data to a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

The mapping affects all the documents uploaded&nbsp;by any user from Workfront to Workfront DAM.

As a Workfront administrator, you must enable Workfront DAM in Workfront before you can map the fields for the metadata mapping process. For more information about how to&nbsp;enable Workfront DAM, see [Configure Workfront to send metadata to Workfront DAM](#configur2). &nbsp;

To configure Workfront to send metadata to Workfront DAM:

1. <![CDATA[        ]]>Click `Setup` near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. Click `Documents` > `Metadata Mapping`.   

1. In the `Select Source Field for Mapping` field, begin&nbsp;typing the name of the Workfront field you want to map to Workfront DAM, then select it when you see it in the list.&nbsp;
1. In the `Select Target Field for Mapping`, select the Workfront DAM field you want to populate with the information in the selected Workfront field.

   >[!NOTE]
   >
   >&nbsp;All&nbsp;documents sent to Workfront DAM by users who have the rights to do so have their metadata updated with the Workfront fields mapped here, when they upload to Workfront DAM.

1. Click `Add Mapping`.  

1. Continue adding more Workfront fields and&nbsp;corresponding Workfront DAM fields.&nbsp;

### Delete mapped fields

1. Click `Setup` near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. Expand `Documents`, then click `Metadata Mapping`.

1. In the list of fields, select any of the fields you want to remove from metadata mapping.
1. Click `Delete`.

   The fields are removed from metadata mapping and the information contained in them is not transferred to Workfront DAM with the uploaded documents.&nbsp;

