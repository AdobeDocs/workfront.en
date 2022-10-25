---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Email
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Microsoft Office 365 Email, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
---
# Microsoft Office 365 Email

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Microsoft Office 365 Email, as well as connect it to multiple third-party applications and services.

In order to use Office 365 Email with [!DNL Adobe Workfront Fusion], it is necessary to have an Office 365 account. You can create one at www.office.com.

For instructions about connecting your Office 365 account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

After you grant consent, you are redirected back to the [!UICONTROL Workfront Fusion administration] page where you can continue creating your scenario.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Microsoft Office 365 Email modules, you must have a Microsoft Office 365 Email account.

## Microsoft Office 365 Email modules and their fields

When you configure Microsoft Office 365 Email modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional Microsoft Office 365 Email fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Message](#message)
* [Draft Message](#draft-message)
* [Attachment](#attachment)
* [Other](#other)

### Message {#message}

* [Watch Messages](#watch-messages)
* [Search messages](#search-messages)
* [Get a message](#get-a-message)
* [[!UICONTROL Create and Send a Message]](#create-and-send-a-message)
* [[!UICONTROL Move a Message]](#move-a-message)
* [Delete a Message](#delete-a-message)

#### Watch Messages {#watch-messages}

Triggers when a new email message is sent or received.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Watch Messages</p> </td> 
   <td> <p>Select the messages you want to watch:</p> 
    <ul> 
     <li>Only Unread</li> 
     <li>Only read</li> 
     <li>All</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mail Folder</td> 
   <td> <p>Select the folder that contains the messages you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search</td> 
   <td>Enter your search query. For information on how to write a search query, see the Microsoft support article <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Search Mail and People in Outlook.com</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Enter the maximum number of messages [!DNL Workfront Fusion] should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search messages {#search-messages}

Searches for messages based on specific criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mail Folder</td> 
   <td> <p>Select the folder that contains the messages you want to search.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search</td> 
   <td>Enter your search query. For information on how to write a search query, see the Microsoft support article <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Search Mail and People in Outlook.com</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Order by</td> 
   <td> <p>Select how you want to order the results:</p> 
    <ul> 
     <li>Subject (Ascending or descending)</li> 
     <li>Created Date Time (Ascending or descending)</li> 
     <li>Last Modified Date Time (Ascending or descending)</li> 
     <li>Received Date Time (Ascending or descending)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter the maximum number of messages [!DNL Workfront Fusion] should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a message {#get-a-message}

Gets the metadata of a specific message

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to retrieve metadata for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get MIME contents</td> 
   <td>Enable this option to retrieve data about the MIME content of the message. MIME content may include images, audio, video, or other types of files.</td> 
  </tr> 
 </tbody> 
</table>

#### Create and Send a Message {#create-and-send-a-message}

Creates and sends an email message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td> <p>Enter or map the subject line of the message.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Body Content Type</td> 
   <td>Select whether the body content of the message is HTML or Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content</td> 
   <td> <p>Enter or map the message body text of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importance</td> 
   <td> <p>Select the importance of the email</p> 
    <ul> 
     <li>Low</li> 
     <li>Normal</li> 
     <li>High</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>To Recipients</p> </td> 
   <td> <p>Add the email address to which you want to send the messages:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CC Recipients</p> </td> 
   <td> <p>Add the recipients that you want to receive a copy of the message:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc Recipients</p> </td> 
   <td> <p>Add the recipients that you want to copy on the message, without allowing other recipients to see their names or email addresses:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add the attachments to the email:</p> 
    <ul> 
     <li> <p><strong>File name</strong> </p> <p>Enter the file name. Example: <code>sample.doc</code></p> </li> 
     <li> <p><strong>Data</strong> </p> <p>Enter the file data to the field or map the source of the file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Internet Message Headers</td> 
   <td> <p>Add the message headers for the email.</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the header</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter a value for the header.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Move a Message {#move-a-message}

Moves an email message to a selected folder in the mailbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to move to a different folder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mail Folder </td> 
   <td> <p>Select or map the ID of the folder where you want to move the message.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Message {#delete-a-message}

Deletes an existing email message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Draft Message {#draft-message}

* [Create a Draft Message](#create-a-draft-message)
* [Send a Draft Message](#send-a-draft-message)
* [Update a Message](#update-a-message)

#### Create a Draft Message {#create-a-draft-message}

Creates a new email message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td> <p>Enter the subject line of the message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body Content Type</td> 
   <td>Select whether the body content of the message is HTML or Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content</td> 
   <td> <p>Enter the message body text of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importance</td> 
   <td> <p>Select the importance of the email</p> 
    <ul> 
     <li>Low</li> 
     <li>Normal</li> 
     <li>High</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>To Recipients</p> </td> 
   <td> <p>Add the recipients to which you want to send the messages:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CC Recipients</p> </td> 
   <td> <p>Add the recipients The you want to receive a copy of the message:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc Recipients</p> </td> 
   <td> <p>Add the recipients that you want to copy on the message, without allowing other recipients to see their names or email addresses:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add the attachments to the email:</p> 
    <ul> 
     <li> <p><strong>File name</strong> </p> <p>Enter the file name. Example: <code>sample.doc</code></p> </li> 
     <li> <p><strong>Data</strong> </p> <p>Enter the file data to the field or map the source of the file.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Send a Draft Message {#send-a-draft-message}

Sends an email message that is currently in draft.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Draft Message ID</td> 
   <td> <p> Select or map the Message ID of the draft you want to send.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Message {#update-a-message}

Updates an existing message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a message ID</td> 
   <td> <p>Select how you want to identify the message to update:</p> 
    <ul> 
     <li> <p><strong>Enter Manually</strong> </p> <p>Enter or map the message ID.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the folder that contains the message you want to update, then select the message</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td> <p>Enter the subject line of the message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content</td> 
   <td> <p>Enter the message body text of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importance</td> 
   <td> <p>Select the importance of the email</p> 
    <ul> 
     <li>Low</li> 
     <li>Normal</li> 
     <li>High</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>To Recipients</p> </td> 
   <td> <p>Add the email address to which you want to send the messages:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CC Recipients</p> </td> 
   <td> <p>Add the recipients The you want to receive a copy of the message:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc Recipients</p> </td> 
   <td> <p>Add the recipients that you want to copy on the message, without allowing other recipients to see their names or email addresses:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><strong>Email Address</strong> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add the attachments to the email:</p> 
    <ul> 
     <li> <p><strong>File name</strong> </p> <p>Enter the file name. Example: <code>sample.doc</code></p> </li> 
     <li> <p><strong>Data</strong> </p> <p>Enter the file data to the field or map the source of the file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mark it as Read</td> 
   <td>Enable this option to mark the updated message as read.</td> 
  </tr> 
 </tbody> 
</table>

### Attachment {#attachment}

* [List Attachments](#list-attachments)
* [Download an Attachment](#download-an-attachment)

#### List Attachments {#list-attachments}

This module retrieves a list of attachments belonging to the specified message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to retrieve attachments from.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of attachments you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Download an Attachment {#download-an-attachment}

This module downloads the specified attachment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message that contains the attachment you want to download.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attachment ID</td> 
   <td> <p>Enter or map the ID of the attachment you want to download.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other {#other}

* [Make an API Call](#make-an-api-call)
* [Add an Attachment](#add-an-attachment)

#### Make an API&nbsp;Call {#make-an-api-call}

This module allows you to perform a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to <code>https://graph.microsoft.com</code>. Example:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Add the query for the API call in the form of a standard JSON object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard [!DNL JSON] object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Add an Attachment {#add-an-attachment}

This module adds a large attachment to a message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to add an attachment to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td> <p>Select a file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
 </tbody> 
</table>
