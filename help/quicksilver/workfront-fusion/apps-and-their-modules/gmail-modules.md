---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Gmail modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Gmail, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
---

# Gmail modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Gmail, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md). For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

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

To use Gmail modules, you must have a Gmail account.

## Connect Gmail to Workfront Fusion {#connect-gmail-to-workfront-fusion}

* [Connect Gmail to Workfront Fusion using G Suite](#connect-gmail-to-workfront-fusion-using-g-suite) 
* [Connect Gmail to Workfront Fusion using gmail.com or googlemail.com](#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com)

### Connect Gmail to Workfront Fusion using G Suite {#connect-gmail-to-workfront-fusion-using-g-suite}

For instructions about connecting your G Suite account to Workfront Fusion, see [Connect the module's app or web service to Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md#connect) in the article [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connect Gmail to Workfront Fusion using gmail.com or googlemail.com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

If you are @gmail.com or @googlemail.com user you must create an OAuth client on the [Google Cloud Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) in order to obtain a Client ID and Client Secret.

For step-by-step instructions on how to create the OAuth client and obtain a Client ID and Client Secret, see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Gmail modules and their fields

When you configure Gmail modules, Workfront Fusion displays the fields listed below. Along with these, additional Gmail fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Iterators](#iterators)

### Triggers {#triggers}

#### Watch emails

This trigger module executes a scenario when a new email is received to be processed.

The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the email folder you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td>Filter type </td> 
   <td> <p>Select the filter type you want to use to watch emails</p> 
    <ul> 
     <li> <p><strong>Simple filter</strong> </p> <p>Fill out the Criteria, Sender Email Address, Subject, and Search Phrase fields</p> </li> 
     <li> <p> <strong>Gmail filter</strong> </p> <p>In the Query field, enter the query that you want to use to filter emails.</p> <p>For more information on Gmail filters, see <a href="https://support.google.com/mail/answer/7190">Search operators</a> in the Gmail documentation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Criteria</td> 
   <td>Select whether you want to watch all email, only read emails, or only unread emails.</td> 
  </tr> 
  <tr> 
   <td>Sender email address</td> 
   <td> <p> Enter an email address to watch only emails sent from that address.</p> </td> 
  </tr> 
  <tr> 
   <td>Subject</td> 
   <td>Enter a text string to watch only emails that have that text string in the subject.</td> 
  </tr> 
  <tr> 
   <td>Search phrase</td> 
   <td>Enter a text string to watch only emails that have that text string anywhere in the email.</td> 
  </tr> 
  <tr> 
   <td>Mark email message(s) as read when fetched</td> 
   <td> <p> Enable this option to mark retrieved emails as read.</p> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of results</td> 
   <td> <p> Set the maximum number of results that Workfront Fusion will work with during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Send an email](#send-an-email) 
* [Create a draft](#create-a-draft) 
* [Mark an email as read](#mark-an-email-as-read) 
* [Mark an email as unread](#mark-an-email-as-unread) 
* [Move an email](#move-an-email) 
* [Copy an email](#copy-an-email) 
* [Delete an email](#delete-an-email) 
* [Modify email labels](#modify-email-labels)

#### Send an email {#send-an-email}

This action module sends a new email.

You specify the recipient of the email.

The module returns the ID of the email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>From</td> 
   <td> <p>Enter or map a sender email address.</p> <p>Note:  If you enter an incorrect email address, an error may occur when sending a message because your account may not have permission to send emails from an address different than your own.</p> </td> 
  </tr> 
  <tr> 
   <td>To </td> 
   <td> <p>Click <strong>Add</strong>, then enter or map the email address for each recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>Subject </td> 
   <td> <p>Enter or map the email subject.</p> </td> 
  </tr> 
  <tr> 
   <td>Content </td> 
   <td> <p>Enter or map the email content (message body). HTML tags are allowed.</p> </td> 
  </tr> 
  <tr> 
   <td>Attachments </td> 
   <td> <p>Click <strong>Add</strong> to add an attachment. You can map a file from the previous modules.</p> </td> 
  </tr> 
  <tr> 
   <td>Copy recipients</td> 
   <td> <p> Click <strong>Add</strong>, then enter or map the email address for each copy recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>Blind copy recipients</td> 
   <td> <p> Click <strong>Add</strong>, then enter or map the email address for each blind copy recipient.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a draft {#create-a-draft}

This action module creates a new email draft and adds it to a folder you specify.

You specify the folder where you want to create a draft.

The module returns the ID of the email draft and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the Gmail folder you want to create a draft in.</p> </td> 
  </tr> 
  <tr> 
   <td>To </td> 
   <td> <p>Click <strong>Add</strong>, then enter or map the email address for each recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>Subject </td> 
   <td> <p>Enter or map the email subject.</p> </td> 
  </tr> 
  <tr> 
   <td>Content </td> 
   <td> <p>Enter or map the email content (message body). HTML tags are allowed.</p> </td> 
  </tr> 
  <tr> 
   <td>Attachments </td> 
   <td> <p>Click <strong>Add</strong> to add an attachment. You can map a file from the previous modules.</p> </td> 
  </tr> 
  <tr> 
   <td>Copy recipients</td> 
   <td> <p> Click <strong>Add</strong>, then enter or map the email address for each copy recipient.</p> </td> 
  </tr> 
  <tr> 
   <td>Blind copy recipients</td> 
   <td> <p> Click <strong>Add</strong>, then enter or map the email address for each blind copy recipient.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Mark an email as read {#mark-an-email-as-read}

This action module marks an email as read.

You specify the ID of the email and its folder.

The module returns the ID of the  email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the Gmail folder that contains the email.</p> </td> 
  </tr> 
  <tr> 
   <td>Email ID (UID)</td> 
   <td> <p> Enter or map the Email ID.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Mark an email as unread {#mark-an-email-as-unread}

This action module marks an email or an email draft as unread.

You specify the ID of the email and its folder.

The module returns the ID of the  email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the Gmail folder that contains the email.</p> </td> 
  </tr> 
  <tr> 
   <td>Email ID (UID) </td> 
   <td> <p>Enter or map the Email ID of the email you want to mark as unread.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Move an email {#move-an-email}

This action module moves an email or an email draft to a folder you specify.

You specify the folder, the destination folder, and the ID of the email..

The module returns the ID of the  email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the Gmail source folder that contains the email you want to move.</p> </td> 
  </tr> 
  <tr> 
   <td>Destination folder</td> 
   <td> <p> Select the Gmail target folder you want to move the email to.</p> </td> 
  </tr> 
  <tr> 
   <td>Email ID (UID)</td> 
   <td> <p> Enter or map the Email ID of the email you want to move.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Copy an email {#copy-an-email}

This action module copies an email or email draft into a folder you specify.

You specify the folder, the destination folder, and the ID of the email..

The module returns the ID of the email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the Gmail source folder that contains the email you want to copy.</p> </td> 
  </tr> 
  <tr> 
   <td>Destination folder</td> 
   <td> <p>Select the Gmail target folder you want to copy the email to.</p> </td> 
  </tr> 
  <tr> 
   <td>Email ID (UID)</td> 
   <td> <p>Enter or map the Email ID of the email you want to copy.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete an email {#delete-an-email}

This action module removes an email or an email draft from a folder you specify.

The module returns the ID of the  email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gmail Message ID</p> </td> 
   <td> <p>Enter or map the Email ID of the email you want to delete.</p> </td> 
  </tr> 
  <tr> 
   <td>Permanently </td> 
   <td> <p>Enable this option to allow the module to permanently delete the email, instead of moving it to the trash folder.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Modify email labels {#modify-email-labels}

This action module modifies the label on an email message you specify.

The module returns the ID of the  email and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on connecting your Gmail account to Workfront Fusion, see <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect Gmail to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Gmail Message ID</td> 
   <td> <p> Enter or map the Email ID of the email you want to delete.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Labels to add</p> </td> 
   <td> <p>Select or map the label you want to add to the selected email message.</p> </td> 
  </tr> 
  <tr> 
   <td>Labels to remove</td> 
   <td> <p> Select or map the label you want to remove from the selected email message.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Label to add and Label to remove fields load only user-created labels.

### Iterators {#iterators}

#### Iterate attachments

You can iterate email attachments. Each attachment is a separate bundle in the module's output. For more information, see [Iterator module in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Source module </td> 
   <td> <p>Select the module you want to iterate attachments from. </p> </td> 
  </tr> 
 </tbody> 
</table>

