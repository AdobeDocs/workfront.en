---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Journey Optimizer], as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
hide: yes
hidefromtoc: yes
---
# [!DNL Adobe Journey Optimizer] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Journey Optimizer], as well as connect it to multiple third-party applications and services. [!DNL Adobe Journey Optimizer] modules allow you to create, read, update, or delete records, or perform a custom API call to the [!DNL Adobe Journey Optimizer] API.


If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
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

## Prerequisites

Before you can use the [!DNL Adobe Journey Optimizer] connector, you must ensure that the following prerequisites are met:

* You must have an active [!DNL Adobe Journey Optimizer] account.

## Create a connection to Adobe Journey Optimizer

You can create a connection in any Adobe Journey Optimizer module.

1. Click **[!UICONTROL Add]** next to the Connection box.
    
1. Fill in the following fields:
    
    <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Select whether you are connecting to a production or non-production environment.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Select whether you are connecting to a service account or a personal account.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!UICONTROL Adobe] [!UICONTROL Client ID]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Adobe] [!UICONTROL Client Secret]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Enter your [!DNL Adobe] [!UICONTROL Organization ID]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

   
## [!DNL Adobe Journey Optimizer] modules and their fields

When you configure [!DNL Adobe Journey Optimizer] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Journey Optimizer] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Check if configuration can be deployed](#check-if-configuration-can-be-deployed)
* [Check service health](#check-service-health)
<!--* [Copy artifacts synchronously](#copy-artifacts-synchronously)-->
* [Create a configuration](#create-a-configuration)
* [Create a record](#create-a-record)
* [Delete a configuration](#delete-a-configuration)
* [Delete a record](#delete-a-record)
* [Deploy a configuration](#deploy-a-configuration)
<!--* [Export artifacts asynchronously](#export-artifacts-asynchronously)-->
* [Get a configuration](#get-a-configuration)
* [Get a record](#get-a-record)
<!--* [Import artifacts asynchronously](#import-artifacts-asynchronously)-->
* [Make a custom API call](#make-a-custom-api-call)
* [Patch a record](#patch-a-record)
<!--[Status for audience-based message](#status-for-audience-based-message)-->
<!--* [Trigger an audience-based message](#trigger-an-audience-based-message)-->
<!--* [Trigger a unitary message execution](#trigger-a-unitary-message-execution)-->
* [Undeploy a configuration](#undeploy-a-configuration)
* [Update a configuration](#update-a-configuration)
* [Update a record](#update-a-record)
* [List configurations](#list-configurations)
* [List records](#list-records)

### Check if configuration can be deployed

This action module verifies whether a capping or throttling configuration can be deployed.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are checking a capping configuration or a throttling configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Enter or map the ID of the configuration you want to check.</td> 
  </tr> 
 </tbody> 
</table>

### Check service health

This action module checks that the service represented by the connection is running.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
 </tbody> 
</table>

### Copy artifacts synchronously

This action module copies artifacts from a source sandbox into a destination sandbox.



### Create a configuration

This action module creates a capping endpoint or throttling configuration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are creating a capping configuration or a throttling configuration.<ul><li><p><b>Capping</b></p>Continue to <a href="#capping-fields" class="MCXref xref" >Capping fields</a>.</li><li><p><b>Throttling</b></p>Continue to <a href="#throttling-fields" class="MCXref xref" >Throttling fields</a>.</li></ul></td> 
  </tr> 
   </tbody> 
</table>

#### Capping fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Enter or map the URL of the endpoint you want to configure.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IMS organization ID]</td> 
   <td>Enter or map the Adobe IMS ID of the organization.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methods]</td> 
   <td>Select the methods to use in this configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service]</td> 
   <td>Select whether you are using an action or a datasource for this configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum HTTP connections]</td> 
   <td>Enter or map the maximum number of simultaneous connections to this endpoint.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum calls]</td> 
   <td>Enter or map the maximum number of calls to be performed in the period specified in the Time period field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Time period (milliseconds)]</td> 
   <td>Enter or map the number of milliseconds that relates to the Maximum calls field.</td> 
  </tr> 
 </tbody> 
</table>

#### Throttling fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for this configuration.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for this configuration.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL URL pattern]</td> 
   <td>Enter or map the URL for the endpoint you want to throttle.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methods]</td> 
   <td>Select the methods to use in this configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max throughput]</td> 
   <td>Select whether you are using an action or a datasource for this configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum HTTP connections]</td> 
   <td>Enter or map the maximum number of simultaneous connections to this endpoint.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum calls]</td> 
   <td>Enter or map the maximum throughput that you want for this endpoint. This value must be between 200 and 5000.</td> 
  </tr> 
 </tbody> 
</table>

### Create a record

This action module creates a new content template or content fragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Select whether you are creating a content template or a content fragment.<ul><li><p><b>Content template</b></p>Continue to <a href="#template-fields" class="MCXref xref" >Template fields</a>.</li><li><p><b>Content fragment</b></p>Continue to <a href="#fragment-fields" class="MCXref xref" >Fragment fields</a>.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

#### Template fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for this content template.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for this content template.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Select the type of template that you want to create.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td>Select the channels included in this template.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content template origin]</td> 
   <td>Select the source for this template.</td>  
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>To include custom properties in the new template, select "Add metadata" and enter or map the metadata's key and value. Repeat for each custom field you want to include.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email HTML]</td> 
   <td>Enter or map the HTML of the email included in this template.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>To include custom properties in the email, select "Add editor context" and enter or map the context's key and value. Repeat for each custom field you want to include.</td> 
  </tr> 
 </tbody> 
</table>

#### Fragment fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for this content fragment.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for this content fragment.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Select the type of template that you want to create.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td>Select the channels included in this template.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content fragment origin]</td> 
   <td>Select the source for this fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>To include custom properties in the new template, select "Add metadata" and enter or map the metadata's key and value. Repeat for each custom field you want to include.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td>Enter or map the content of the fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>To include custom properties in the email, select "Add editor context" and enter or map the context's key and value. Repeat for each custom field you want to include.</td> 
  </tr> 
 </tbody> 
</table>

### Delete a configuration

This action module deletes a capping endpoint or throttling configuration.

If the configuration has been deployed, it must be undeployed before it can be deleted.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are deleting a capping configuration or a throttling configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Enter or map the ID of the configuration you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

### Delete a record

This action module deletes a content template or content fragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Select whether you are deleting a content template or content fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template/Fragment ID]</td> 
   <td>Enter or map the ID of the template or fragment you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

### Deploy a configuration

This action module deploys the specified capping or throttling configuration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are deploying a capping configuration or a throttling configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Enter or map the ID of the configuration you want to deploy.</td> 
  </tr> 
 </tbody> 
</table>

### Export Artifacts asynchronously

### Get a configuration

This action module returns the capping or throttling configuration identified by the specified ID. The latest definition is returned.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are retrieving a capping configuration or a throttling configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Enter or map the ID of the configuration you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>


### Get a record

This action module returns the content template or content fragment identified by the specified ID. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Select whether you are retrieving a content template or content fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template/Fragment ID]</td> 
   <td>Enter or map the ID of the template or fragment you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>

### Import Artifacts asynchronously



### List records

This action module lists all capping or throttling configurations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Select whether you are retrieving a content template or content fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td>Enter or map the parameter name that you want to sort this list by. Add <code>-</code> or <code>+</code> to sort descending or ascending. If no sign is specified, the list is sorted descending.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>This field is used for pagination. Enter or map the criteria for the next page with respect to the property specified in the Order by field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td>Enter or map the parameter name that you want to sort this list by. Add <code>-</code> or <code>+</code> to sort descending or ascending. If no sign is specified, the list is sorted descending.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by property]</td> 
   <td>For each property filter you want to add, click <b>Add item</b> and enter the property's key and value. Records that include the specified value for the property are included in the list.</td> 
  </tr> 
 </tbody> 
</table>

### Make a custom API call

This action module makes a custom API call to the Adobe Journey Optimizer API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Enter a path relative to the base URL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds authorization, <code>x-api-key</code>, and <code>x-gw-ims-org-id</code> headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Patch a record

This action module updates a record using PATCH with JSON pointer format

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Select whether you are patching a content template or content fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template/Fragment ID]</td> 
   <td>Enter or map the ID of the template or fragment you want to patch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload data]</td> 
   <td>To add a record to the payload of this patch: <ol><li>Click <b>Add a record</b>.</li><li>Select the operation: Add, Remove, or Replace.</li><li>In the Path field, select whether you want to patch the name or the description.</li><li> In the From field, enter or map a string that contains a JSON pointer value.</li><li>In the Value field, enter the value to be used in the operation.</li></ol></td> 
  </tr> 
 </tbody> 
</table>

### Status for audience-based message

### Trigger an audience-based message

### Trigger a unitary message execution

### Undeploy a configuration

This action module undeploys a capping or throttling configuration. The configuration state is changed back to the state before the deployment (`created` or `updated`).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are undeploying a capping configuration or a throttling configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Enter or map the ID of the configuration you want to undeploy.</td> 
  </tr> 
 </tbody> 
</table>

### Update a configuration

This action module updates the specified capping or throttling configuration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you are updating a capping configuration or a throttling configuration.<ul><li><p><b>Capping</b></p>For fields, see <a href="#capping-fields" class="MCXref xref" >Capping fields</a> in the Create a configuration section of this article.</li><li><p><b>Throttling</b></p>For fields, see <a href="#throttling-fields" class="MCXref xref" >Throttling fields</a> in the Create a configuration section of this article.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

### Update a record

This action module updates a content template or fragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Select whether you are updating a capping configuration or a throttling configuration.<ul><li><p><b>Template</b></p>For fields, see <a href="#template-fields" class="MCXref xref" >Template fields</a> in the Create a record section of this article.</li><li><p><b>Fragment</b></p>For fields, see <a href="#fragment-fields" class="MCXref xref" >Fragment fields</a> in the Create a record section of this article.</li></ul></td> 
  </tr> 
  </tbody> 

### List configurations

This action module lists all capping or throttling configurations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Select whether you want to list capping configurations or a throttling configurations.</td> 
  </tr> 
 </tbody> 
</table>



