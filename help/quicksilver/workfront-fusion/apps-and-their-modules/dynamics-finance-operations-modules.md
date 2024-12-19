---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 Finance and Operations modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Microsoft Dynamics 365 Finance and Operations, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 19b00ee8-dc05-4cde-9a76-d857090fa543
---
# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

>[!IMPORTANT]
>
>The Adobe Workfront Fusion documentation has moved to a new location. 
>
>The information in this article can now be found in the article:
>
>* [Microsoft Dynamics 365 Finance and Operations modules](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/dynamics-finance-operations-modules.html)
>
>Please update any bookmarks.
>
>This article is no longer being updated, and will be removed in the near future.

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Microsoft Dynamics 365], as well as connect it to multiple third-party applications and services.

>[!NOTE]
>
>The [!DNL Microsoft Dynamics 365 Finance and Operations] connector does not support [!DNL Dynamics 365].
>
>For Microsoft Dynamics 365 modules, see [[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Create a connection

To create a connection for your Microsoft Dynamics 365 Finance and Operations modules:

1. In any Microsoft Dynamics 365 Finance and Operations module, click **[!UICONTROL Add]** next to the Connection box.
    
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
          <p>Select whether you are creating a standard Dynamics Finance and Operations connection, or a connection using an authorization code.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your Dynamics Finance and Operations [!UICONTROL Client ID].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your Dynamics Finance and Operations [!UICONTROL Client Secret]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tenant ID]</td>
        <td>Enter your Dynamics Finance and Operations  Tenant ID.</td>
        </tr>
        <tr>
        <td role="rowheader">Resource</td>
        <td>Enter the URL of your Dynamics Finance and Operations account (without https://)</td>
        </tr>
      </tbody>
    </table>
    
1. Click **[!UICONTROL Continue]** to save the connection and return to the module.
    


## Microsoft Dynamics 365 Finance and Operations modules and their fields

>[!IMPORTANT]
>
>The data entities available through the Dynamics 365 F&O API can vary by instance. If you are not sure what entities are available through the API, it's useful to look through the entities in your instance using the "data" endpoint. The "data" endpoint in Dynamics 365 Finance and Operations is the root URL for accessing OData services. This endpoint allows you to interact with various data entities exposed by the system using standard OData protocols.
>
>You can retrieve these entities using the custom API call module.
>
><!--For more information --> 



### Create entity item

This action module creates a new entity item in Microsoft Dynamics 365 Finance and Operations.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Enter or map the Dynamics Finance and Operations entity type that you want to create.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Enter or map a JSON body that contains the data that you want to include in the new entity item.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Delete entity item

This action module deletes an entity item from Dynamics Finance and Operations. The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Enter or map the Dynamics Finance and Operations entity type that you want to delete.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Primary key fields]</td>
     <td> The Primary key fields identify the item. For each primary key field that you want to provide, click <b>Add item</b> and enter or map the unique key and value that identify that item. </td> 
  </tr> 
 </tbody> 
</table>

### Make a custom API call

This action module makes a custom call to the Dynamics Finance and Operations API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to your Dynamics Finance and Operations URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object. This determines the content type of the request.</p> <p>For example,<code> {"Content-type":"application/json"}</code></p> <p>Note: If you're getting errors and it's difficult to determine their origin, consider modifying headers based on the [!DNL Workfront] documentation. If your Custom API Call returns a 422 HTTP Request Error, try using a <code>"Content-Type":"text/plain"</code> header.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query string]</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> <p>Tip: We recommend that you send information through the JSON body rather than as query parameters.</p> </td> 
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



### Read entity item

This action module returns data from an entity item. The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Enter or map the Dynamics Finance and Operations entity type that you want to read.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Primary key fields]</td>
     <td> The Primary key fields identify the item. For each primary key field that you want to provide, click <b>Add item</b> and enter or map the unique key and value that identify that item. </td> 
  </tr> 
 </tbody> 
</table>

### Update entity item

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Enter or map the Dynamics Finance and Operations entity type that you want to update.</td> 
  </tr>  
  <tr> 
    <td>[!UICONTROL Primary key fields]</td>
     <td> The Primary key fields identify the item. For each primary key field that you want to provide, click <b>Add item</b> and enter or map the unique key and value that identify that item. </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Enter or map a JSON body that contains the data that you want to include in the new entity item.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Search

This search module returns results based on criteria you specify.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entity]</td> 
   <td>Enter or map the Dynamics Finance and Operations entity type that you want to search.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort by]</td> 
   <td> <p>Enter or map the field that you want to sort the results by.</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
