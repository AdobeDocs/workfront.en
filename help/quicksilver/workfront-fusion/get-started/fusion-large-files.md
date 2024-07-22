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



