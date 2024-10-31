---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Working with large files in Adobe Workfront Fusion
description: Large file support is currently available for the Workfront and HTTP connectors.
author: Becky
feature: Workfront Fusion
---
# Working with large files in Adobe Workfront Fusion

Enhanced data transfer capabilities are now available in Workfront Fusion, enabling scenarios to process significantly larger files. 

Large file capability is available only to Workfront Ultimate customers. 

To handle larger files, your scenarios must be updated.  

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>
   <td> <p>New: Ultmate</p> <p>Or</p> <p>Current: Not available</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p><p>Or</p><p>Current: Not available</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy: Any </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>New: [!DNL Workfront Fusion] is included in the Ultimate Workfront plan.</p> <p>Or</p>
   <p>Current: Not available</p>
   </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Connectors that support large files

For the initial release, the following connectors support large files. 

* Workfront
* HTTP

Other connectors will be supported in future releases.

## Update your scenarios to handle large files

The Workfront > Upload Document module has been modified to handle larger files. The former version of this module now displays `(Legacy)` appended to the module name. In most cases the legacy module will continue to function. 

If you plan on working with larger files, we recommend replacing the legacy module with the new Upload Document module. The new Upload Document module prevents timeouts and other errors.  

![Upload document](assets/new-upload-document.png)

## FAQ 

### What is the new file size limit? 

Users can now process files exceeding the previous 1 GB limit, enhancing efficiency and productivity.  Although the platform can support individual files up to 15 GB for a single action (such as uploading a file), there are other factors that affect data transfer. The file size limit of single action ultimately depends on the web service that Fusion connects to. Data transfer is the total processing for a single execution. This means multiple actions in a single execution contribute to the total data transfer. 

Fusion processes files until the execution limit of 40 minutes is reached. Large files may take some time to upload, download, or process in your Fusion scenario. While there is no limit on individual file size, there is a 40 minute limit on scenario execution time. Therefore, if large files cause the execution to take more than 40 minutes, the scenario fails. Scenario execution time can also be affected by scenario size, module complexity, and network speed. Therefore, we recommend that you consider these aspects of your scenarios when using large files.  

### How does Fusion's new file transfer work? 

When Fusion processes files, larger files are added to persistent storage (S3 Bucket or Azure Blob Storage). When a Fusion module executes a file action, like upload or download, Fusion uses the file in persistent storage as the source instead of active memory.  

### Can I work with larger files using incomplete executions? 

Yes, Fusion supports incomplete executions with larger files. Note that incomplete executions are limited in size for an organization, and should be actively managed.  

### Can I use larger files with any connector? 

Each Fusion connector must be updated to support larger files. The supported connectors include Workfront, HTTP, and AEM Assets. Fusion connectors are still limited by the file size supported by the web service. File size limits are typically included in the API documentation for web service endpoints that download and upload files.  

### Does this affect operations? 

No, the number of operations executed by a module are the same.  

### When will Fusion's UI be updated to display file transfer data? 

We are actively working on updates to Fusion's UI for file transfer on the dashboard and scenario execution detail page, with a targeted release in Q1 2025. 

### What are some ways to think about the new file processing limits that will help me design scenarios?  

Designing a scenario to work within the 40 minutes execution limit can seem complicated. We recommend keeping the following in mind when designing a scenario:

* **Understand your business requirements for execution time**: Fusion's platform limit for execution time is 40 minutes, but most business process automations are expected to execute much faster. For example, user-initiated automations with result-dependent continuationwould be expected to complete well under the 40-minute limit.  
* **Consider execution time when designing**:  When designing your scenario, it is essential to understand the module execution time for individual file actions, such as uploads and downloads. This knowledge helps you plan scenarios that involve multiple file actions.  To ensure accuracy in your design, we recommend rounding the module's execution time up to include a buffer.
   For example, if Fusion downloads a document in 144 seconds (2.4 minutes), you can anticipate that a single execution can perform similar actions multiple times. In this example, the module execution takes 144 seconds to execute, and you should plan for 3 minutes execution time for download. If your requirements include both an upload and a download, the expected execution time would be approximately 6 minutes. Note that Fusion execution times are capped at 40 minutes. 

* **Consolidate file actions**: the most common example of file actions in a Fusion scenario is one download and one upload. Most scenarios with only these two actions will execute in a few minutes. When possible Fusion designers should constrain their scenarios to one download and one upload.  

* **Calculate size using the mapping panel**: Workfront and other web services include the file size of a file in the download module's output. You can use this data to filter out files too large for a module upload or too large for the scenario execution time.  

* **Isolate file actions in their own scenario when working with multiple files**: Fusion designers should consider isolating file actions into separate scenarios. For example, a Fusion scenario triggered by a new Workfront request with multiple attached files may need to accommodate up to 30 files. Given that uploading and downloading each file could take up to 3 minutes, processing all files in a single execution would surpass Fusion's 40-minute execution limit. The solution is to create a file actions scenario dedicated to handling the upload and download of individual files. The request-triggered scenario would iterate through the attached files, invoking the file actions scenario for each file using the HTTP module. This approach ensures that each file is processed within the execution time limits. 

<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom


If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->




