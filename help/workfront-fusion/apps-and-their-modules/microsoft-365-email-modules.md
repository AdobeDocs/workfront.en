---
filename: microsoft-365-email-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Email
description: In order to use Office 365 Email with Adobe Workfront Fusion, it is necessary to have an Office 365 account. You can create one at www.office.com.
---

# Microsoft Office 365 Email

In order to use Office 365 Email with `Adobe Workfront Fusion`, it is necessary to have an Office 365 account. You can create one at www.office.com.

For instructions about connecting your `Office 365` account to `Workfront Fusion`, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

After you grant consent, you are redirected back to the `Workfront Fusion` administration page where you can continue creating your scenario.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Microsoft Office 365 Email modules, you must have a Microsoft Office 365 Email account.

## Microsoft Office 365 Email modules and their fields

When you configure `Microsoft Office 365 Email` modules, `Workfront Fusion` displays the fields listed below. Along with these, additional `Microsoft Office 365 Email` fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Message](#message) 
* [Draft Message](#draft) 
* [Attachment](#attachme) 
* [Other](#other)

### Message

* [Watch Messages](#watch) 
* [Search messages](#search) 
* [Get a message](#get) 
* [Create and Send a Message](#create) 
* [Move a Message](#move) 
* [Delete a Message](#delete)

#### Watch Messages

Triggers when a new email message is sent or received.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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
   <td> <p>Enter the maximum number of messages <span>Workfront Fusion</span> should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search messages

Searches for messages based on specific criteria.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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
   <td> <p>Enter the maximum number of messages <span>Workfront Fusion</span> should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a message

Gets the metadata of a specific message

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to retrieve metadata for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get Mime contents</td> 
   <td>Enable this option to retrieve data about the MIME content of the message. MIME content may include images, audio, video, or other types of files.</td> 
  </tr> 
 </tbody> 
</table>

#### Create and Send a Message

Creates and sends an email message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td> <p>Enter or map the subject line of the message.</p> </td> 
  </tr> Body Content Type Select whether the body content of the message is HTML or Text. 
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
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CC Recipients</p> </td> 
   <td> <p>Add the recipients that you want to receive a copy of the message:</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc Recipients</p> </td> 
   <td> <p>Add the recipients that you want to copy on the message, without allowing other recipients to see their names or email addresses:</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add the attachments to the email:</p> 
    <ul> 
     <li> <p><span class="bold">File name</span> </p> <p>Enter the file name. Example: <code>sample.doc</code></p> </li> 
     <li> <p><span class="bold">Data</span> </p> <p>Enter the file data to the field or map the source of the file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Internet Message Headers</td> 
   <td> <p>Add the message headers for the email.</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the header</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter a value for the header.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Move a Message

Moves an email message to a selected folder in the mailbox.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

#### Delete a Message

Deletes an existing email message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Draft Message

* [Create a Draft Message](#create2) 
* [Send a Draft Message](#send) 
* [Update a Message](#update)

#### Create a Draft Message

Creates a new email message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CC Recipients</p> </td> 
   <td> <p>Add the recipients The you want to receive a copy of the message:</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc Recipients</p> </td> 
   <td> <p>Add the recipients that you want to copy on the message, without allowing other recipients to see their names or email addresses:</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add the attachments to the email:</p> 
    <ul> 
     <li> <p><span class="bold">File name</span> </p> <p>Enter the file name. Example: <code>sample.doc</code></p> </li> 
     <li> <p><span class="bold">Data</span> </p> <p>Enter the file data to the field or map the source of the file.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Send a Draft Message

Sends an email message that is currently in draft.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Draft Message ID</td> 
   <td> <p> Select or map the Message ID of the draft you want to send.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Message

Updates an existing message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a message ID</td> 
   <td> <p>Select how you want to identify the message to update:</p> 
    <ul> 
     <li> <p><span class="bold">Enter Manually</span> </p> <p>Enter or map the message ID.</p> </li> 
     <li> <p><span class="bold">Select from the list</span> </p> <p>Select the folder that contains the message you want to update, then select the message</p> </li> 
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
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>CC Recipients</p> </td> 
   <td> <p>Add the recipients The you want to receive a copy of the message:</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc Recipients</p> </td> 
   <td> <p>Add the recipients that you want to copy on the message, without allowing other recipients to see their names or email addresses:</p> 
    <ul> 
     <li> <p><span class="bold">Name</span> </p> <p>Enter the name of the contact</p> </li> 
     <li> <p><span class="bold">Email Address</span> </p> <p>Enter the email address of the contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add the attachments to the email:</p> 
    <ul> 
     <li> <p><span class="bold">File name</span> </p> <p>Enter the file name. Example: <code>sample.doc</code></p> </li> 
     <li> <p><span class="bold">Data</span> </p> <p>Enter the file data to the field or map the source of the file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mark it as Read</td> 
   <td>Enable this option to mark the updated message as read.</td> 
  </tr> 
 </tbody> 
</table>

### Attachment

* [List Attachments](#list) 
* [Download an Attachment](#download)

#### List Attachments

This module retrieves a list of attachments belonging to the specified message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message you want to retrieve attachments from.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of <span>attachment</span>s you want the module to <span>return</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Download an Attachment

This module downloads the specified attachment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Select or map the ID of the message that contains the attachment you want to download.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attachment ID</td> 
   <td> <p>Enter or map the ID&nbsp;of the attachment you want to download.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other

* [Make an API Call](#make) 
* [Add an Attachment](#add)

#### Make an API&nbsp;Call

This module allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to <code>https://graph.microsoft.com</code>. Example:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. <span>Workfront Fusion</span> adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Add the query for the API call in the form of a standard JSON object.</p> </td> 
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

#### Add an Attachment

This module adds a large attachment to a message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <span>Office 365</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

