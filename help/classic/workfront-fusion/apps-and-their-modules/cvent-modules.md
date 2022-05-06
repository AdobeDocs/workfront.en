---
filename: cvent-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Cvent modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Cvent, as well as connect it to to multiple third-party applications and services.
---

# Cvent modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

In an Adobe Workfront Fusion scenario, you can automate workflows that use Cvent, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

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
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Cvent modules, you must have a Cvent account.

## Connect Cvent to Adobe Workfront Fusion {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>The Cvent modules work through a SOAP API. To create a connection to Cvent, you must ensure the following:
>
>* You have SOAP access to the Cvent API.
>* The Workfront Fusion IP addresses have been added to your organization's allowlist. 
>
>  For a list of Workfront Fusion IP&nbsp;addresses, see [IP Addresses for accessing Adobe Workfront Fusion](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)
>

You can create a connection to your Cvent account directly from inside a Cvent module.

1. In any Cvent module, click **Add** next to the Connection field.
1. Select the region that you want to connect to.

   * North America
   * Europe
   * Sandbox

1. Click **Continue** to create the connection and go back to the module.

## Cvent modules and their fields

When you configure Cvent modules, Workfront Fusion displays the fields listed below. Along with these, additional Cvent fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions) 
* [Searches](#searches)

### Actions {#actions}

* [Custom API Call](#custom-api-call) 
* [Read a record](#read-a-record) 
* [Register Invitee](#register-invitee) 
* [Add Invitee](#add-invitee) 
* [Delete Contact](#delete-contact) 
* [Update Contact](#update-contact) 
* [Create meeting request](#create-meeting-request)

#### Custom API&nbsp;Call {#custom-api-call}

This action module lets you make a custom authenticated call to the Cvent API. This way, you can create a data flow automation that can't be accomplished by the other Cvent modules.

When you are configuring this module, the following fields display.

The module returns the a status code, along with the headers and body of the API&nbsp;call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operation</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body (XML)</td> 
   <td> <p>Enter or map the body of the API call. This must include only the XML. The module will automatically include authentication headers. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read a record {#read-a-record}

This action module reads information about a specific record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Record type</p> </td> 
   <td>Select the item type of the record you want to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contact / Event / Invitee ID</td> 
   <td> <p>Enter or map the ID of the item you want to read.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the fields that you want to include in the module's output. Fields are available based on the item type you selected.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Register Invitee {#register-invitee}

This action module registers an invitee for an event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Invitee ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the invitee you want to register for an event.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>Enter or map the ID of the event you want to register the invitee for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Add Invitee {#add-invitee}

This action module invites a contact to an event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Contact ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the contact you want to add to an event.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>Enter or map the ID of the event you want to add the contact to.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete Contact  {#delete-contact}

This action module deletes a single contact in Cvent.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contact ID</td> 
   <td> <p>Enter or map the ID of the contact you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update Contact {#update-contact}

This action module updates an existing contact using its ID.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Contact ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the contact you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fields</td> 
   <td> <p>Select the fields that you want to input information for, then fill in the desired values for those fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom fields</td> 
   <td> <p>Select the fields that you want to input information for, then fill in the desired values for those fields.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create meeting request {#create-meeting-request}

This action module adds a meeting request to your account.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Form ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the Form you want to use to create the new meeting request.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Meeting Request Fields</td> 
   <td> <p>Select the meeting request fields that you want to input information for, then fill in the desired values for those fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event Request Fields</td> 
   <td> <p>Select the event request fields that you want to input information for, then fill in the desired values for those fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">RFP Request Fields</td> 
   <td> <p>Select the request for proposal fields that you want to input information for, then fill in the desired values for those fields.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

#### List records

This search module retrieves information about all records of a specific type.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Record type</p> </td> 
   <td> <p>Select the type of record that you want to list.</p> 
    <ul> 
     <li> <p>All events from your Cvent account</p> </li> 
     <li> <p>All sessions for an event</p> </li> 
     <li> <p>All invitees for an event</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>If you are listing invitees or sessions, enter or map the ID&nbsp;of the even that those invitees or sessions are associated with.</p> </td> 
  </tr> 
 </tbody> 
</table>

