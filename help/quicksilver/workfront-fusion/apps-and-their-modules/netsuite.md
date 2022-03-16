---
filename: netsuite
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: NetSuite modules
description: In a Adobe Workfront Fusion scenario, you can connect your NetSuite account to multiple third-party applications and services.
---

# NetSuite modules

In a Adobe Workfront Fusion scenario, you can connect your NetSuite account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use NetSuite modules, you must have a NetSuite account.

<!--
Connect NetSuite to Workfront Fusion Prerequisites for using NetSuite's REST web services To use NetSuite's REST web services, you must first enable the relevant features in your account, and assign the required permissions to the web services user's role. Note: For instructions on enabling these features and assigning these permissions: See the "REST Web Services Prerequisites and Setup" section of the latest version of Oracle's SuiteTalk REST Web Services documentation. Or Log in to your Oracle Net Suite account, and search the online documentation for "REST Web Services Prerequisites and Setup." Enable Features Assign permissions Enable Features Enable the following features REST Web Services feature To use this feature, you must accept the SuiteCloud Terms of Service. REST Record Service (beta) feature This feature enables you to work with the REST record service beta functionality. Using the REST record service, you can: Perform CRUD operations on beta records Filter record collections Interact with record metadata Perform record actions and transformations. To use this feature, you must accept the SuiteCloud Terms of Service. REST Query Service (beta) feature This feature enables you to work with the REST query service beta functionality. Using the REST query service, you can work with datasets and related functionality. Suite Analytics Workbook feature This feature allows you to create workbooks that combine datasets, tables, pivot tables, and charts using the analytics data source. Note: To access the REST Record Service, REST Query Service, Record Customization, or SuiteScript Workbook API beta features, you must complete the Oracle NetSuite Umbrella Beta Program Recruitment Form. On this form, you must identify an authorized user who can sign to accept the Oracle Cloud Services Beta Trial License Agreement. After this agreement is fully executed by an authorized user through completion of this form, the requested features are available for enablement on this page. To locate the Oracle NetSuite Umbrella Beta Program Recruitment Form, search the Oracle NetSuite documentation. Assign permissions Assign the following permissions: REST Web Services Log in using Access Tokens Suite Analytics Workbook Create a new integration record To set up a connection between NetSuite and Workfront Fusion, you need to create a new integration record in Netsuite. Note: For instructions on creating a new integration record. See the "Setting Up OAuth 2.0 Authentication for REST Web Services" section of the latest version of Oracle's SuiteTalk REST Web Services documentation. Or Log in to your Oracle Net Suite account, and search the online documentation for "Create Integration Records for Applications to use Oauth 2.0." Begin creating a new integration record. When creating the new record, configure the following fields: Name Enter a name for your NetSuite integration State Select Enabled Authorization Code Grant Check this checkbox Redirect URI https://app.workfrontfusion.com/oauth/cb/workfront-netsuite-rest2 Scope Check the checkbox next to REST WEB SERVICES. Save the new integration. A page showing your client credentials appears. Copy and save the client credentials in a secure place. You will need them to create a connection in Workfront Fusion. Warning: You must copy and save the credentials before you close this window. You will not be able to access them again. Create a connection to NetSuite in a Workfront Fusion NetSuite module You can create a connection to your NetSuite account directly from inside a NetSuite module. In any NetSuite module, click Add next to the Connection field. Enter the Account ID of the Netsuite account you want the module to access. Enter the Client ID and Client Secret that you saved in step 3 in Create a new integration record above. Note: For security reasons, the values for Client Credentials are only displayed on the initial setup page. They cannot be retrieved from the system. If you did not save this information, you must reset credentials to obtain new values for your Client Credentials. Click Continue to create the connection and go back to the module.
-->

## NetSuite modules and their fields

When you configure NetSuite modules, Workfront Fusion displays the fields listed below. Along with these, additional NetSuite fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<!--
Triggers Actions Searches Triggers Watch records This trigger module activates a scenario when a record is created or updated. Connection For instructions about connecting your NetSuite account to Workfront Fusion, seeCreate a connection to NetSuite in a Workfront Fusion NetSuite module in this article. Record type Select the type of record you want to watch. Outputs Select the fields that you want to include in the module output. The available fields depend on the type of record you want to watch. Event type Select whether you want to watch for new records or updated records. Limit Set the highest number of records you want the module to return during each scenario execution cycle. Actions Custom API Call Create a record Update a record Delete a Record Read a Record
-->

#### Custom API Call

This action module lets you make a custom authenticated call to the NetSuite API. This way, you can create a data flow automation that can't be accomplished by the other NetSuite modules.

The action is based on the entity type (Allocadia object type) you specify.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create3" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Use the following URL format:</p> <p><code>https://{accountID}.suitetalk.api.netsuite.com/services/rest/record/{version}/{resource}?{query-parameters}</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
Create a record This action module creates a new record. You specify the type of record and field values for the new record. The module returns the ID of the record. You can map this information in subsequent modules in the scenario. When you are configuring this module, the following fields display. Connection For instructions about connecting your NetSuite account to Workfront Fusion, seeCreate a connection to NetSuite in a Workfront Fusion NetSuite module in this article. Record type Select the type of record you want to create. Properties Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create. Update a record This action module updates an existing record. When you are configuring this module, the following fields display. Connection For instructions about connecting your NetSuite account to Workfront Fusion, seeCreate a connection to NetSuite in a Workfront Fusion NetSuite module in this article. Record type Select the type of record you want to update. Internal ID Enter the unique NetSuite ID of the record that you want the module to update Properties Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create. Delete a Record This action module deletes a single record from NetSuite. You specify the ID of the record. The module returns the internal ID of the deleted record. When you are configuring this module, the following fields display. Connection For instructions about connecting your NetSuite account to Workfront Fusion, seeCreate a connection to NetSuite in a Workfront Fusion NetSuite module in this article. Record Type Select the type of record that you want the module to delete. Internal ID Enter or map the NetSuite ID of the record you want the module to delete. Read a Record This action module reads data from a single record in NetSuite. You specify the ID of the record. The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario. When you are configuring this module, the following fields display. Connection For instructions about connecting your NetSuite account to Workfront Fusion, seeCreate a connection to NetSuite in a Workfront Fusion NetSuite module in this article. Record Type Select the type of record that you want the module to read. Outputs Select the fields that you want the module to output. The output for these fields can be mapped in later modules. Internal ID Enter or map the NetSuite ID of the record you want the module to delete. Searches Search for records This search module searches for records based on custom criteria. Connection For instructions about connecting your NetSuite account to Workfront Fusion, seeCreate a connection to NetSuite in a Workfront Fusion NetSuite module in this article. Record Type Select the type of record that you want the module to read. Search criteria Field Select the field that you want to use in your search. The available fields depend on the type of record you want to create. Logical operator Select the operator. This will vary based on the type of field. Value Enter or map the value you want to search for Records to return Select whether you want to return the first matching record, or all matching records. Outputs Select the fields that you want the module to output. The output for these fields can be mapped in later modules. Limit Enter or map the maximum number of records you want the module to return during each scenario execution cycle.
-->

