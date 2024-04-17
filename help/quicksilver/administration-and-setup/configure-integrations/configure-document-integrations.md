---
title: Configure document integrations
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: As an Adobe Workfront administrator, you can configure document integrations to manage documents in Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
---
# Configure document integrations

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

As an [!DNL Adobe Workfront] administrator, you can configure document integrations to manage documents in [!UICONTROL Workfront]. You can also configure [!UICONTROL Workfront] so that documents are stored only in document services applications and not in [!UICONTROL Workfront] itself. For more information, see [Update and link a document from [!UICONTROL Workfront] to an external cloud provider](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>To allow open communication between [!DNL Workfront Proof] and the [!DNL Workfront] servers, you might need to add certain IP addresses to your allowlist. For more information, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>New: [!UICONTROL Standard]</p>
       <p>or</p>
       <p>Current: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a [!DNL Workfront] administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Supported integrations

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

You can configure the following integrations for managing documents:

   <!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Linking proofs from [!DNL Workfront Proof] allows you to make proofs that were originally created within [!DNL Workfront Proof] available within [!DNL Workfront]. For the current plans, a [!UICONTROL Pro] [!DNL Workfront] Plan or higher is required to use this feature. For the new plans, this feature is available with all plans. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

   For information about integrating with [!DNL SharePoint], see [Configure the [!DNL SharePoint] integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Third party cloud document providers:

    * [!DNL Box]
    * [!DNL Dropbox]
    * [!DNL Dropbox Business]
    * [!DNL WebDAM]
    * [!DNL Microsoft OneDrive]
    * [!DNL Microsoft SharePoint]
    * [!UICONTROL Google Drive]

      <!--Quip-->
      
   >[!TIP]
   >
   >You can proof and approve documents linked from an external cloud provider the same way you proof and approve documents uploaded directly to [!DNL Workfront].

* Other document providers (through custom document integrations).

   For the current plans, a [!UICONTROL Pro] [!DNL Workfront] Plan or higher is required to use this feature. For the new plans, this feature is available with all plans. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).

In addition, you can enhance your [!DNL Workfront] document experience with a native Digital Asset Management (DAM) system, or with third-party DAM integrations. Administrators must enable these features in order for users to link the service to their [!DNL Workfront] account. For more information about Workfront DAM, see [Managing Documents with [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configure integrations to manage documents

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers].**

1. (Optional) To stored documents in a document services application and not in [!DNL Workfront], select **[!UICONTROL Prevent Users From Storing Documents in [!DNL Workfront]].**

1. Select the integrations you want enabled.
1. Click **[!UICONTROL Save]**.

If you are setting up integrations with [!DNL Workfront DAM], you can enable [!DNL Workfront] to include metadata with documents. For information about mapping metadata, see [Set up metadata mapping](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configure custom document integrations

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

A custom document integration allows [!DNL Workfront] users to link files into [!DNL Workfront] from practically any system, provided that the system is made to work with [!DNL Workfront].

To make the custom integration available to users, you first need to build the integration. For information about how to build integrations to be used with [!DNL Workfront], see [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

After the custom document integration is built, you can make it available to users on your site.

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]**.

1. Click **[!UICONTROL Add Custom integration]**.
1. Enter the following information to configure the integration:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>The name of the custom integration. This is the name users see when using the integration within Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>The base HTTP or secure HTTP URL for API calls. For example, <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>The authentication method to use when making authorized API calls to the custom integration.</p> 
       <ul> 
        <li>If you choose <strong>[!UICONTROL OAuth]</strong>, continue with Step 5.</li> 
        <li>If you choose <strong>[!UICONTROL ApiKey]</strong>, continue with Step 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional) If you selected **[!UICONTROL OAuth]** authentication for the **[!UICONTROL Authentication Type]**, enter the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>The full URL used for user authentication. [!DNL Workfront] navigates users to this address as part of the OAuth provisioning process.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>The full API URL used to retrieve OAuth tokens.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>The OAut Client ID for this integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>The OAut Client Secret for this integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Parameters]</td> 
      <td> <p>Enter optional values to be appended to the query string of every API call. For example, access_type=offline.</p> <p>To add multiple request parameters, click <strong>+Add Request Parameter</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >The [!DNL Workfront] Redirect URI that displays at the bottom of the [!UICONTROL Custom Integration] page lists the URI used to register this integration with the external document provider.

1. (Conditional) If you selected **[!UICONTROL ApiKey]** authentication for the **[!UICONTROL Authentication Type]**, enter the API key that was issued by the custom document provider.

   [!DNL Workfront] uses this API key to make authorized API calls to the document provider.

1. Click **[!UICONTROL Save]** to create the integration.

## Use document integrations

For information about how users can use [!DNL Workfront DAM], see [Managing Documents with [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

For information about how users can use proofing, see [Create proofs](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

For information about how users can use third-party document integrations after you have configured them, see [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configure [!DNL Workfront] to send metadata to [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

When sending a document from [!DNL Workfront] to [!DNL Workfront DAM], you can also send information associated with that document. Information about the document is mapped to [!DNL Workfront DAM] as metadata.

Information is mapped one-way only, from [!DNL Workfront] to [!DNL Workfront DAM] and it is transferred only when the document is uploaded to [!DNL Workfront DAM]. Any future changes in the Workfront fields will not update metadata fields in [!DNL Workfront DAM] after the document has already been uploaded.\
You can map the same [!DNL Workfront] field to various [!DNL Workfront DAM] fields, but you cannot use the same [!DNL Workfront DAM] field for multiple [!DNL Workfront] fields.

If you must configure multiple [!DNL Workfront] fields to export to one [!DNL Workfront DAM] field, first create a calculated custom field in [!DNL Workfront] to display all the individual custom fields of an object. Then, map the calculated [!DNL Workfront] field to one [!DNL Workfront DAM] field.\
For more information about calculated custom fields, see [Add calculated data to a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

The mapping affects all the documents uploaded by any user from [!DNL Workfront] to [!UICONTROL Workfront] DAM.

As a [!DNL Workfront] administrator, you must enable [!DNL Workfront DAM] in Workfront before you can map the fields for the metadata mapping process.

To configure [!DNL Workfront] to send metadata to [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Click **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. In the **[!UICONTROL Select Source Field for Mapping]** field, begin typing the name of the Workfront field you want to map to [!DNL Workfront DAM], then select it when you see it in the list.
1. In the **[!UICONTROL Select Target Field for Mapping]**, select the [!DNL Workfront DAM] field you want to populate with the information in the selected [!DNL Workfront] field.

   >[!NOTE]
   >
   > All documents sent to [!DNL Workfront DAM] by users who have the rights to do so have their metadata updated with the [!DNL Workfront] fields mapped here, when they upload to [!DNL Workfront DAM].

1. Click **[!UICONTROL Add Mapping]**.

1. Continue adding more [!UICONTROL Workfront] fields and corresponding [!DNL Workfront DAM] fields.

### Delete mapped fields

{{step-1-to-setup}}

1. Expand **[!UICONTROL Documents]**, then click **[!UICONTROL Metadata Mapping]**.

1. In the list of fields, select any of the fields you want to remove from metadata mapping.
1. Click **[!UICONTROL Delete]**.

   The fields are removed from metadata mapping and the information contained in them is not transferred to [!DNL Workfront DAM] with the uploaded documents.
