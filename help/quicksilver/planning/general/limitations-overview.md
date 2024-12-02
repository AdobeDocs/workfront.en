---
title: Adobe Workfront Planning Object Limitations Overview
description: Adobe Workfront Planning has limits for how many objects you can create in your instance. Object limits are in place to improve product performance and enhance your experience with Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
---
<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Adobe Workfront Planning object limitations overview

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}


Adobe Workfront Planning has limits for how many objects you can create in your instance. Object limits are in place to improve product performance and enhance your experience with Workfront Planning. 

The following table shows the limits for how many objects you can create in Workfront Planning. The limitations are subject to change as we move into the next phases of development. 

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with Planning <br> 500,000 for customers with Planning Plus                                                                                                         |
|     Number of total records for one instance of Workfront Planning                                               |   500,000 for customers with the Planning plan <br>2 million for customers with Planning Plus                                                                                                         |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a Single-line text field                                                               |   1,000 characters                                                                                              |
|     Number of characters for a paragraph  field                                                               |   10,000 characters                                                                                              |
|     Number of paragraph fields for one record type                                                               |   20 paragraph fields                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |
| Size of CSV of Excel file you can import to create record types | 5MB |
| <span class="preview">Number of rows you can import in a CSV or Excel file to create record types</span> | 10,000 |
| <span class="preview">Number of columns you can import in a CSV or Excel file to create record types</span> | 500 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.

For information about Workfront Planning pricing and packaging, see [Adobe Workfront pricing and packaging](https://business.adobe.com/products/workfront/pricing.html). 

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->
