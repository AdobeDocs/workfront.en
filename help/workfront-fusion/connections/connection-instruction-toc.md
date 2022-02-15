---
filename: connection-instruction-toc
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
---



# Create connections in *`Adobe Workfront Fusion`* {#create-connections-in-adobe-workfront-fusion}

A connection must adhere to the requirements set by the API of the app or web service it connects to. For this reason, instructions for setting up a connection vary based on the app or web service. This article can help you identify and locate the instructions for connecting *`Adobe Workfront Fusion`* to your chosen app or web service.


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Connect *`Adobe Workfront`* to *`Workfront Fusion`* {#connect-adobe-workfront-to-workfront-fusion}

*`Workfront`* and *`Workfront Fusion`* are designed to work together. The connection you create determines the account that *`Workfront Fusion`* uses to perform actions in *`Workfront`*.


For instructions, see [Connect Workfront to Workfront Fusion](workfront-modules.md#connect) in [Adobe Workfront modules](workfront-modules.md). 


## Connect to an app or web service that does not require configuration {#connect-to-an-app-or-web-service-that-does-not-require-configuration}

In most cases, you can use the module to create a connection with little or no extra information. *`Workfront Fusion`* handles the authentication automatically.


For instructions on creating a connection with no special considerations, see [Create a connection to Workfront Fusion - Basic instructions](connect-to-fusion-general.md).


## Connect to a Microsoft app or web service {#connect-to-a-microsoft-app-or-web-service}

Most of the Microsoft apps in *`Workfront Fusion`* allow you to create a connection with no extra information. 


The following circumstances do require extra steps in creating a connection:



*  Using Microsoft Dynamics 365 modules.


  For instructions, see [Microsoft Dynamics 365 modules](microsoft-dynamics-365-modules.md).

*  Connecting to the Microsoft Graph API using an HTTP module


  For instructions, see [Call the MS Graph REST API via the HTTP > Make an OAuth 2.0 request module](call-the-ms-graph-rest-api .md).





## Connect to a Google app or web service {#connect-to-a-google-app-or-web-service}

The process for connecting to Google apps may differ based on what kind of Google account you are using. In addition, Google security measures may require extra configuration when you are connecting to *`Workfront Fusion`*.


For more information see:



*  [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](connect-fusion-to-google-using-oauth.md) 
*  [Connect Adobe Workfront Fusion to Google Services with updated security measures](connect-to-google-with-new-security-measures.md) 




## Other apps that require additional configuration {#other-apps-that-require-additional-configuration}

The following apps do not follow the basic configuration for *`Workfront Fusion`* connections. You can find instructions for connecting these apps in the article for that app.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <thead> 
  <tr> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadH-Column1-">App / Web Service</th> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadG-Column2-">Additional information about connections</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Allocadia</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="allocadia-modules.md#connect" class="MCXref xref">Connect Allocadia to Workfront Fusion</a> in <a href="allocadia-modules.md" class="MCXref xref">Allocadia modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>AWS S3</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="aws-s3-modules.md#connecti" class="MCXref xref">Connect AWS to Workfront Fusion</a> in <a href="aws-s3-modules.md" class="MCXref xref">AWS S3 modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Azure DevOps</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="azure-dev-ops.md#connect" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in <a href="azure-dev-ops.md" class="MCXref xref">Azure DevOps modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Bynder</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="bynder-modules.md#connect" class="MCXref xref">Connect Bynder to Workfront Fusion </a> in <a href="bynder-modules.md" class="MCXref xref">Bynder modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Cvent</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="cvent-modules.md#connect" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in <a href="cvent-modules.md" class="MCXref xref">Cvent modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Datadog</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="datadog-modules.md#connect" class="MCXref xref">Connect Datadog to Workfront Fusion</a> in <a href="datadog-modules.md" class="MCXref xref">Datadog modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>DocuSign</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="docusign-modules.md#connect" class="MCXref xref">Connect DocuSign to Workfront Fusion</a> in <a href="docusign-modules.md" class="MCXref xref">DocuSign modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Email</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="email-modules.md#connecti" class="MCXref xref">Connect your email to Workfront Fusion</a> in <a href="email-modules.md" class="MCXref xref">Email modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Gmail</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="gmail-modules.md#connect3" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in <a href="gmail-modules.md" class="MCXref xref">Gmail modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Intacct</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="intacct-modules.md#connecti" class="MCXref xref">Connect Intacct to Workfront Fusion</a> in <a href="intacct-modules.md" class="MCXref xref">Intacct modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Jira Cloud</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="jira-software-modules.md#connect" class="MCXref xref">Connect Jira Cloud to Workfront Fusion</a> in <a href="jira-software-modules.md" class="MCXref xref">Jira Software modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Jira Server</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="jira-software-modules.md#connect2" class="MCXref xref">Connect Jira Server to Workfront Fusion</a> in <a href="jira-software-modules.md" class="MCXref xref">Jira Software modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Maria DB</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="mariadb-modules.md#connect" class="MCXref xref">Connect MariaDB to Workfront Fusion</a> in <a href="mariadb-modules.md" class="MCXref xref">MariaDB modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Marketo</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="marketo-modules.md#connect" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in <a href="marketo-modules.md" class="MCXref xref">Marketo modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>MS Dynamics</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in <a href="microsoft-dynamics-365-modules.md" class="MCXref xref">Microsoft Dynamics 365 modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Qualtrics</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="qualtrics-modules.md#connecti" class="MCXref xref">Connecting Qualtrics to Workfront Fusion</a> in <a href="qualtrics-modules.md" class="MCXref xref">Qualtrics modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>ServiceNow</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="servicenow-modules.md#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in <a href="servicenow-modules.md" class="MCXref xref">ServiceNow modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>SFTP</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="sftp.md#connect" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in <a href="sftp.md" class="MCXref xref">SFTP modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>SharePoint</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><a href="sharepoint-modules.md#connect" class="MCXref xref">Connect SharePoint to Workfront Fusion</a> in <a href="sharepoint-modules.md" class="MCXref xref">SharePoint modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Split.io</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><a href="split-io-modules.md#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in <a href="split-io-modules.md" class="MCXref xref">Split.io modules</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"> <p>Widen</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><a href="widen-modules.md#connect" class="MCXref xref">Connect Widen to Workfront Fusion </a> in <a href="widen-modules.md" class="MCXref xref">Widen modules</a></td> 
  </tr> 
 </tbody> 
</table>

