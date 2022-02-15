---
filename: fusion-may-3
product: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
---



# *`Workfront Fusion`* release activity:&nbsp;Week of May 3, 2021 {#workfront-fusion-release-activity-week-of-may}

This page describes all enhancements made in *`Adobe Workfront Fusion`* the week of *`May 3, 2021`*.


For a list of all recent changes, see [Adobe Workfront Fusion release activity](fusion-release-activity.md).


For a list of recent bug fixes in *`Workfront Fusion`*, see the [ *`Workfront`* Maintenance Updates](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) page and check for any updates labeled *`Workfront Fusion`* Maintenance Update.


## Salesforce connector can now search using SOQL {#salesforce-connector-can-now-search-using-soql}

The Salesforce > Search for records module now has the option to search using SOQL (Salesforce Object Query Language). You can also search using the previously available options (SOSL and simple searches).


For more information, see [Salesforce modules](salesforce-modules.md).


## New connection type in Azure DevOps connector requires fewer scopes {#new-connection-type-in-azure-devops-connector-requires-fewer-scopes}

To enhance security, we've added a new connector type to the Workfront Fusion Azure DevOps Connector. Now, when you create a connection in an Azure DevOps module, you can select from two types of connections:



*  Azure DevOps


  This new connection type limits scopes to those specifically needed by Workfront Fusion.

*  Azure DevOps (Request all scopes)


  This is the legacy connection type, which requests all scopes available in a connection to Azure DevOps.



We recommend that you use the Azure DevOps connection type in all your new scenarios that use Azure DevOps. We also recommend that you change any Azure DevOps modules in your existing scenarios to use the new connection type. The legacy Azure DevOps (Request all scopes) connection type will be deprecated in the near future.


For more information, see [Azure DevOps modules](azure-dev-ops.md).
