---
filename: netsuite
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: NetSuite modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use NetSuite, as well as connect it to to multiple third-party applications and services.
---

# NetSuite modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use NetSuite, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
    </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use NetSuite modules, you must have a NetSuite account.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Connect NetSuite to Workfront Fusion</h2>
<h3>Prerequisites for using NetSuite's REST web services</h3>
<p>To use NetSuite's REST web services, you must first enable the relevant features in your account, and assign the required permissions to the web services user's role. </p> <note type="note">
<p>For instructions on enabling these features and assigning these permissions:</p>
<ul>
<li> <p>See the "REST&nbsp;Web Services Prerequisites and Setup" section of the latest version of Oracle's <a href="https://docs.oracle.com/cloud/latest/netsuitecs_gs/NSTRW/NSTRW.pdf">SuiteTalk REST Web Services</a> documentation.</p> <p>Or</p> </li>
<li> <p>Log in to your Oracle Net Suite account, and search the online documentation for "REST Web Services Prerequisites and Setup."</p> </li>
</ul>
</note>
<ul>
<li> <p><a href="#enable-features" class="MCXref xref">Enable Features</a> </p> </li>
<li> <p><a href="#assign-permissions" class="MCXref xref">Assign permissions</a> </p> </li>
</ul>
<h4 id="enable-features">Enable Features</h4>
<p>Enable the following features</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">REST Web Services feature</td>
<td> <p>To use this feature, you must accept the SuiteCloud Terms of Service.</p> </td>
</tr>
<tr>
<td role="rowheader">REST Record Service (beta) feature</td>
<td> <p>This feature enables you to work with the REST&nbsp;record service beta functionality. </p> <p>Using the REST record service, you can:</p>
<ul>
<li> <p> Perform CRUD operations on beta records</p> </li>
<li> <p>Filter record collections </p> </li>
<li> <p>Interact with record metadata</p> </li>
<li> <p>Perform record actions and transformations.</p> </li>
</ul> <p>To use this feature, you must accept the SuiteCloud Terms of Service.</p> </td>
</tr>
<tr>
<td role="rowheader">REST Query Service (beta) feature</td>
<td>This feature enables you to work with the REST&nbsp;query service beta functionality. Using the REST query service, you can work with datasets and related functionality.</td>
</tr>
<tr>
<td role="rowheader">Suite Analytics Workbook feature</td>
<td>This feature allows you to create workbooks that combine datasets, tables, pivot tables, and charts using the analytics data source.</td>
</tr>
</tbody>
</table> <note type="note">
<p>To access the REST Record Service, REST&nbsp;Query Service, Record Customization, or SuiteScript Workbook API beta features, you must complete the Oracle NetSuite Umbrella Beta Program Recruitment Form. On this form, you must identify an authorized user who can sign to accept the Oracle Cloud Services Beta Trial License Agreement. After this agreement is fully executed by an authorized user through completion of this form, the requested features are available for enablement on this page.</p>
<p>To locate the Oracle NetSuite Umbrella Beta Program Recruitment Form, search the Oracle NetSuite documentation.</p>
</note>
<h4 id="assign-permissions">Assign permissions</h4>
<p>Assign the following permissions:</p>
<ul>
<li> <p>REST Web Services</p> </li>
<li> <p>Log in using Access Tokens</p> </li>
<li> <p>Suite Analytics Workbook</p> </li>
</ul>
<p><strong>Create a new integration record</strong></p>
<p>To set up a connection between NetSuite and Workfront Fusion, you need to create a new integration record in Netsuite.</p> <note type="note">
<p>For instructions on creating a new integration record.</p>
<ul>
<li> <p>See the "Setting Up OAuth 2.0 Authentication for REST Web Services" section of the latest version of Oracle's <a href="https://docs.oracle.com/cloud/latest/netsuitecs_gs/NSTRW/NSTRW.pdf">SuiteTalk REST Web Services</a> documentation.</p> <p>Or</p> </li>
<li> <p>Log in to your Oracle Net Suite account, and search the online documentation for "Create Integration Records for Applications to use Oauth 2.0."</p> </li>
</ul>
</note>
<ol>
<li value="1"> <p>Begin creating a new integration record. </p> <p>When creating the new record, configure the following fields:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Name</td>
<td>Enter a name for your NetSuite integration</td>
</tr>
<tr>
<td role="rowheader">State</td>
<td>Select <strong>Enabled</strong></td>
</tr>
<tr>
<td role="rowheader">Authorization Code Grant</td>
<td>Check this checkbox</td>
</tr>
<tr>
<td role="rowheader">Redirect URI</td>
<td>https://app.workfrontfusion.com/oauth/cb/workfront-netsuite-rest2</td>
</tr>
<tr>
<td role="rowheader">Scope</td>
<td> <p>Check the checkbox next to REST&nbsp;WEB&nbsp;SERVICES.</p> </td>
</tr>
</tbody>
</table> <p> <img src="assets/netsuite-setup-350x275.png" style="width: 350;height: 275;"> </p> </li>
<li value="2"> <p><strong>Save</strong> the new integration.</p> <p>A page showing your client credentials appears.</p> </li>
<li value="3"> <p>Copy and save the client credentials in a secure place. You will need them to create a connection in Workfront Fusion.</p> <note type="warning">
You must copy and save the credentials before you close this window. You will not be able to access them again.
</note> </li>
</ol>
<p><strong>Create a connection to NetSuite in a Workfront Fusion NetSuite module</strong></p>
<p>You can create a connection to your NetSuite account directly from inside a NetSuite module.</p>
<ol>
<li value="1"> <p>In any NetSuite module, click <strong>Add</strong> next to the Connection field.</p> </li>
<li value="2"> <p>Enter the Account ID&nbsp;of the Netsuite account you want the module to access.</p> </li>
<li value="3"> <p>Enter the Client ID and Client Secret that you saved in step 3 in <a href="#create-a-new-integration-record" class="MCXref xref">Create a new integration record</a> above.</p> <note type="note">
For security reasons, the values for Client Credentials are only displayed on the initial setup page. They cannot be retrieved from the system. If you did not save this information, you must reset credentials to obtain new values for your Client Credentials.
</note> </li>
<li value="4"> <p>Click <strong>Continue</strong> to create the connection and go back to the module.</p> </li>
</ol>
</div>
-->

