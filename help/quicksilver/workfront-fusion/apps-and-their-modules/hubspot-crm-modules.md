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

## HubSpot CRM API information

The HubSpot CRM connector uses the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Base URL</td> 
   <td>https://api.hubapi.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API tag</td> 
   <td>v2.0.14</td> 
  </tr>
 </tbody> 
 </table>

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
* [Engagements](#engagements)
* [Events and Notifications](#events-and-notifications)
* [Files](#files)
* [Tasks](#tasks)
* [Users](#users)
* [Tickets](#tickets)
* [Forms](#forms)
* [Social Media (Broadcast)](#social-media-broadcast)
* [Blog Posts](#blog-posts)
<!--* [Workflows]-->
* [Subscriptions](#subscriptions)
<!--* [Associations](#associations)-->
* [Other](#other)

+++**CRM objects**

### CRM objects

* [Search for CRM objects](#search-for-crm-objects)
* [Watch CRM objects](#watch-crm-objects)

#### [!UICONTROL Search for CRM Objects]

This search module searches for CRM objects by custom properties or by query. To search for products or line items, use a special connection with a required custom scope.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

#### Watch CRM objects

This trigger module starts a scenario when a CRM object is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of items that the module will return in one execution cycle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object type to search]</td> 
   <td> <p>Select the type of object that you want to search for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Select the properties that you want to include in the output for this module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Created/Updated]</td> 
   <td>Select whether you want to watch created (new) or updated (modified) objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by]</td> 
   <td>You can add a filter to ensure that the scenario starts only when certain conditions are met.<ul><li><b>Query</b><p>Enter the query that you want to filter by.</li><li><b>Properties</b><p>For each property that you want to use to filter results, click <b>Add item</b> and enter the property name, operator, and property value.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Records (Deals, Contacts, and Companies)**

### Records (Deals, Contacts, and Companies) 

* [Create a Record](#create-a-record)
* [[!UICONTROL Create a Record (Legacy)]](#create-a-record-legacy)
* [[!UICONTROL Delete a Record]](#delete-a-record)
* [[!UICONTROL Get a Record]](#get-a-record)
* [[!UICONTROL Get a Record Property]](#get-a-record-property)
* [List Records](#list-records)
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

+++

+++**Contacts**

### Contacts

* [[!UICONTROL Add Contacts to a List]](#add-contacts-to-a-list)
* [Create/Update a contact](#createupdate-a-contact)
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

+++

+++**Deals**

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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>Select whether you want to list deals or tickets.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Companies**

### Companies

#### [!UICONTROL Search for Companies by domain]

Retrieves a list of companies based on an exact match to the domain property.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

+++

+++**Engagements**

### Engagements

* [Associate an Engagement with a CRM object](#associate-an-engagement-with-a-crm-object)
* [Create an Engagement](#create-an-engagement)
* [Delete an Engagement](#delete-an-engagement)
* [Watch Engagements](#watch-engagements)

#### Associate an Engagement with a CRM object

This action module associates an engagement with a contact, company, or deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Select the type of CRM record that you want to associate an engagement with. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Engagement ID]</td> 
  <td>Enter or map the ID of the engagement that you want to associate with the object.</td> 
   </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record ID]</td> 
  <td>Enter or map the ID of the record that you want to associate the engagement with.</td> 
   </tr> 
 </tbody> 
</table>

#### Create an Engagement

This action module creates an engagement (such as a note, task, or activity) with a CRM object in HubSpot. Engagements are any interaction with a contact that should be logged in the CRM.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Is Active?]</td> 
   <td>Enable this option if the new engagement will be active when it is created. An engagement must be active to appear in the timeline.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
  <td>Select the type of engagement that you want to create.
  <ul>
  <li><b>Email</b><p></p>Continue to <a href="#email-metadata" class="MCXref xref" >Email metadata</a>.</p></li>
  <li><b>Call</b><p>Continue to <a href="#call-metadata" class="MCXref xref" >Call metadata</a>.</p></li>
  <li><b>Meeting</b><p>Continue to <a href="#meeting-fields" class="MCXref xref" >Meeting fields</a>.</p></li>
  <li><b>Task</b><p>Continue to <a href="#task-fields" class="MCXref xref" >Task fields</a>.</p></li>
  <li><b>Note</b><p>In the Body field, enter the text of the note.</p></li>
  </ul>
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Timestamp</td> 
   <td>Enter or map a timestamp for the engagement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Owner ID</td> 
   <td>Enter or map the Owner ID of the person that the engagement will be assigned to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">UID</td> 
   <td>Enter or map an ID for the engagement, that can be used across object types.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portal ID</td> 
   <td>Enter or map the ID of the portal. This is useful if your organization has multiple portals.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Associated Contacts</td> 
   <td>For each contact that you want to associate this engagement with, click <b>Add item</b> and enter the Contact ID.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Associated Companies</td> 
   <td>For each company that you want to associate this engagement with, click <b>Add item</b> and enter the Company ID.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Associated Deals</td> 
   <td>For each deal that you want to associate this engagement with, click <b>Add item</b> and enter the Deal ID.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Associated Tickets</td> 
   <td>For each ticket that you want to associate this engagement with, click <b>Add item</b> and enter the Ticket ID.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attachments</td> 
   <td>For each attachment that you want to associate this engagement with, click <b>Add item</b> and enter the File ID of the file you want to attach.</td> 
  </tr> 
 </tbody> 
</table>

##### Email metadata

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL From > Email]</p> </td> 
   <td> <p>Enter or map the email address that the email will be sent from.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First Name]</td> 
   <td>Enter or map the first name of the person that the email will be sent from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Last Name]</td> 
  <td>Enter or map the last name of the person that the email will be sent from.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">To</td> 
   <td>For each email address that you want to send the email to, click <b>Add item</b> and enter or map the email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cc</td> 
   <td>For each email address that you want to Cc the email to, click <b>Add item</b> and enter or map the email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bcc</td> 
   <td>For each email address that you want to Bcc the email to, click <b>Add item</b> and enter or map the email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td>Enter or map the text of the email subject</td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML</td> 
   <td>To send an HTML-formatted email, enter or map the body of the email, including HTML tags.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Text</td> 
   <td>To send a text-only email, enter or map the text of the body of the email.</td> 
  </tr> 
 </tbody> 
</table>

##### Call metadata

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL To Number]</p> </td> 
   <td> <p>Enter or map the telephone number that the call will be made to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL From Number]</td> 
   <td>Enter or map the telephone number that the call will be made from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
  <td>Select the status of the call.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the details or notes for the call.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">External ID</td> 
   <td>This field represents the internal ID of a call made in HubSpot. It requires no action.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Duration</td> 
   <td>Enter or map the length of the call in milliseconds</td> 
  </tr> 
  <tr> 
   <td role="rowheader">External Account ID</td> 
   <td>This field represents the internal account ID of a call made in HubSpot. It requires no action.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Recording URL</td> 
   <td>Enter or map the URL of the recording file.</td> 
  </tr> 
 </tbody> 
</table>

##### Meeting fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Title]</p> </td> 
   <td> <p>Enter or map the title or subject of the meeting.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Enter or map the text of the meeting description or details.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Time]</td> 
  <td>Enter or map the start time of the meeting as a UNIX timestamp.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">End time</td> 
   <td>Enter or map the end time of the meeting as a UNIX timestamp.</td> 
  </tr> 
 </tbody> 
</table>

##### Task fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Subject]</p> </td> 
   <td> <p>Enter or map the title or subject of the task.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Enter or map the text of the task description or details.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status</td> 
   <td>Select the status of the task.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL For Object Type]</td> 
  <td>Enter either <code>CONTACT</code> or <code>COMPANY</code>.
  </td> 
   </tr> 
 </tbody> 
</table>

#### Delete an Engagement

This action module deletes an engagement by its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Enter or map the ID of the engagement that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Engagements

This trigger module starts a scenario when a new engagement is created in a portal. This module only returns records created in the last 30 days, or the 10,000 most recently created records.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>The maximum number of companies [!DNL Workfront Fusion] should return during one scenario execution cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>Enter or map the earliest date for which you want to watch events. Use the format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Events and Notifications**

### Events and Notifications

* [Create / Update a Timeline Event](#create--update-a-timeline-event)
* [List Timeline Event Types](#list-timeline-event-types)
* [Watch Calendar Events](#watch-calendar-events)
* [Watch Notifications](#watch-notifications)

#### Create / Update a Timeline Event

This action module creates or updates a timeline event. This module can be used only with a developer connection that includes your user identifier, your HubSpot API key, Client ID, and Client Secret. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application ID]</td> 
   <td>Enter or map the ID of the application that this event belongs to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td>Enter or map an ID for this event. Event IDs are not generated by the system.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Type ID]</td> 
   <td>Enter or map the ID of this event's event type.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Enter or map the email address of the contact that you're creating the event for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object ID]</td> 
   <td>Enter or map the ID of the contact that you're creating the event for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp]</td> 
   <td>Enter or map the timestamp for this event.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom data]</td> 
   <td>For each item of custom data that you want to add to this event, click <b>Add item</b> and enter the item's name and value.</td> 
  </tr> 
 </tbody> 
</table>

#### List Timeline Event Types

This search module returns a list of all timeline events for a specific application. This module can be used only with a developer connection that includes your user identifier, your HubSpot API key, Client ID, and Client Secret. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application ID]</td> 
   <td>Enter or map the ID of the application that this events belong to. </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Calendar Events

This trigger module starts a scenario when a new event is added to a calendar. It includes up to 500 tasks in the interval between the start and end date. This module can be used only with a developer connection that includes your user identifier, your HubSpot API key, Client ID, and Client Secret. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Events Type]</td> 
   <td>Select whether you want to watch social events, content events, or all events.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>Enter or map the start date.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>Enter or map the end date.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Notifications

This trigger module starts a scenario when a new notification about changes is sent.  It includes up to 500 tasks in the interval between the start and end date. This module can be used only with a developer connection that includes your user identifier, your HubSpot API key, Client ID, and Client Secret. You can have only one webhook URL per developer application in HubSpot.

To create a webhook for this module, click **Add** next to the webhook field and fill out the following fields:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application ID]</td> 
   <td>Enter the application ID that you want to use for this webhook. You can find the ID in your HubSpot developer portal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscriptions]</td> 
   <td> <p>For each type of notification that you want to watch, click <b>Add item</b> and select the subscription type.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Force to Remove Old Subscriptions]</td> 
   <td>Enable this option to detach or delete old subscriptions attached to this webhook.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Files**

### Files

* [[!UICONTROL Create a Folder]](#create-a-folder)
* [Delete a File](#delete-a-file)
* [[!UICONTROL Delete a Folder]](#delete-a-folder)
* [List Files](#list-files)
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

+++

+++**Tasks**

### Tasks

* [Create a Calendar Task](#create-a-calendar-task)
* [Delete a Calendar Task](#create-a-calendar-task)
* [Watch Task Events](#watch-task-events)

#### Create a Calendar task

This action module creates a new task for a calendar. The connection used in this module must use the credentials of a user with a paid Marketing account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the new calendar task.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the new calendar task.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Owner ID]</td> 
   <td>Enter or map the owner ID of the user that is assigned to this task.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Date]</td> 
   <td>Enter or map the date for this task.<p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Select the type of event.<ul><li><b>Blog Post</b><p>Enter the content group ID. This is the ID of the blog page.</p></li><li><b>Email</b><p>Enter or map the path to the email template you want to use.</li><li><b>Landing Page</b><p>Enter or map the path to the landing page template you want to use.</li><li><b>Custom</b></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Enter whether the event is in a "To do" or "Done" state.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign GUID]</td> 
   <td>Enter or map the internal HubSpot ID of the campaign that this event is part of.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Calendar Task

This action module deletes a calendar task. The connection used in this module must use the credentials of a user with a paid Marketing account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the task that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Task Events

This trigger module starts a scenario when there is a new task event in a calendar. The connection used in this module must use the credentials of a user with a paid Marketing account. The module returns up to 500 events.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

+++

+++**Users**

### Users

* [Get an Owner](#get-an-owner)
* [List Owners](#list-owners)

#### Get an Owner

This action module returns details of an owner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Owner ID]</td> 
   <td> <p>Enter or map the ID of the owner that you want to return details for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Owners

This search module returns a list of all of the owners in a HubSpot account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tickets**

### Tickets

<!--* [Create a Ticket]-->
* [Delete a Ticket](#delete-a-ticket)
<!--* [Create a Ticket]-->
<!--* [Create a Ticket]-->
<!--* [Create a Ticket]-->
<!--* [Create a Ticket]-->

<!-- Create a Ticket Need to find a working connection-->

#### [!UICONTROL Delete a Ticket]

Deletes an existing ticket by its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter the ID of the ticket that you want to delete. </td> 
  </tr> 
 </tbody> 
</table>

<!-- Get a Ticket  Need to find a working connection-->

<!-- List Tickets  Need to find a working connection-->

<!-- Update a Ticket Need to find a working connection--->

<!-- Watch Tickets Need to find a working connection-->

+++

+++**Forms**

### Forms

* [Get a File Uploaded via Form](#get-a-file-uploaded-via-form)
* [List Forms](#list-forms)
<!--* [Submit Data to a Form]-->
<!--* [Watch Submissions for a Form]-->

#### Get a File Uploaded via Form

This action module returns a file that was uploaded through a form.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td>Enter or map the URL of the file you want to retrieve. This can be found in the form metadata.</td> 
  </tr> 
 </tbody> 
</table>

#### List Forms

This action module returns all forms that have been created in the account associated with the connection used for this module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of forms that the module will return in one execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Submit Data to a Form Need to find a working connection-->



<!--#### Watch Submissions for a Form--Need to find a working connection>-->

+++

+++**Social Media (Broadcast)**

### Social Media (Broadcast)

* [Cancel a Broadcast Message](#cancel-a-broadcast-message)
* [Create a Broadcast Message](#create-a-broadcast-message)
* [Watch Broadcast Messages](#watch-broadcast-messages)

#### Cancel a Broadcast Message

This action module cancels a scheduled broadcast, such as a tweet or a Facebook post.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Broadcast ID]</td> 
   <td>Enter or map the ID of the broadcast that you want to cancel.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a Broadcast Message

This action module creates and immediately publishes a message on the specified social media channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel ID]</td> 
   <td>Enter or map the ID of the channel that you want to use for this broadcast.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter or map a title for this broadcast.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Enter or map the text of the broadcast.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Photo URL]</td> 
   <td>Enter or map the URL of a photo that you want to include in the broadcast.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thumbnail URL]</td> 
   <td>Enter or map the URL of a thumbnail that you want to use for this broadcast.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trigger at]</td> 
   <td>Enter or map the date and time that you want the broadcast to be sent. If this is left blank, the broadcast is sent immediately.<p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Watch Broadcast Messages

This trigger module starts a scenario when a message is posted from HubSpot to the specified social media channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of items that the module will return in one execution cycle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by Status]</td> 
   <td>To start the scenario only when the message is in a specific status, select the status.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by Channel]</td> 
   <td>To start the scenario only when the message is on a specific channel, select the channel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Broadcast ID]</td> 
   <td>To start the scenario only when the message is on or after a specific date, enter or map the date in the format <code>MM/DD/YYYY</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Blog Posts**

### Blog posts 

<!--* [Create a Blog Post]-->
* [Delete a Blog Post](#delete-a-blog-post)
<!--* [List Blog Posts]-->
* [Publish/Unpublish a Blog Post](#publish--unpublish-a-blog-post)
<!--* [Watch Blog Posts]-->

<!--
#### Create a Blog Post May need connection
-->


#### Delete a Blog Post

This action module deletes a single blog post.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the blog post that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### List Blog Posts May need connection

This search module retrieves posts from a HubSpot blog.-->

#### Publish / Unpublish a Blog Post

This action module schedules or cancels publishing of a blog post.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the blog post that you want to schedule or cancel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td>Select whether you want to schedule the blog post, or cancel a previously scheduled blog post.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Watch Blog PostsMay need connection-->

+++

<!--+++**Workflows**>

<!--### Workflows May need connection

#### Add a Contact to a Workflow


#### Remove a Contact from a Workflow

-->

<!--+++-->

+++**Subscriptions**

### Subscriptions

* [Update Email Subscription](#update-email-subscription)
* [Watch Subscriptions Timeline for a Portal](#watch-subscriptions-timeline-for-a-portal)

#### Update Email Subscription

This action module updates an email subscription in HubSpot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Enter or map the email address of the subscription you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Statuses]</td> 
   <td>For each status that you want to update the subscription for, click <b>Add item</b> and enter the status's ID, and whether the email address will be subscribed to that status.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal Subscription Legal Status]</td> 
   <td>To record the legal basis for this subscription for GDPR, select the legal status of this subscription.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal Subscription Legal Basis Explanation]</td> 
   <td>To add a note regarding the legal basis for this subscription for GDPR, enter or map the text of the note.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Subscriptions Timeline for a Portal

This trigger module starts a scenario when a new email timeline subscription is added to the portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of items that the module will return in one execution cycle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Timestamp]</td> 
   <td>To return results from on or after a specific date, enter the date in the format <code>MM/DD/YYYY.</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Timestamp]</td> 
   <td>To return results from on or before a specific date, enter the date in the format <code>MM/DD/YYYY.</code></td> 
  </tr> 
 </tbody> 
</table>

+++

<!--+++**Associations**-->

<!--### Associations-->

<!--#### Associate CRM Objects  May need connection

This action module associates two CRM objects.-->

<!--#### Associate Multiple CRM Objects  May need connection-->



<!--#### Delete an Association May need connection-->



<!--#### Delete Multiple Associations between CRM Objects May need connection-->



<!--#### List Associations for a CRM Object May need connection-->

<!--+++-->

+++**Other**

### Other

#### [!UICONTROL Make an API Call]

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
   <td> <p>For instructions about connecting your [!DNL HubSpot CRM] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
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

+++

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
