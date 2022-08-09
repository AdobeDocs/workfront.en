---
title: Jira Software modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Jira Software, as well as connect it to multiple third-party applications and services.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
---
# Jira Software modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Jira Software, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Jira modules you must have a Jira account.

## Connect Jira Software to Workfront Fusion

Your connection method is based on whether you are using Jira Cloud or Jira Server.

* [Connect Jira Cloud to Workfront Fusion](#connect-jira-cloud-to-workfront-fusion) 
* [Connect Jira Server to Workfront Fusion](#connect-jira-server-to-workfront-fusion)

### Connect Jira Cloud to Workfront Fusion {#connect-jira-cloud-to-workfront-fusion}

Connect Jira Cloud to Workfront Fusion

To connect Jira Software to Workfront Fusion, you must create an API token and insert it together with your Service URL and Username to the Create a connection field in Workfront Fusion.

#### Create an API&nbsp;token in Jira {#create-an-api-token-in-jira}

1. Go to [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) and log in.
1. Click **Create API token**.
1. Type a name for the token, such as *Workfront Fusion*.
1. Copy the token using the **Copy to clipboard** button.

   >[!IMPORTANT]
   >
   >You can't view the token again after closing this dialog.

1. Store the generated token in a safe place.
1. Continue with [Configure the Jira API token in Workfront Fusion](#configure-the-jira-api-token-in-workfront-fusion).

#### Configure the Jira API token in Workfront Fusion {#configure-the-jira-api-token-in-workfront-fusion}

1. In Workfront Fusion, add a Jira module to a scenario to open the **Create a connection** box.
1. Specify the following information:

   * **Service URL** 
   
     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Provide a brief description of what this is.</span>   
     -->

   * **Username: Provide a brief description of what this is.**
   * **API token:**&nbsp;This is the API token you created in the [Create an API token in Jira](#create-an-api-token-in-jira) section of this article.

1. Click Continue to create the connection and return to the module.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">LP: Do you have to hit Save or anything?</p>
   -->

### Connect Jira Server to Workfront Fusion {#connect-jira-server-to-workfront-fusion}

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

To authorize a connection between Workfront Fusion and Jira Server, you need your Consumer Key, Private Key, And Service URL. You might need to contact your Jira administrator for this information.

* [Generate Public and Private keys for your Jira connection](#generate-public-and-private-keys-for-your-jira-connection) 
* [Configure the client app as a consumer in Jira](#configure-the-client-app-as-a-consumer-in-jira) 
* [Create a connection to Jira Server or Jira Data Center in Workfront Fusion](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Generate Public and Private keys for your Jira connection {#generate-public-and-private-keys-for-your-jira-connection}

To acquire a private key for your Workfront Fusion Jira connection, you need to generate public and private keys.

1. In your terminal, run the following `openssl` commands.

   * `openssl genrsa -out jira_privatekey.pem 1024`
   
     This command generates a 1024 bit private key.
   
   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`
   
     This command creates an X509 certificate.
   
   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`
   
     This command extracts the private key (PKCS8 format) to the `jira_privatekey.pcks8` 
     file.
   
   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`
   
     This command extracts the public key from the certificate to the `jira_publickey.pem` file.

     >[!NOTE]
     >
     >If you are using Windows, you might need to save the public key to the `jira_publickey.pem` file manually:
     >
     >1. In your terminal, run the following command:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copy the terminal output (including `-------BEGIN PUBLIC KEY--------` and `-------END PUBLIC KEY--------`
     >   
     >1. Paste the terminal output into a file named `jira_publickey.pem`.

1. Continue to [Configure the client app as a consumer in Jira](#configure-the-client-app-as-a-consumer-in-jira)

#### Configure the client app as a consumer in Jira {#configure-the-client-app-as-a-consumer-in-jira}

1. Log in to your Jira instance.
1. In the left navigation panel, click **Jira Settings** ![](assets/jira-settings-icon.png) > **Applications**> **Application links**.
1. In the **Enter the URL of the application you want to link** field, enter 

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Click **Create new link**. Ignore the "No response was received from the URL you entered" error message.
1. In the **Link applications** window, enter values into the **Consumer key** and **Shared secret** fields.

   You can choose the values for these fields.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">LP: Would it be helpful to provide examples here?</p>
   -->

1. Copy the values of the **Consumer key** and **Shared secret** fields to a secure location.

   You will require these values later in the configuration process.

1. Fill in the URL fields as follows:

   |Field | Description |
   |---|---|
   | Request Token URL |`<Jira base url>/plugins/servlet/oauth/request-token`|
   | Authorization URL |`<Jira base url>/plugins/servlet/oauth/authorize`|
   | Access Token URL |`<Jira base url>/plugins/servlet/oauth/access-token`|

1. Select the **Create incoming link** checkbox.
1. Click **Continue**.
1. In the **Link applications** window, fill in the following fields:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Consumer Key</p> </td> 
      <td> Paste in the consumer key that you copied to a secure location.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consumer name</td> 
      <td>Enter a name of your choice. This name is for your own reference.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Public key</td> 
      <td>Paste in the public key from your <code>jira_publickey.pem</code> file.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue**.
1. Continue to [Create a connection to Jira Server or Jira Data Center in Workfront Fusion](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Create a connection to Jira Server or Jira Data Center in Workfront Fusion {#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion}

>[!NOTE]
>
>Use the Jira Server app to connect to Jira Server or Jira Data Center.

1. In any Jira Server module in Workfront Fusion, click **Add** next to the connection field.
1. In the Create a connection panel, fill in the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Connection name</p> </td> 
      <td> <p>Enter a name for the connection</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consumer Key</td> 
      <td>Paste in the consumer key that you copied to a secure location in <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure the client app as a consumer in Jira</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private Key</td> 
      <td>Paste in the private key from the <code>jira_privatekey.pcks8</code> file you created in <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Generate Public and Private keys for your Jira connection</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Service URL</td> 
      <td>Enter your Jira instance URL. </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue** to create the connection and go back to the module.

## Jira Software modules and their fields

When you configure Jira Software modules, Workfront Fusion displays the fields listed below. Along with these, additional Jira Software fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

#### Watch for records

This trigger module starts a scenario when a record is added, updated, or deleted.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook</td> 
   <td> <p>Select the webhook that you want to use to watch for records. </p> <p>To add a new webhook:</p> 
    <ol> 
     <li value="1">Click <strong>Add</strong></li> 
     <li value="2">Enter a name for the webhook.</li> 
     <li value="3"> <p>Select the connection you want to use for your webhook. </p> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </li> 
     <li value="4"> <p>Select the record type that you want the software to watch for:</p> 
      <ul> 
       <li>Comment </li> 
       <li>Issue</li> 
       <li>Project </li> 
       <li>Sprint</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Add issue to sprint](#add-issue-to-sprint) 
* [Custom API Call](#custom-api-call) 
* [Create a Record](#create-a-record) 
* [Delete a record](#delete-a-record) 
* [Download an attachment](#download-an-attachment) 
* [Read a record](#read-a-record) 
* [Update a record](#update-a-record)

#### Add issue to sprint {#add-issue-to-sprint}

This action module adds one or more issues to a sprint.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sprint ID</td> 
   <td>Enter or map the Sprint ID of the sprint that you want to add an issue to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Issue ID or Keys</td> 
   <td>Add an Issue ID or Key for each issue you want to add to the sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a Record {#create-a-record}

This action module creates a new record in Jira.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to create. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Attachment</li> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>Worklog</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the Jira Software API. This way, you can create a data flow automation that can't be accomplished by the other Jira Software modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to<code>&lt;Instance URL&gt;/rest/api/2/ </code></td> 
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

#### Delete a record {#delete-a-record}

This action module deletes a particular record.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to delete. </p> 
    <ul> 
     <li>Attachment</li> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID or Key</td> 
   <td>Enter or map the ID or Key of the record you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Download an attachment {#download-an-attachment}

This action module downloads a particular attachment.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the ID of the attachment you want to download.</td> 
  </tr> 
 </tbody> 
</table>

#### Read a record {#read-a-record}

This action module reads data from a single record in Jira Software.

You specify the ID of the record.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of Jira record you want the module to read.</p> 
    <ul> 
     <li>Attachment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>User</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the outputs that you want to receive. Output options are available based on the type of record selected in the "Record Type" field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td> <p>Enter or map the unique Jira Software ID of the record that you want the module to read.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a record {#update-a-record}

This action module updates an existing record, such as an issue or project,.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to update. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>Transition issue</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID or Key</td> 
   <td>Enter or map the ID or Key of the record you want to update.</td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

* [List records](#list-records) 
* [Search for records](#search-for-records)

#### List records {#list-records}

This search module retrieves all items of a specific type that match your search query

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to list. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint issue</li> 
     <li>Worklog</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Max Results</p> </td> 
   <td> <p>Enter or map the maximum number of records you want the module to retrieve during each scenario execution cycle.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### Search for records {#search-for-records}

This search module looks for records in an object in Jira Software that match the search query you specify.

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Jira Software account to Workfront Fusion, see <a href="#connect-jira-cloud-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to search for. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Issues</li> 
     <li> <p>Issues by JQL (Jira Query Lanuguage) </p> <p>For more information on JQL, see <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQL stands for Jira Query,project managers%2C and business users.">JQL</a> at the Atlassian help site. </p> </li> 
     <li>Project</li> 
     <li>Project by issue</li> 
     <li>User</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
