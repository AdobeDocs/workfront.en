---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Cvent modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Cvent, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
---
# Cvent modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Cvent, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

To use Cvent modules, you must have a Cvent account.

## Connect Cvent to Adobe Workfront Fusion {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>The Cvent modules work through a SOAP API. To create a connection to Cvent, you must ensure the following:
>
>* You have SOAP access to the [!DNL Cvent] API.
>* The [!DNL Workfront Fusion] IP addresses have been added to your organization's allowlist.
>
>  For a list of [!DNL Workfront] Fusion IP&nbsp;addresses, see [IP Addresses for accessing Adobe Workfront Fusion](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


You can create a connection to your Cvent account directly from inside a Cvent module.

1. In any Cvent module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. Select the region that you want to connect to.

   * North America
   * Europe
   * Sandbox

1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## Cvent modules and their fields

When you configure Cvent modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional Cvent fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Searches](#searches)

### Actions {#actions}

* [Custom API Call](#custom-api-call)
* [[!UICONTROL Read a record]](#read-a-record)
* [Register Invitee](#register-invitee)
* [Add Invitee](#add-invitee)
* [Delete Contact](#delete-contact)
* [Update Contact](#update-contact)
* [Create meeting request](#create-meeting-request)

#### Custom API&nbsp;Call {#custom-api-call}

This action module lets you make a custom authenticated call to the Cvent API. This way, you can create a data flow automation that can't be accomplished by the other Cvent modules.

When you are configuring this module, the following fields display.

The module returns the a status code, along with the headers and body of the API&nbsp;call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operation</td> 
   td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body (XML)</td> 
   <td> <p>Enter or map the body of the API call. This must include only the XML. The module will automatically include authentication headers. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read a record {#read-a-record}

This action module reads information about a specific record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
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

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Invitee ID</p> </td> 
   <td> <p>Enter or map the ID of the invitee you want to register for an event.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>Enter or map the ID of the event you want to register the invitee for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Add Invitee {#add-invitee}

This action module invites a contact to an event.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Contact ID</p> </td> 
   <td> <p>Enter or map the ID of the contact you want to add to an event.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>Enter or map the ID of the event you want to add the contact to.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete Contact  {#delete-contact}

This action module deletes a single contact in Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contact ID</td> 
   <td> <p>Enter or map the ID of the contact you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update Contact {#update-contact}

This action module updates an existing contact using its ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Contact ID</p> </td> 
   <td> <p>Enter or map the ID of the contact you want to update.</p> </td> 
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

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Form ID</p> </td> 
   <td> <p>Enter or map the ID of the Form you want to use to create the new meeting request.</p> </td> 
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

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Cvent account to Workfront Fusion, see <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!UICONTROL Connect] Cvent to Adobe Workfront Fusion</a> in this article.</p> </td> 
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
   <td> <p>If you are listing invitees or sessions, enter or map the ID of the even that those invitees or sessions are associated with.</p> </td> 
  </tr> 
 </tbody> 
</table>
