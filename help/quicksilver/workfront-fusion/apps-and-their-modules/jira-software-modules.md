---
title: Jira Software modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Jira] Software, as well as connect it to multiple third-party applications and services.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
---
# [!DNL Jira Software] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Jira Software], as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] or higher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use [!DNL Jira] modules you must have a [!DNL Jira] account.

## Connect [!DNL Jira Software] to [!DNL Workfront Fusion]

Your connection method is based on whether you are using [!DNL Jira Cloud] or [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] to Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] to [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] to [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] to [!DNL Workfront Fusion]

To connect [!DNL Jira Software] to [!DNL Workfront Fusion], you must create an API token and insert it together with your Service URL and Username to the [!UICONTROL Create a connection] field in [!DNL Workfront Fusion].

#### Create an API token in [!DNL Jira] 

1. Go to [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) and log in.
1. Click **[!UICONTROL Create API token]**.
1. Type a name for the token, such as *Workfront Fusion*.
1. Copy the token using the **[!UICONTROL Copy to clipboard]** button.

   >[!IMPORTANT]
   >
   >You can't view the token again after closing this dialog.
1. Store the generated token in a safe place.
1. Continue with [Configure the [!DNL Jira] API token in [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configure the [!DNL Jira] API token in [!DNL Workfront Fusion] 

1. In [!DNL Workfront Fusion], add a [!DNL Jira] module to a scenario to open the **[!UICONTROL Create a connection]** box.
1. Specify the following information:

   * **[!UICONTROL Service URL]**
   * **[!UICONTROL Username]**
   * **[!UICONTROL API token]:**&nbsp;This is the API token you created in the [Create an API token in [!DNL Jira]](#create-an-api-token-in-jira) section of this article.

1. Click [!UICONTROL Continue] to create the connection and return to the module.

### Connect [!DNL Jira Server] to [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

To authorize a connection between [!DNL Workfront Fusion] and [!DNL Jira Server], you need your Consumer Key, Private Key, And Service URL. You might need to contact your [!DNL Jira] administrator for this information.

* [Generate Public and Private keys for your [!DNL Jira] connection](#generate-public-and-private-keys-for-your-jira-connection)
* [Configure the client app as a consumer in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Create a connection to [!DNL Jira] Server or Jira Data Center in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Generate Public and Private keys for your [!DNL Jira] connection 

To acquire a private key for your [!DNL Workfront Fusion Jira] connection, you need to generate public and private keys.

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


1. Continue to [Configure the client app as a consumer in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configure the client app as a consumer in [!DNL Jira] 

1. Log in to your [!DNL Jira] instance.
1. In the left navigation panel, click **[!UICONTROL [!DNL Jira] Settings]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Applications]**> **[!UICONTROL Application links]**.
1. In the **[!UICONTROL Enter the URL of the application you want to link]** field, enter

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Click **[!UICONTROL Create new link]**. Ignore the "No response was received from the URL you entered" error message.
1. In the **[!UICONTROL Link applications]** window, enter values into the **[!UICONTROL Consumer key]** and **[!UICONTROL Shared secret]** fields.

   You can choose the values for these fields.

1. Copy the values of the **[!UICONTROL Consumer key]** and **[!UICONTROL Shared secret]** fields to a secure location.

   You will require these values later in the configuration process.

1. Fill in the URL fields as follows:

   | Field | Description |
   |---|---|
   | [!UICONTROL Request Token URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL Authorization URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL Access Token URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Select the **[!UICONTROL Create incoming link]** checkbox.
1. Click **[!UICONTROL Continue]**.
1. In the **[!UICONTROL Link applications]** window, fill in the following fields:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Paste in the consumer key that you copied to a secure location.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer name]</td> 
      <td>Enter a name of your choice. This name is for your own reference.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public key]</td> 
      <td>Paste in the public key from your <code>[!DNL jira_publickey.pem]</code> file.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Continue]**.
1. Continue to [Create a connection to [!DNL Jira Server] or [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Create a connection to [!DNL Jira Server] or [!DNL Jira Data Center] in [!DNL Workfront Fusion] 

>[!NOTE]
>
>Use the [!DNL Jira Server] app to connect to [!DNL Jira Server] or [!DNL Jira Data Center].
1. In any [!DNL Jira Server] module in [!DNL Workfront Fusion], click **[!UICONTROL Add]** next to the [!UICONTROL connection] field.
1. In the [!UICONTROL Create a connection] panel, fill in the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Enter a name for the connection</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Paste in the consumer key that you copied to a secure location in <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure the client app as a consumer in [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Paste in the private key from the <code>[!DNL jira_privatekey.pcks8]</code> file you created in <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Generate Public and Private keys for your [!DNL Jira] connection</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Enter your [!DNL Jira] instance URL. </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## [!DNL Jira Software] modules and their fields

When you configure [!DNL Jira Software] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Jira Software] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers

#### [!UICONTROL Watch for records]

This trigger module starts a scenario when a record is added, updated, or deleted.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Select the webhook that you want to use to watch for records. </p> <p>To add a new webhook:</p> 
    <ol> 
     <li value="1">Click <strong>[!UICONTROL Add]</strong></li> 
     <li value="2">Enter a name for the webhook.</li> 
     <li value="3"> <p>Select the connection you want to use for your webhook. </p> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </li> 
     <li value="4"> <p>Select the record type that you want the software to watch for:</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL Issue]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Add issue to sprint]](#add-issue-to-sprint)
* [[!UICONTROL Create a Record]](#create-a-record)
* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Delete a record]](#delete-a-record)
* [[!UICONTROL Download an attachment]](#download-an-attachment)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Update a record]](#update-a-record)

#### [!UICONTROL Add issue to sprint]

This action module adds one or more issues to a sprint.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Enter or map the Sprint ID of the sprint that you want to add an issue to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue ID or Keys]</td> 
   <td>Add an Issue ID or Key for each issue you want to add to the sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Record]

This action module creates a new record in Jira.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want the module to create. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Custom API Call]

This action module lets you make a custom authenticated call to the [!DNL Jira Software] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Jira Software] modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Enter a path relative to<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a record]

This action module deletes a particular record.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want the module to delete. </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>Enter or map the ID or Key of the record you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an attachment]

This action module downloads a particular attachment.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the attachment you want to download.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

This action module reads data from a single record in [!DNL Jira Software].

You specify the ID of the record.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Jira] record you want the module to read.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Select the outputs that you want to receive. Output options are available based on the type of record selected in the "[!UICONTROL Record Type]" field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Enter or map the unique [!DNL Jira Software] ID of the record that you want the module to read.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a record]

This action module updates an existing record, such as an issue or project,.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want the module to update. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Transition issue]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>Enter or map the ID or Key of the record you want to update.</td> 
  </tr> 
 </tbody> 
</table>

### Searches 

* [[!UICONTROL List records]](#list-records)
* [[!UICONTROL Search for records]](#search-for-records)

#### [!UICONTROL List records]

This search module retrieves all items of a specific type that match your search query

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want the module to list. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint issue]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Enter or map the maximum number of records you want the module to retrieve during each scenario execution cycle.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Search for records]

This search module looks for records in an object in [!DNL Jira Software] that match the search query you specify.

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Jira Software] account to [!DNL Workfront Fusion], see <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want the module to search for. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Lanuguage)] </p> <p>For more information on JQL, see <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> at the Atlassian help site. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
