---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Create connections in [!DNL Adobe Workfront] Fusion
description: A connection must adhere to the requirements set by the API of the app or web service it connects to. For this reason, instructions for setting up a connection vary based on the app or web service. This article can help you identify and locate the instructions for connecting [!DNL Adobe Workfront Fusion] to your chosen app or web service.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
---
# Create connections in [!DNL Adobe Workfront] Fusion

A connection must adhere to the requirements set by the API of the app or web service it connects to. For this reason, instructions for setting up a connection vary based on the app or web service. This article can help you identify and locate the instructions for connecting [!DNL Adobe Workfront Fusion] to your chosen app or web service.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td>

</tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Connect [!DNL Adobe] Workfront to Workfront Fusion

Workfront and [!DNL Workfront Fusion] are designed to work together. The connection you create determines the account that [!DNL Workfront Fusion] uses to perform actions in Workfront.

For instructions, see [Connect [!DNL Workfront] to Workfront Fusion](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront] modules](../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

## Connect to an app or web service that does not require configuration

In most cases, you can use the module to create a connection with little or no extra information. [!DNL Workfront Fusion] handles the authentication automatically.

For instructions on creating a connection with no special considerations, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Connect to a Microsoft app or web service

Most of the [!DNL Microsoft] apps in [!DNL Workfront Fusion] allow you to create a connection with no extra information.

The following circumstances do require extra steps in creating a connection:

* Using Microsoft Dynamics 365 modules.

   For instructions, see [Microsoft Dynamics 365 modules](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Connecting to the [!DNL Microsoft] Graph API using an HTTP module

   For instructions, see [Call the MS Graph REST API via the Adobe Workfront Fusion HTTP > Make an OAuth 2.0 request module](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Connect to a Google app or web service

The process for connecting to Google apps may differ based on what kind of Google account you are using. In addition, Google security measures may require extra configuration when you are connecting to Workfront Fusion.

For more information see:

* [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] with updated security measures](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Other apps that require additional configuration

The following apps do not follow the basic configuration for [!DNL Workfront Fusion] connections. You can find instructions for connecting these apps in the article for that app.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>App / Web Service</th> 
   <th>Additional information about connections</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Connect [!DNL Adobe] [!DNL Workfront] to Workfront Fusion</a> in <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">Adobe Workfront modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Allocadia</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Connect Allocadia to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">Allocadia modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Anaplan</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Connect Anaplan to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">Anaplan modules</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>AWS S3</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Connect AWS to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">AWS S3 modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Azure DevOps</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Connect [!DNL Azure DevOps] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bynder</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Connect Bynder to [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">Bynder modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CloudConvert</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Connect CloudConvert to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">CloudConvert modules</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>Cvent</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Connect Cvent to [!DNL Adobe Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">Cvent modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datadog</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Connect Datadog to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">Datadog modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>DocuSign</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Connect your email to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">Email modules</a></td>

<tr> 
   <td role="rowheader"> <p>Gmail</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Connect Gmail to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">Gmail modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Intacct</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md#connecti" class="MCXref xref">Connect Intacct to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md" class="MCXref xref">Intacct modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira Cloud</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Connect [!DNL Jira] Cloud to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira] Software modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira Server</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Connect [!DNL Jira] Server to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira] Software modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Maria DB</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Connect [!DNL MariaDB] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Marketo</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>MS Dynamics</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Connect Microsoft Dynamics 365 to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">Microsoft Dynamics 365 modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Qualtrics</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Connecting Qualtrics to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">Qualtrics modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ServiceNow</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Connect [!DNL ServiceNow] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Connect SFTP to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">SFTP modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SharePoint</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">SharePoint modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Split.io</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Connect Split.io to [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">Split.io modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Widen</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] modules</a></td> 
  </tr> 
 </tbody> 
</table>
