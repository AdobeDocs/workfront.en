---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Working with large files in Adobe Workfront Fusion
description: 
author: Becky
feature: Workfront Fusion
exl-id: 7ba95790-1255-4a3e-ba7b-8dc73001b583
---
# Working with large files in Adobe Workfront Fusion

Consider the following when working with large files in your Fusion scenarios. 

## Large file size effect on scenario execution time

Large files may take some time to upload, download, or process in your Fusion scenario. While there is no limit on file size, there is a 40 minute limit on scenario execution time. Therefore, if large files cause the execution to take more than 40 minutes, the scenario fails.

Scenario execution time can also be affected by scenario size, module complexity, and network speed. Therefore, we recommend that you consider these aspects of your scenarios when using large files. 

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

<!--

## Connectors that support large files

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