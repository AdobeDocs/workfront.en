---
title: HubSpot CRM modules
description: The [!DNL Adobe Workfront Fusion] HubSpot CRM modules enable you to monitor events, records, contacts, engagements, file and form submissions, or create, retrieve, update and delete records, contacts, engagements, events, or files in your [!DNL HubSpot CRM] account.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
---
# [!DNL HubSpot CRM] modules

The [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] modules enable you to monitor events, records, contacts, engagements, file and form submissions, or create, retrieve, update and delete records, contacts, engagements, events, or files in your [!DNL HubSpot CRM] account.

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

## Prerequisites

To use [!DNL HubSpot CRM] modules, you must have a [!DNL HubSpot CRM] account.

## Connect [!DNL Adobe Workfront Fusion] to [!DNL HubSpot CRM]

For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see [Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>When configuring a connection, select the **HubSpot CRM** connection type. The HubSpot CRM (Deprecated) type supports existing connections, but we do not recommend using it to create new connections.

## [!DNL HubSpot CRM] modules and their fields

When you configure [!DNL Hubspot CRM] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Hubspot CRM] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM objects](#crm-objects)
* [Records (Deals, Contacts, and Companies)](#records-deals-contacts-and-companies)
* [Contacts](#contacts)
* [Deals](#deals)
* [Companies](#companies)
* [Files](#files)
* [Tickets](#tickets)
* [Make an API Call](#make-an-api-call)

### CRM objects

#### [!UICONTROL Search for CRM Objects]

This search module searches for CRM objects by custom properties or by query. To search for products or line items, use a special connection with a required custom scope.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of items that the module will return in one execution cycle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type to Search]</td> 
   <td>Select the type of Hubspot CRM object that you want to search for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Select the properties that you want to appear in the module's output. The available fields depend on the object you selected.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by] </td> 
   <td> <p>Select how you want to filter the search</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Enter or map the query</p> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Enter the groups or filters for your search.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Click if you want to sort the results. If you choose to sort results, the following fields appear. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Property name]</strong> </p> <p>Select the property by which you want to sort results</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Choose whether you want to sort the results in an ascending or descending direction.</p> </li> 
    </ul> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
 </tbody> 
</table>

<!-- #### Watch CRM objects NEED CONNECTION EXPANDED-->

### Records (Deals, Contacts, and Companies) 

* [[!UICONTROL Create a Record (Legacy)]](#create-a-record-legacy)
* [[!UICONTROL Delete a Record]](#delete-a-record)
* [[!UICONTROL Get a Record]](#get-a-record)
* [[!UICONTROL Get a Record Property]](#get-a-record-property)
* [[!UICONTROL Update a Record]](#update-a-record)
* [[!UICONTROL Watch Records]](#watch-records)

#### Create a record

This action module creates a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want to create.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property groups]</td> 
   <td>For each property that you want to add when creating the record, select the group where the property is found. The property group will open, and you can then fill in the value for the properties. The available property groups and properties depend on the type of record you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Record (Legacy)]

This action module creates contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record you want to create.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Record]

This action module deletes a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Select the type of record you want to delete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter the ID of the contact, company, or deal you want to delete. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Record]

This action module gets details of a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the record type.</p> 
    <ul> 
     <li>[!UICONTROL Contact]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td>If you are getting a contact, select whether you want to identify it by ID or by Email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter the ID of the contact, company or deal that you want to retrieve. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Enter the email address of the contact whose details you want to retrieve. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Record Property]

This action module gets metadata for a specific record property by its (internal) name.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Select the type of record that has the property you want to retrieve metadata for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property Name]</td> 
   <td>Select the property that you want to retrieve metadata for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> Some properties have a set of available options that a user can select as the property value. Enter the ID of the option that represents the property value you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Records

This search module returns a list of contacts, companies or deals. Output is limited to 5000 contacts, 12,500 companies, or 12,500 deals.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Select the type of record you want to return.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Select the properties that you want to include in the output for this module.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 

 </tbody> 
</table>

#### [!UICONTROL Update a Record]

This action module updates a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Select the type of record you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>If you are getting a contact, select how you want to identify the record:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter the ID of the contact, company or deal that you want to update. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Enter the email address of the contact whose details you want to update. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Records]

This trigger module starts a scenario when a contact, company, or deal has been modified or created within the last 30 days. Output is limited to 10,000 records.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Select the type of record that has the property you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Select whether you want to watch recently modified or recently created records.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Select the properties that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contacts

* [[!UICONTROL Add Contacts to a List]](#add-contacts-to-a-list)
* [[!UICONTROL Create/Update a Contact (Legacy)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Create/Update a Group of Contacts]](#createupdate-a-group-of-contacts)
* [[!UICONTROL List Contacts]](#list-contacts)
* [[!UICONTROL List Contacts of a Company]](#list-contacts-of-a-company)
* [[!UICONTROL Merge contacts]](#merge-contacts)
* [[!UICONTROL Remove a Contact from a List]](#remove-a-contact-from-a-list)
* [[!UICONTROL Search for Contacts]](#search-for-contacts)
* [Watch Contacts Added to a List](#watch-contacts-added-to-a-list)

#### [!UICONTROL Add Contacts to a List]

This module adds contact records that have already been created in the system to a contact list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Select the ID of the list to which you want to add the contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/Emails] </td> 
   <td> <p>Select how you want to identify the contacts you want to add to the list:</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Add the IDs of the contacts that you want to add to the list.</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>Add the email addresses of the contacts that you want to add to the list.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Create/Update a Contact

This action module creates a contact if it doesn't exist in a portal. If the contact does exist in the portal, this module updates it with the provided values.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property groups]</td> 
   <td>For each property that you want to add when creating the contact, select the group where the property is found. The property group will open, and you can then fill in the values for the properties.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Update a Contact (Legacy)]

Creates a contact if it doesn't exist in a portal already, or updates it with the latest property values if it does exist in a portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Fill in any properties that you want to set or update for the contact. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Update a Group of Contacts] 

Creates a group of contacts or updates them if they already exist. Performance is best when batch size is limited to 100 contacts or fewer. Changes made through this endpoint are processed asynchronously, so it can take several minutes for changes to be applied to contact records.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch of Contacts to Create/Update] </td> 
   <td> <p>Add the batch of contacts.</p> <p>Click <strong>[!UICONTROL Add item]</strong> to add a new contact. In the window that appears, enter or map the following information:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>Select how you want to identify the contact:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Enter the ID of the contact that you want to create or update. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Enter the email address of the contact that you want to create or update. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Fill in any properties that you want to set or updatefor the contact.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Contacts]

Returns all contacts that have been created in the portal. The output is limited to 5000 contacts. To list previous or next contacts, you can use the [!UICONTROL advanced] parameter to offset the list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>The maximum number of contacts [!DNL Workfront Fusion] should return during one scenario execution cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Select the properties that you want to appear in the module's output. </td> 
  </tr> 
   <tr> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL List Contacts of a Company]

Retrieves a list of contacts in the company. The output is limited to 5000 contacts. To list previous or next contacts, you can use the [!UICONTROL advanced] parameter to offset the list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter the ID of the company whose contacts you want to list. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>The maximum number of contacts [!DNL Workfront Fusion] should return during one scenario execution cycle. </td> 
  </tr> 
   <tr> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL Merge contacts]

This action module merges contacts

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Enter the ID of the one of the contacts you want to merge. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Enter the ID of the other contact that you want to merge.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove a Contact from a List]

Removes a contact from a contact list.

>[!NOTE]
>
>You cannot manually remove contacts from a dynamic list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Select the ID of the list from which you want to remove the contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID] </td> 
   <td>Enter the ID of the contact you want to remove from the list. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search for Contacts]

Retrieves a list of contacts using the search query.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Enter the search query.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Enter or map the maximum number of contacts [!DNL Workfront Fusion] should return during one scenario execution cycle. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch contacts added to a list]

This trigger module starts a scenario when a new contact is added to a list. This is available only to users with a paid Marketing account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Enter or map the ID of the list that contains the contacts you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Select the properties that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Deals

* [[!UICONTROL Get a Deal's CRM Pipeline]](#get-a-deals-crm-pipeline)
* [[!UICONTROL List Deal/Ticket Pipelines]](#list-dealticket-pipelines)

#### [!UICONTROL Get a Deal's CRM Pipeline]

Returns a specific deal pipeline..

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pipeline ID] </td> 
   <td>Enter or map the ID of the pipeline you want to retrieve details for. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>Enter or map the ID of the stage you want to retrieve details for. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Deal/Ticket Pipelines]

Returns all deal and ticket pipelines for a given portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>Select whether you want to list deals or tickets.</td> 
  </tr> 
 </tbody> 
</table>

### Companies

#### [!UICONTROL Search for Companies by domain]

Retrieves a list of companies based on an exact match to the domain property.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Enter the domain of the companies you want to search for, such as <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>The maximum number of companies [!DNL Workfront Fusion] should return during one scenario execution cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Select the properties that you want to appear in the module's output. </td> 
  </tr> 
 </tbody> 
</table>

### Files

* [[!UICONTROL Create a Folder]](#create-a-folder)
* [Delete a file](#delete-a-file)
* [List files](#list-files)
* [[!UICONTROL Delete a Folder]](#delete-a-folder)
* [[!UICONTROL Move a File]](#move-a-file)
* [Upload a file](#upload-a-file)
* [Watch files](#watch-files)

#### [!UICONTROL Create a Folder]

This module creates a folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder Name] </td> 
   <td>Enter or map a name for the new folder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>Select the ID of the parent folder for the folder you are creating. </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a File

This action module permanently deletes a file and all related data and thumbnails from the file manager.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Enter or map the ID of the file that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Folder]

Marks a folder as deleted.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the folder that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### List Files 

This search module returns a list of files stored in the file manager.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Enter or map the ID of the folder that contains the files you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>To include only files that contain specific characters in the filename, enter or map the characters that you want the filename to include.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File]

Moves a file to a different folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>Enter or map the ID of the file you want to move. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>Select the ID of the folder where you want to move the file. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter a name for the moved file.</td> 
  </tr> 
 </tbody> 
</table>

#### Upload a File 

This action module uploads a file to the file manager.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Access type] </td> 
   <td>Select whether you want the file to be private, public but not indexable, or public and indexable. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>Select the ID of the folder where you want to upload the file. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Enable this option to overwrite the file if it already exists in the folder.</td> 
  </tr> 
 </tbody> 
</table>

### Watch Files

This trigger module starts a scenario when a new file is saved to the file manager.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Enter or map the ID of the folder that contains the files you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>To include only files that contain specific characters in the filename, enter or map the characters that you want the filename to include.</td> 
  </tr> 
 </tbody> 
</table>

### Tasks

* [Create a Calendar Task]
* [Delete a Calendar Task]
* [Watch Task Events]

#### Create a Calendar task

This action module creates a new task for a calendar. The connection used in this module must use the credentials of a user with a paid Marketing account.



#### Delete a Calendar Task

This action module deletes a calendar task. The connection used in this module must use the credentials of a user with a paid Marketing account.




#### Watch Task Events

This trigger module starts a scenario when there is a new task event in a calendar. The connection used in this module must use the credentials of a user with a paid Marketing account. The module returns up to 500 events.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>Enter or map the earliest date for which you want to watch events. Use the format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>Enter or map the latest  date for which you want to watch events. Use the format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
 </tbody> 
</table>

























<!-- Users (All)-->

### Tickets

<!-- Create a Ticket -->

#### [!UICONTROL Delete a Ticket]

Deletes an existing ticket by its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter the ID of the ticket that you want to delete. </td> 
  </tr> 
 </tbody> 
</table>

<!-- Get a Ticket -->

<!-- List Tickets -->

<!-- Update a Ticket -->

<!-- Watch Tickets -->

<!-- Forms (All)-->

<!-- Social Media (All)-->

<!-- Blog posts (All)-->

<!-- Workflows (All)-->

<!-- Subscriptions (All)-->

<!-- Associations (All)-->

### [!UICONTROL Make an API Call]

Allows you to perform a custom API call.

>[!NOTE]
>
>The following endpoints were deprecated in the HubSpot API on August 31, 2023, and can no longer be used in Fusion modules.
>
>* List content events
>* List social events
>* List calendar task events
>* List all calendar events
>* Create calendar task
>* Get calendar task by ID
>* Update calendar task
>* Delete a calendar task

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Enter a path relative to https://api.hubapi.com/. For example, /contacts/v1/lists/all/contacts/all</p> <p>For the list of available endpoints, refer to the <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API Documentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Select the HTTP method you want to use:</p> <p>[!UICONTROL GET]</p> <p>to retrieve information for an entry.</p> <p>[!UICONTROL POST]</p> <p>to create a new entry.</p> <p>[!UICONTROL PUT]</p> <p>to update/replace an existing entry.</p> <p>[!UICONTROL PATCH]</p> <p>to make a partial entry update.</p> <p>[!UICONTROL DELETE]</p> <p>to delete an entry.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Enter the desired request headers. You don't have to add authorization headers; we already did that for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Example:** The following API call returns all contacts in your [!DNL HubSpot] account:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Method**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>Matches of the search can be found in the module's Output under [!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL contacts].
>
>In our example, 3 contacts were returned:
>
>![](assets/hubspot-api-output.png)

## Create a new application

1. Log in to your [!DNL HubSpot] developer account.
1. Select the **[!UICONTROL Create an App]** option.
1. Enter the App Name and [!UICONTROL Save] the dialog.
1. Select the scopes you will need for your webhook.

   For example, add contacts scopes for triggering the module when a new contact is created or deleted.

   The [!UICONTROL contacts scope] is all you need to receive contacts, deals, and company event webhooks.

   >[!IMPORTANT]
   >
   >Do not fill in the [!UICONTROL Redirect URL] field.