## NetSuite modules and their fields

When you configure NetSuite modules, Workfront Fusion displays the fields listed below. Along with these, additional NetSuite fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<ul>
<li><a href="#triggers" class="MCXref xref">Triggers</a> </li>
<li><a href="#actions" class="MCXref xref">Actions</a> </li>
<li><a href="#searches" class="MCXref xref">Searches</a> </li>
</ul>
<p><strong>Triggers</strong></p>
<h4>Watch records</h4>
<p>This trigger module activates a scenario when a record is created or updated.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
<td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Record type</td>
<td> <p style="color: #000000;">Select the type of record you want to watch.</p> </td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the module output. The available fields depend on the type of record you want to watch.</td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to watch for new records or updated records.</td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Limit</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Set the highest number of records you want the module to return during each scenario execution cycle.</td>
</tr>
</tbody>
</table>
<p><strong>Actions</strong></p>
<ul>
<li> <p><a href="#custom-api-call" class="MCXref xref">Custom API Call</a> </p> </li>
<li> <p><a href="#create-a-record" class="MCXref xref">Create a record</a> </p> </li>
<li> <p><a href="#update-a-record" class="MCXref xref">Update a record</a> </p> </li>
<li> <p><a href="#delete-a-record" class="MCXref xref">Delete a Record</a> </p> </li>
<li> <p><a href="#read-a-record" class="MCXref xref">Read a Record</a> </p> </li>
</ul>
</div>
-->

### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the NetSuite API. This way, you can create a data flow automation that can't be accomplished by the other NetSuite modules.

The action is based on the entity type (Allocadia object type) you specify.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Use the following URL format:</p> <p><code>https://{accountID}.suitetalk.api.netsuite.com/services/rest/record/{version}/{resource}?{query-parameters}</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
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
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h4 id="create-a-record">Create a record</h4>
<p>This action module creates a new record.</p>
<p>You specify the type of record and field values for the new record.</p>
<p>The module returns the ID of the record. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
<td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Record type</td>
<td>
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the type of record you want to create.</p>
</td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Properties</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create.</td>
</tr>
</tbody>
</table>
<h4 id="update-a-record">Update a record</h4>
<p>This action module updates an existing record.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Record type</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the type of record you want to update.</td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Internal ID</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Enter the unique NetSuite ID of the record that you want the module to update</td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Properties</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create.</td>
</tr>
</tbody>
</table>
<h4 id="delete-a-record">Delete a Record</h4>
<p>This action module deletes a single record from NetSuite.</p>
<p>You specify the ID of the record.</p>
<p>The module returns the internal ID of the deleted record.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Connection</td>
<td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Record Type</td>
<td>Select the type of record that you want the module to delete.</td>
</tr>
<tr>
<td role="rowheader">Internal ID</td>
<td>Enter or map the NetSuite ID of the record you want the module to delete.</td>
</tr>
</tbody>
</table>
<h4 id="read-a-record">Read a Record</h4>
<p>This action module reads data from a single record in NetSuite.</p>
<p>You specify the ID of the record.</p>
<p>The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Connection</td>
<td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Record Type</td>
<td>Select the type of record that you want the module to read.</td>
</tr>
<tr>
<td role="rowheader">Outputs</td>
<td>Select the fields that you want the module to output. The output for these fields can be mapped in later modules.</td>
</tr>
<tr>
<td role="rowheader">Internal ID</td>
<td>Enter or map the NetSuite ID of the record you want the module to delete.</td>
</tr>
</tbody>
</table>
<p><strong>Searches</strong></p>
<h4>Search for records</h4>
<p>This search module searches for records based on custom criteria.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Connection</td>
<td> <p>For instructions about connecting your NetSuite account to Workfront Fusion, see<a href="#create-a-connection-to-netsuite-in-a-workfront-fusion-netsuite-module" class="MCXref xref">Create a connection to NetSuite in a Workfront Fusion NetSuite module</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Record Type</td>
<td>Select the type of record that you want the module to read.</td>
</tr>
<tr>
<td role="rowheader">Search criteria</td>
<td>
<ul>
<li> <p><strong>Field</strong> </p> <p>Select the field that you want to use in your search. The available fields depend on the type of record you want to create.</p> </li>
<li> <p><strong>Logical operator</strong> </p> <p>Select the operator. This will vary based on the type of field.</p> </li>
<li> <p><strong>Value</strong> </p> <p>Enter or map the value you want to search for </p> </li>
</ul> </td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td role="rowheader">Records to return</td>
<td>Select whether you want to return the first matching record, or all matching records.</td>
</tr>
<tr>
<td role="rowheader">Outputs</td>
<td>Select the fields that you want the module to output. The output for these fields can be mapped in later modules.</td>
</tr>
<tr>
<td role="rowheader">Limit</td>
<td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td>
</tr>
</tbody>
</table>
</div>
-->
