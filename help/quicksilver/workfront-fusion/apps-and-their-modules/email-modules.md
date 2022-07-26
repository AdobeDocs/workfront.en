---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Email modules
description: In a Adobe Workfront Fusion scenario, you can connect your Email account to multiple third-party applications and services.This allows you to download emails via IMAP, send emails via SMTP, create new drafts, move and copy emails from one folder to another folder, mark emails as read or unread, and delete emails.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
---
# Email modules

In a Adobe Workfront Fusion scenario, you can connect your Email account to multiple third-party applications and services.This allows you to download emails via IMAP, send emails via SMTP, create new drafts, move and copy emails from one folder to another folder, mark emails as read or unread, and delete emails.

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

## Connect your email to Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Connect to Google](#connect-to-google) 
* [Connect to other email services (SMAP)](#connect-to-other-email-services-smap)

### Connect to Google {#connect-to-google}

Use this option to create scenarios with email modules that require a connection to your Google account. This is an account with restricted scopes.

You can create a connection to your Google account directly from inside an Allocadia module.

1. In any Email module, click **Add** next to the Connection field.
1. Select **Google** as the connection type.
1. Enter a name for the connection.
1. (Optional) Enter your Google Client ID and Client Secret.
1. Click **Continue** to create the connection and go back to the module.

### Connect to other email services (SMAP) {#connect-to-other-email-services-smap}

SMAP connection allows you to access your mailbox remotely and read or manipulate messages in your mailbox. SMAP connection is used by most of the Email modules.

1. In any Email module, click **Add** next to the Connection field.
1. Select **Others (SMTP)**as the connection type.
1. Enter a **Name** for the connection.
1. Select your **Email provider** from the list. If your email provider is not on the list, select Other.
1. Enter your **Email address**, **Your full name**, your **User name**, and your **Password**.
1. (Conditional) If your provider is not on the list, enter your **SMTP server** and **Port**, and specify whether you want to **Use a secure connection (TLS)**. To find this information, check the Help section for your mailbox. If you don't have this information available, contact your email service provider.
1. Click **Continue** to create the connection and go back to the module.

## Email modules and their fields

When you configure email modules, Workfront Fusion displays the fields listed below. Along with these, additional email fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

Some of the email fields might already contain data because you used them in another module in the scenario. See the email help documentation if you need information about them.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>The Unique Email ID known as 'Email ID (UID)' is the email's identifier. The Email ID is specific for each of the email's folders.

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Iterators](#iterators)

### Triggers {#triggers}

#### Watch Emails

Triggers when a new email is received for processing according to specified criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder </td> 
   <td> <p>Select the folder that contains emails you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criteria</p> </td> 
   <td> <p>Select the criteria by which you want to watch emails:</p> 
    <ul> 
     <li>All Emails</li> 
     <li>Only Read Emails</li> 
     <li>Only Unread Emails</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sender Email Address </td> 
   <td> <p>Enter the email address of the sender whose emails you want to watch.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Recipient Email Address</td> 
   <td> <p> Enter the email address of the recipient whose emails you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject </td> 
   <td> <p>Enter the subject of the email you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Phrase </td> 
   <td> <p>Enter any keywords to watch only those emails containing specific phrases.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mark message(s) as read when fetched</td> 
   <td> <p>Enable this option to mark the unread email as read after retrieving the details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of results</td> 
   <td> <p> The maximum number of emails Workfront Fusion should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Send an Email](#send-an-email) 
* [Create a Draft](#create-a-draft) 
* [Mark an Email as Read](#mark-an-email-as-read) 
* [Mark an Email as Unread](#mark-an-email-as-unread) 
* [Move an Email](#move-an-email) 
* [Copy an Email](#copy-an-email) 
* [Delete an Email](#delete-an-email) 
* [Get Emails](#get-emails) 
* [Send me an Email](#send-me-an-email)

#### Send an Email {#send-an-email}

Sends a new email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Save Message after Sending</td> 
   <td>After the email message is sent, it will be saved in your mailbox. Enable this option if you want to save emails sent using Workfront Fusion to the <i>Sent mail</i> folder or another folder in your mailbox. Some email services, such as Gmail, save sent messages automatically.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">To </td> 
   <td> <p>Add the email addresses you want to send the email to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject </td> 
   <td> <p>Enter or map the subject line of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Content Type</p> </td> 
   <td> <p>Select the content type for the email:</p> 
    <ul> 
     <li>HTML</li> 
     <li>Plaintext</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Content </td> 
   <td> <p>Enter or map the email content in HTML format using HTML tags, or in the plain text, depending on what you chose in the Content Type field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add an attachment:</p> 
    <ul> 
     <li> <p><strong>File name</strong> </p> <p>Enter the file name. For example, sample.doc.</p> </li> 
     <li> <p><strong>Data</strong> </p> <p>Enter the path to the folder to upload the attachment.</p> </li> 
     <li> <p><strong>Content-ID</strong> </p> <p>Enter the content ID to insert the attachment (image) in the content.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Copy Recipient </td> 
   <td> <p>Enter or map one or more email addresses to which you want to send a copy of this email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Blind Copy Recipient</td> 
   <td> <p> Enter or map one or more email addresses to which you want to send a copy of this email without having the email address appear in the email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">From </td> 
   <td> <p>Enter or map the email address (and name, if needed) that appears in the From field in the email. </p> <p>Important: Use the correct syntax: <code>name@email.com</code> or <code>"Name" name@email.com</code>.</p> <p>Note:  Normally, Workfront Fusion uses the email address that you entered when creating the connection as the sender address. If you enter any other email address, an error may occur when sending a message because your account may not have permission to send emails from a different address than your own. E.g. <code>test@mail.com</code> or "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sender</p> </td> 
   <td> <p>Enter or map the email address that appears in the Sender field in the email.</p> <p>Tip:  If you are unsure whether to use this field or the From field, we recommend choosing the From field.</p> <p>Important: Use the correct syntax: <code>name@email.com</code> or <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reply-To</td> 
   <td> <p> If you want replies to this email sent to a different address than the "from" address, enter the email address where you want replies to this email sent.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">In-Reply-To</td> 
   <td> <p> If you are replying to a specific email, enter or map the ID of the email you are replying to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">References </td> 
   <td> <p>Enter the message IDs of all the replies in the thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Priority</p> </td> 
   <td> <p>Select the priority of the email:</p> 
    <ul> 
     <li>High</li> 
     <li>Normal</li> 
     <li>Low</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Headers</p> </td> 
   <td> <p>Add the headers:</p> 
    <ul> 
     <li> <p><strong>Key</strong> </p> <p>Add the key. For example, Sender, Date, To, and so on.</p> </li> 
     <li> <p><strong>Value</strong> </p> <p>Enter the value for the key.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Draft {#create-a-draft}

Creates and adds a new draft to a selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td>Select the folder in which you want to create the draft email.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">To </td> 
   <td> <p>Enter or map the email address to which you want to send the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject </td> 
   <td> <p>Enter or map the subject line of the email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Content Type</p> </td> 
   <td> <p>Select the content type for the email:</p> 
    <ul> 
     <li>HTML</li> 
     <li>Plain Text</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Content </td> 
   <td> <p>Enter or map the email content in HTML format using HTML tags, or in the plain text, depending on what you chose in the Content Type field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add an attachment:</p> 
    <ul> 
     <li> <p><strong>File name</strong> </p> <p>Enter the file name. For example, sample.doc.</p> </li> 
     <li> <p><strong>Data</strong> </p> <p>Enter the path to the folder to upload the attachment.</p> </li> 
     <li> <p><strong>Content-ID</strong> </p> <p>Enter the content ID to insert the attachment (image) in the content.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Copy Recipient </td> 
   <td> <p>Enter or map one or more email addresses to which you want to send a copy of this email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Blind Copy Recipient</td> 
   <td> <p> Enter or map one or more email addresses to which you want to send a copy of this email without having the email address appear in the email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">From </td> 
   <td> <p>Enter or map the email address (and name, if needed) that appears in the From field in the email. </p> <p>Important: Use the correct syntax: <code>name@email.com</code> or <code>"Name" name@email.com</code>.</p> <p>Note:  Normally, Workfront Fusion uses the email address that you entered when creating the connection as the sender address. If you enter any other email address, an error may occur when sending a message because your account may not have permission to send emails from a different address than your own. E.g. <code>test@mail.com</code> or "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Sender</p> </td> 
   <td> <p>Enter or map the email address that appears in the Sender field in the email.</p> <p>Tip:  If you are unsure whether to use this field or the From field, we recommend choosing the From field.</p> <p>Important: Use the correct syntax: <code>name@email.com</code> or <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Reply-To</td> 
   <td> <p> If you want replies to this email sent to a different address than the "from" address, enter the email address where you want replies to this email sent.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">In-Reply-To</td> 
   <td> <p> If you are replying to a specific email, enter or map the ID of the email you are replying to.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">References </td> 
   <td> <p>Enter the message IDs of all the replies in the thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Priority</p> </td> 
   <td> <p>Select the priority of the email:</p> 
    <ul> 
     <li>High</li> 
     <li>Normal</li> 
     <li>Low</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Headers</p> </td> 
   <td> <p>Add the headers:</p> 
    <ul> 
     <li> <p><strong>Key</strong> </p> <p>Add the key. For example, Sender, Date, To, and so on.</p> </li> 
     <li> <p><strong>Value</strong> </p> <p>Enter the value for the key.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Mark an Email as Read {#mark-an-email-as-read}

Marks an email or a draft in a selected folder as read by setting the Read flag.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td>Select the folder of the email you want to mark as read. Example: Primary.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email ID (UID)</p> </td> 
   <td> <p>Enter the Email UID of the email you want to mark as read.</p> <p>You can get the UID of the email by using the Email &gt; Watch Email module or Search Email module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Mark an Email as Unread {#mark-an-email-as-unread}

Marks an email or a draft in a selected folder as unread by setting the Unread flag.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td>Select the folder of the email you want to mark as unread. Example: Primary.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email ID (UID)</p> </td> 
   <td> <p>Enter the Email UID of the email you want to mark as unread.</p> <p>You can get the UID of the email by using the Email &gt; Watch Email module or Search Email module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Move an Email {#move-an-email}

Moves a chosen email or a draft to a selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source Folder</td> 
   <td>Select the folder that contains the email from which you want to move the email. Example: Primary.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Destination Folder</td> 
   <td> <p> Select the folder to which you want to add the email. Example: Work.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email ID (UID)</p> </td> 
   <td> <p>Enter the Email UID of the email you want to move to the destination folder.</p> <p>You can get the UID of the email by using the Email &gt; Watch Email module or Search Email module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Copy an Email {#copy-an-email}

Copies an email or a draft into a selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source Folder</td> 
   <td>Select the folder from which you want to copy the email. Example: Primary.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Destination Folder</td> 
   <td> <p> Select the folder to which you want to copy the email. Example: Work.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email ID (UID)</p> </td> 
   <td> <p>Enter the Email UID of the email you want to copy to the destination folder.</p> <p>You can get the UID of the email by using the Email &gt; Watch Email module or Search Email module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete an Email {#delete-an-email}

Removes an email or a draft from the selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td>Select the folder of the email you want to delete. Example: Primary.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email ID (UID)</p> </td> 
   <td> <p>Enter the Email UID of the email you want to delete.</p> <p>You can get the UID of the email by using the Email &gt; Watch Email module or Search Email module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Expunge</td> 
   <td> <p>Enable this option to allow the module to permanently remove all messages flagged as Deleted in the currently open mailbox.</p> <p>Note: In Gmail, this behavior is driven by the setting in Settings &gt; Forwarding POP/IMAP in IMAP access section.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get Emails {#get-emails}

Returns emails that match the specified criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your email account to Workfront Fusion, see <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connect your email to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder </td> 
   <td> <p>Select the folder that contains the emails you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mark message(s) as read when fetched </td> 
   <td> <p>Enable this option if you want to mark the unread email as read after retrieving the details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criteria</p> </td> 
   <td> <p>Select the criteria of the emails you want to retrieve:</p> 
    <ul> 
     <li>All Emails</li> 
     <li>Only Read Emails</li> 
     <li>Only Unread Emails</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sender Email Address </td> 
   <td> <p>Enter or map the email address of the sender whose emails you want to retrieve.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Recipient Email Address</td> 
   <td> <p> Enter or map the email address of the recipient whose emails you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">From date </td> 
   <td> <p>Enter or map the date to retrieve the emails processed on or after the specified date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Before date</td> 
   <td> <p> Enter or map the date to retrieve the emails processed on or before the specified date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject </td> 
   <td> <p>Enter or map the subject of the email you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Phrase </td> 
   <td> <p>Enter or map any keywords to retrieve only those emails containing specific phrases.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email ID (UID)</td> 
   <td> <p> Enter the Email ID (UID) of the email whose details you want to retrieve.</p> <p>You can get the UID of the email by using Workfront Fusion's Watch Email module or Search Email module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of results</td> 
   <td> <p> The maximum number of emails Workfront Fusion should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Continue the execution of the route even if the module returns no results</td> 
   <td> <p> Select if you want to continue to run the module even if there are no results returned.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Send me an Email {#send-me-an-email}

Sends a new email to your email address.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Subject </td> 
   <td> <p>Enter or map the subject line of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Content </td> 
   <td> <p>Enter the body of the email.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iterators {#iterators}

#### Iterate Attachments

Iterates received attachments one by one.

The email iterator module lets you manage email attachments separately. For example, you can set up to watch emails to iterate the emails with attachments and receive alerts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Source module</td> 
   <td> <p>Select the module that outputs the email with the attachments that you want to iterate through.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more information about iterators, see [Iterator module in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).
