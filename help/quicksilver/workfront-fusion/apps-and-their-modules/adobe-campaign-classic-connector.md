---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic modules
description: With the [!DNL Adobe Campaign Classic] modules, you can start an [!DNL Adobe Workfront Fusion] scenario based on events in your [!DNL Adobe Campaign Classic] account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
---
# [!DNL Adobe Campaign Classic] modules

With the [!DNL Adobe Campaign Classic] modules, you can start an [!DNL Adobe Workfront Fusion] scenario based on events in your [!DNL Adobe Campaign Classic] account, create, read, or update records, search for records using criteria you set, and perform custom API calls.

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

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Adobe Campaign Classic] to [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>We highly recommend creating a server-to-server connection. Adobe Campaign has updated their API to accept only server-to-server connections. If you are connecting to Campaign version 8 or higher, you **must** create a server-to-server connection. 
>
>For more information about Campaign's new connection requirements, see [Migration of Campaign technical operators to Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) in the Campaign documentation.

1. In any [!DNL Adobe Campaign Classic] module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. Fill in the following fields:
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>Select whether you are creating a basic connection or a server-to-server connection.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Enter a name for this connection.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Base URL]</td>
          <td>Enter the base URL that you use to connect to your [!DNL Adobe Campaign Classic] instance.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Username]</td>
          <td>If you are creating a basic connection, enter your Adobe Campaign username.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Password]</td>
          <td>If you are creating a basic connection, enter your Adobe Campaign password.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>If you are creating a server-to-server connection, enter your [!DNL Adobe] [!UICONTROL Client ID]. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>If you are creating a server-to-server connection, enter your [!DNL Adobe] [!UICONTROL Client Secret]. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Select whether you are connection to a Production or Non-production environment.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Select whether you are connecting to a service account or a personal account.
        </tr>
   </tbody>
    </table>
1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## [!DNL Adobe Campaign Classic] modules and their fields

When you configure [!DNL Adobe Campaign Classic] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Campaign Classic] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers

#### [!UICONTROL Watch records]

This scheduled trigger module starts a scenario when a record changes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Select whether you want to watch for new records, updated records, or both.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Select the resource that you want to watch for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output]</td> 
   <td>Select the fields that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>For each custom field that you want to include in output, click <b>[!UICONTROL Add]</b> and enter the name of the custom field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>


### Actions

* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Delete a record]](#delete-record)
* [[!UICONTROL Perform an action]](#perform-an-action)
* [[!UICONTROL Read a record]](#-read-a-record)
* [[!UICONTROL Subscribe or unsubscribe]](#subscribe-or-unsubscribe)
* [[!UICONTROL Update a record]](#update-record)

#### [!UICONTROL Create a record]

This action module creates a new record in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Select the type of [!DNL Adobe Campaign Classic] record you want to create.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Select the fields that you want to set values for when the record is created, then fill in the values for those fields. Fields vary based on the type of record you select.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> For each custom field that you want to add to the new record, click <b>[!UICONTROL Add item]</b> and enter or map the field's name and value. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make a custom API call]

This module makes a custom API call to the [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Select the action that you want the API call to perform.</p>
      <p>[!UICONTROL Execute query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Get entity if more recent]</p>
      <p>[!UICONTROL Select all]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds the [!UICONTROL x-security] token header automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Add the body content for the API call in XML, without the session element. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Delete Record]

This action module deletes a single record from [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Select the type of resource that you want to delete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the resourece you want to delete.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Perform an action]

This action module performs a selected action on an object in the [!DNL Adobe Campaign Classic] API.

For information on specific actions and fields, see [[!DNL Adobe Campaign] - API Documentation](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Select the action to perform on the object.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> For available fields, see <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in this article. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> For available fields, see <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in this article. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> For available fields, see <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Create a record]</a> in this article. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> For available fields, see <a href="#update-record" class="MCXref xref" >[!UICONTROL Update a record]</a> in this article. </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> For available fields, see <a href="#delete-record" class="MCXref xref" >[!UICONTROL Delete a record]</a> in this article. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

This action module reads a record from [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Select the type of [!DNL Adobe Campaign Classic] record you want to read.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Enter of map the ID of the record you want to read.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output] </td> 
   <td>Select the fields that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>For each custom field that you want to include in output, click <b>[!UICONTROL Add]</b> and enter the name of the custom field.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Subscribe or unsubscribe]

This action module subscribes a user to or unsubscribes a user from an information service.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe or unsubscribe]</td> 
   <td>Select whether you want to subscribe or unsubscribe to the information service.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>Select the service that you want to subscribe to or unsubscribe from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient email address] </td> 
   <td>Enter or map the email address of the user you want to subscribe or unsubscribe to the information service.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update record]

This action module updates a single record in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Select the type of [!DNL Adobe Campaign Classic] record you want to create.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Enter of map the ID of the record you want to update.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Select the fields that you want to update values for, then fill in the values for those fields. Fields vary based on the type of record you select.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> For each custom field that you want to update, click <b>[!UICONTROL Add item]</b> and enter or map the field's name and value. </td> 
  </tr> 
 </tbody> 
</table>

### Searches

#### [!UICONTROL Search]

This search module returns records based on the specified criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Campaign Classic], see <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to [!DNL Adobe Campaign Classic]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Select the type of [!DNL Adobe Campaign Classic] record you want to create.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>
