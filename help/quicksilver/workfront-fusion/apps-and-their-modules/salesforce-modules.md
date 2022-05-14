---
filename: salesforce-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Salesforce modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Salesforce, as well as connect it to to multiple third-party applications and services.
---

# Salesforce modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Salesforce, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Not all editions of Salesforce have API access. For details, see the information about Salesforce editions with API access on the Salesforce Community site.
>* For information on specific errors returned from the Salesforce API, see the Salesforce API docs. You can also check the status of the Salesforce API for any possible service outages.
>

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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

To use Salesforce modules, you must have a Salesforce account.

## About searching for Salesforce objects

When searching for objects, you can either enter individual search words or create a more complex query using wild cards and operators:

* Use the asterisk wild card (&#42;) as a substitute for zero or more characters. For example, a search for Ca&#42; finds items that start with Ca
* Use a question mark wild card (?) as a substitute for a single character. For example, a search for Jo?n finds items with the term John or Joan but not Jon
* Use the quotation marks operator (" ") to find an exact phrase match. For example: "Monday meeting"

For more information about search possibilities, see the Salesforce developer documentation about SOQL and SOSL.

## Salesforce modules and their fields

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

* [Watch for Records](#watch-for-records) 
* [Watch Outbound Messages](#watch-outbound-messages) 
* [Watch a field](#watch-a-field)

#### Watch for Records {#watch-for-records}

This trigger module executes a scenario when a record in an object is created or updated. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Type </td> 
   <td> <p>Select the type of Salesforce record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td>Record Fields</td> 
   <td>Select the fields that you want the module to watch. Available fields depend on the type of record.</td> 
  </tr> 
  <tr> 
   <td>Maximal count of records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td>Watch</td> 
   <td> <p>Determine whether you want the scenario to watch only new records of the type you selected, or new records of the type you selected and all other changes to records of that type.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Outbound Messages {#watch-outbound-messages}

This trigger module executes a scenario when someone sends a message. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span>
-->

This module requires some extra setup:

1. Go to the Salesforce setup page.

   To access the setup page, locate and click the button labeled “Setup” in the upper-right hand corner of the Salesforce account. From the Salesforce setup page, locate the “Quick Find / Search” bar on the left hand side. Search for “Workflow Rules.” 

1. Click **Workflow Rules**. This will take you to .
1. On the the Workflow Rules page that appears, click **New Rule** and select the object type the rule will apply to (such as. “Opportunity” if you are monitoring updates to Opportunity records).
1. Click **Next**.
1. Set a rule name, evaluation criteria, and rule criteria, then click **Save** and **Next**.

1. Click **Done**.
1. From the newly created Workflow rule, click **Edit**..
1. From the **Add Workflow Action** drop-down list, select **New Outbound Message**.

1. Specify name, description, Endpoint URL, and fields you want to include in the new outbound message, then click **Save**.

   The **Endpoint URL** field contains the URL provided on the Salesforce Outbound Message 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   card
   </MadCap:conditionalText>
   -->

   in Workfront Fusion.

1. Configure a scenario beginning with the Outbound Message event. 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   card
   </MadCap:conditionalText>
   -->

1. Click the **</>** icon in the bottom right and copy the provided URL.
1. Return to the **Workflow Rules** page, locate the newly created rule, then click **Activate**.

When you are configuring this module, the following fields display.

<!--
<table data-mc-conditions="QuicksilverOrClassic.Draft mode">
<col>
<col>
<tbody>
<tr>
<td>Connection</td>
<td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td>
</tr>
</tbody>
</table>
-->

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Webhook</td> 
   <td> <p>Select the webhook that you want to use to watch outgoing messages. To add a webhook, click <strong>Add</strong> and enter the webhook's name and connection.</p> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Record Type </td> 
   <td> <p>Select the type of Salesforce record that you want the module to watch for outgoing messages.</p> </td> 
  </tr> 
  <tr> 
   <td>Fields</td> 
   <td> <p>Select the fields that you want the module to watch for outgoing messages. Available fields depend on the type of record.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch a field {#watch-a-field}

This trigger module starts a scenario when a field is updated in Salesforce.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Record Type </td> 
   <td> <p>Select the type of record that contains the field you want the module to watch. You must choose a record type that has Field History turned on in Salesforce setup. For more information, see <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Field History Tracking</a> in the Salesforce documentation. </p> </td> 
  </tr> 
  <tr> 
   <td>Field</td> 
   <td> <p>Select the fields that you want the module to watch for changes.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p>Enter or map the maximum number of fields you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#create-a-record-static-fields" class="MCXref xref">Create a Record (Static Fields)</a> </li>
  -->

* [Create a Record](#create-a-record) 
* [Read a Record](#read-a-record) 
* [Delete a Record](#delete-a-record) 
* [Custom API Call](#custom-api-call) 
* [Upload Attachment/Document](#upload-attachment-document) 
* [Download Attachment/Document](#download-attachment-document)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#update-a-record-static-fields" class="MCXref xref">Update a Record (Static Fields)</a> </li>
  -->

* [Create a Record](#create-a-record)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h4 id="create-a-record-static-fields">Create a Record (Static Fields)</h4>
<p>This action module creates a new record in an object.</p>
<p>You specify the type of record.</p>
<p>The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table>
<col>
<col>
<tbody>
<tr>
<td>Connection</td>
<td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td>
</tr>
<tr>
<td> <p>Record Type </p> </td>
<td> <p>Select the type of Salesforce record that you want the module to create. Fields become available based on the type of record selected in the Record Type field. These fields are based on the Salesforce API.</p> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Create a Record  {#create-a-record}

This action module creates a new record in an object.

The module allows you to select which of the object's fields are available in the module. This reduces the number of fields you must scroll through when setting up the module.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>Record Type </p> </td> 
   <td> <p>Select the type of Salesforce record that you want the module to create. Fields become available based on the type of record selected in the Record Type field. These fields are based on the Salesforce API.</p> </td> 
  </tr> 
  <tr> 
   <td>Select fields to map</td> 
   <td> <p>Select the fields that you want the module to configure when creating the new record. Required fields are at the top of the list. </p> <p>The fields you select open below this field. You can now enter values into these fields.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read a Record {#read-a-record}

This action module reads data from a single object in Salesforce.

You specify the ID of the record.

The module returns the ID of the record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<!--
<table> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Record Type</td>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the type of Salesforce record that you want the module to [action].read.</td>
  </tr> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Record Fields</td>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want the module to read. You must select at least one field.</td>
  </tr> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">ID</td>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Enter or map the unique Salesforce ID of the record that you want the module to read.</p> <p>To get the ID, open the Salesforce object in your browser and copy the text at the end of the URL after the last forward slash (/). For example: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>
-->

#### Delete a Record {#delete-a-record}

This action module deletes an existing record in an object.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Record Type </td> 
   <td> <p>Select the type of Salesforce record that you want the module to delete.</p> </td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td> <p>Enter or map the unique Salesforce ID of the record that you want the module to delete.</p> <p>To get the ID, open the Salesforce object in your browser and copy the text at the end of the URL after the last forward slash (/). For example: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the Salesforce API. This way, you can create a data flow automation that can't be accomplished by the other Salesforce modules.

The module returns the following:

* **Status Code** (number): This indicates the success or failure of your HTTP request. These are standard codes that you can look up on the internet.
* **Headers** (object): A more detailed context for the response/status code that doesn’t relate to the output body. Not all headers that appear in a response header are response headers, so some might not be useful to you.

  The response headers depend on the HTTP request you chose when configuring the module.

* **Body** (object): Depending on the HTTP request you chose when configuring the module, you may receive some data back. That data, such as the data from a GET request, is contained in this object.

When you are configuring this module, the following fields display.

<!--WRITER - check to see if this renders-->

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>For the list of available endpoints, refer to the <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API Developer Guide</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.For example: <code>{“name”:“something-urgent”}</code></p> </td> 
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

**Example:** The following API call returns the list of all users in your Salesforce account:

* **URL**: `query`
* **Method**: GET
* **Query String**:
* **Key**: `q`
* **Value**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`

Matches of the search can be found in the module's Output under **Bundle > Body > records**.

In our example, 6 users were returned:

![](assets/matches-of-the-search-350x573.png)

#### Upload Attachment/Document {#upload-attachment-document}

This action module uploads a file and attaches it to a record you specify, or uploads a document.

The module returns the ID of the attachment or document and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Type of Upload</td> 
   <td>Select whether you want the module to upload an attachment or a document.</td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Enter or map the ID&nbsp;of the object you want to upload an attachment to.</td> 
  </tr> 
  <tr> 
   <td>Folder</td> 
   <td>Select the folder containing the file you want the module to upload. </td> 
  </tr> 
  <tr> 
   <td>Source File</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
 </tbody> 
</table>

#### Download Attachment/Document {#download-attachment-document}

This action module downloads a document or attachment from a record.

You specify the ID of the record and the type of download you want.

The module returns the ID of the  attachment or document and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<!--
<table> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Type of Download</td>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Specify the type of file that you want to download from Salesforce.</p> 
     <ul> 
      <li>Attachment</li> 
      <li>Document</li> 
      <li>ContentDocument (This is a document that has been uploaded to a library in Saleforce CRM Content or Salesforce Files.)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>ID / </p> <p>Attachment ID / </p> <p>ContentDocument ID</p> </td>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Enter or map the unique Salesforce ID of the record that you want the module to download.</p> <p>To get the ID, open the Salesforce object in your browser and copy the text at the end of the URL after the last forward slash (/). For example: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h4 id="update-a-record-static-fields">Update a Record
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Static Fields)
</MadCap:conditionalText>
</h4>
<p>This action module edits a record in an object.</p>
<p>You specify the ID of the record.</p>
<p>The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table>
<col>
<col>
<tbody>
<tr>
<td>Connection</td>
<td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td>
</tr>
<tr>
<td>ID</td>
<td>Enter or map the unique Salesforce ID of the record that you want the module to update.<p>To get the ID, open the Salesforce object in your browser and copy the text at the end of the URL after the last forward slash (/). For example: <code>https://eu5.salesforce.com/<object ID></code></p></td>
</tr>
<tr>
<td>Record Type </td>
<td> <p>Select the type of Salesforce record that you want the module to [action].update. Fields become available based on the type of record selected in the Record Type field. These fields are based on the Salesforce API.</p> </td>
</tr>
</tbody>
</table>
<p>See also the information about working with records in the Salesforce REST API Developer Guide.</p>
</div>
-->

#### Update a Record

This action module edits a record in an object.

The module allows you to select which of the object's fields are available in the module. This reduces the number of fields you must scroll through when setting up the module.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Enter or map the ID&nbsp;of the record that you want to update.</td> 
  </tr> 
  <tr> 
   <td> <p>Record Type </p> </td> 
   <td> <p>Select the type of Salesforce record that you want the module to update. Fields become available based on the type of record selected in the Record Type field. These fields are based on the Salesforce API.</p> </td> 
  </tr> 
  <tr> 
   <td>Select fields to map</td> 
   <td> <p>Select the fields that you want the module to configure when creating the new record. Required fields are at the top of the list. </p> <p>The fields you select open below this field. You can now enter values into these fields.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

#### Search with Query

This search module looks for records in an object in Salesforce that match the search query you specify. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Search Type</td> 
   <td> <p>Select the type of search you want the module to perform:</p> 
    <ul> 
     <li> <p>Simple</p> </li> 
     <li> <p>Using SOSL (Salesforce Object Search Language)</p> </li> 
     <li> <p>Using SOQL (Salesforce Object Query Language)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Type </p> </td> 
   <td> <p>If you selected the Simple search type, choose the type of Salesforce record that you want the module to search for.</p> </td> 
  </tr> 
  <tr> 
   <td>Query / SOSL Query / SOQL Query</td> 
   <td> <p>Enter the query that you want to search by.</p> <p>For more information on SOSL, see <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language (SOSL)</a> in the Salesforce documentation.</p> <p>For more information on SOQL, see <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> in the Salesforce documentation.</p> <p>Note: Please note that the value of the parameter <code>RETURNING </code>influences the output of the module. If you use <code>LIMIT</code>, Fusion will ignore the settings in the Maximal count of records field. If you don't set any limit, Fusion will insert the value LIMIT = Maximal count of records.</p> </td> 
  </tr> 
  <tr> 
   <td>Maximal count of records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search

This action module retrieves all records meeting a given criteria.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your Salesforce account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type</td> 
   <td> <p>Select the type of object that you want to search for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search criteria</td> 
   <td>Select the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field. You can connect queries by using AND or OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Result set</td> 
   <td>Select whether you want the module to return All Matching Records, or the First Matching Record only.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximal</td> 
   <td>Enter or map the maximum number of records you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

