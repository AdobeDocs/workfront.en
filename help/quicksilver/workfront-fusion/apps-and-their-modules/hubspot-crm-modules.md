---
title: HubSpot CRM modules
description: HubSpot CRM modules
author: Becky
draft: Probably
feature: Workfront Fusion
---
# HubSpot CRM modules

The Adobe Workfront Fusion HubSpot CRM modules enable you to monitor events, records, contacts, engagements, file and form submissions, or create, retrieve, update and delete records, contacts, engagements, events, or files in your HubSpot CRM account.

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

To use HubSpot CRM modules, you must have a HubSpot CRM account.

## Connect Adobe Workfront Fusion to HubSpot CRM

For instructions about connecting your HubSpot CRM account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

## HubSpot CRM modules and their fields

When you configure Hubspot CRM modules, Workfront Fusion displays the fields listed below. Along with these, additional Hubspot CRM fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM objects](#crm-objects) 
* [Records (Deals, Contacts, and Companies)](#records-deals-contacts-and-companies) 
* [Contacts](#contacts) 
* [Deals](#deals) 
* [Companies](#companies) 
* [Files](#files) 
* [Tickets](#tickets) 
* [Make an API Call](#make-an-api-call)

### CRM objects {#crm-objects}

#### Search for CRM Objects

This search module searches for CRM objects by custom properties or by query. To search for products or line items, use a special connection with a required custom scope.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of items that the module will return in one execution cycle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object Type to Search</td> 
   <td>Select the type of Hubspot CRM&nbsp;object that you want to search for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output properties</td> 
   <td>Select the properties that you want to appear in the module's output. The available fields depend on the object you selected.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter by </td> 
   <td> <p>Select how you want to filter the search</p> 
    <ul> 
     <li> <p><strong>Query</strong> </p> <p>Enter or map the query</p> </li> 
     <li> <p><strong>Properties</strong> </p> <p>Enter the groups or filters for your search.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort by</td> 
   <td> <p>Click if you want to sort the results. If you choose to sort results, the following fields appear. </p> 
    <ul> 
     <li> <p><strong>Property name</strong> </p> <p>Select the property by which you want to sort results</p> </li> 
     <li> <p><strong>Direction</strong> </p> <p>Choose whether you want to sort the results in an ascending or descending direction.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID&nbsp;of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Records (Deals, Contacts, and Companies) {#records-deals-contacts-and-companies}

* [Create a Record (Legacy)](#create-a-record-legacy) 
* [Get a Record](#get-a-record) 
* [Update a Record](#update-a-record) 
* [Delete a Record](#delete-a-record) 
* [Get a Record Property](#get-a-record-property) 
* [Watch Records](#watch-records)

#### Create a Record (Legacy) {#create-a-record-legacy}

This action module creates contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want to create</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Properties</td> 
   <td>Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a Record {#get-a-record}

This action module gets details of a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the record type.</p> 
    <ul> 
     <li>Contact</li> 
     <li>Company </li> 
     <li>Deal</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search Type</td> 
   <td>If you are getting a contact, select whether you want to identify it by ID or by Email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter the ID of the contact, company or deal that you want to retrieve. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email</td> 
   <td>Enter the email address of the contact whose details you want to retrieve. </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Record {#update-a-record}

This action module updates a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of record you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search Type</td> 
   <td> <p>If you are getting a contact, select how you want to identify the record:</p> 
    <ul> 
     <li> <p>ID</p> </li> 
     <li> <p>Email</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter the ID of the contact, company or deal that you want to update. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email</td> 
   <td>Enter the email address of the contact whose details you want to update. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Properties</td> 
   <td>Fill in any properties that you want to set for the record. The available fields depend on the type of record you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Record {#delete-a-record}

This action module deletes a contact, a company, or a deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of record you want to delete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter the ID of the contact, company, or deal you want to delete. </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Record Property {#get-a-record-property}

This action module gets metadata for a specific record property by its (internal) name.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of record that has the property you want to retrieve metadata for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Property Name</td> 
   <td>Select the property that you want to retrieve metadata for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Option ID</td> 
   <td> <p> Some properties have a set of available options that a user can select as the property value. Enter the ID of the option that represents the property value you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Records  {#watch-records}

This trigger module starts a scenario when a contact, company, or deal has been modified or created within the last 30 days. Output is limited to 10,000 records.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of record that has the property you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search</td> 
   <td>Select whether you want to watch recently modified or recently created records.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output Properties</td> 
   <td>Select the properties that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contacts {#contacts}

* [Create/Update a Contact (Legacy)](#create-update-a-contact-legacy) 
* [Create/Update a Group of Contacts](#create-update-a-group-of-contacts) 
* [Add Contacts to a List](#add-contacts-to-a-list) 
* [Remove a Contact from a List](#remove-a-contact-from-a-list) 
* [Merge contacts](#merge-contacts) 
* [Search for Contacts](#search-for-contacts) 
* [List Contacts](#list-contacts) 
* [List Contacts of a Company](#list-contacts-of-a-company)

#### Create/Update a Contact (Legacy) {#create-update-a-contact-legacy}

Creates a contact if it doesn't exist in a portal already, or updates it with the latest property values if it does exist in a portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Properties</td> 
   <td>Fill in any properties that you want to set or update for the contact. </td> 
  </tr> 
 </tbody> 
</table>

#### Create/Update a Group of Contacts {#create-update-a-group-of-contacts}

Creates a group of contacts or updates them if they already exist. Performance is best when batch size is limited to 100 contacts or fewer. Changes made through this endpoint are processed asynchronously, so it can take several minutes for changes to be applied to contact records.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Batch of Contacts to Create/Update </td> 
   <td> <p>Add the batch of contacts.</p> <p>Click <strong>Add item</strong> to add a new contact. In the window that appears, enter or map the following information:</p> 
    <ul> 
     <li> <p><strong>Search Type</strong> </p> <p>Select how you want to identify the contact:</p> 
      <ul> 
       <li> <p>ID</p> <p>Enter the ID of the contact that you want to create or update. </p> </li> 
       <li> <p>Email</p> <p>Enter the email address of the contact that you want to create or update. </p> </li> 
      </ul> </li> 
     <li> <p><strong>Properties</strong> </p> <p>Fill in any properties that you want to set or updatefor the contact.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Add Contacts to a List {#add-contacts-to-a-list}

This module adds contact records that have already been created in the system to a contact list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td>Select the ID of the list to which you want to add the contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">IDs/Emails </td> 
   <td> <p>Select how you want to identify the contacts you want to add to the list:</p> 
    <ul> 
     <li> <p>IDs</p> <p>Add the IDs of the contacts that you want to add to the list.</p> </li> 
     <li> <p>Emails</p> <p>Add the email addresses of the contacts that you want to add to the list.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Remove a Contact from a List {#remove-a-contact-from-a-list}

Removes a contact from a contact list.

>[!NOTE]
>
>You cannot manually remove contacts from a dynamic list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td>Select the ID of the list from which you want to remove the contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contact ID </td> 
   <td>Enter the ID of the contact you want to remove from the list. </td> 
  </tr> 
 </tbody> 
</table>

#### Merge contacts {#merge-contacts}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID 1 </td> 
   <td>Enter the ID of the one of the contacts you want to merge. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID 2 </td> 
   <td>Enter the ID&nbsp;of the other contact that you want to merge.</td> 
  </tr> 
 </tbody> 
</table>

#### Search for Contacts {#search-for-contacts}

Retrieves a list of contacts using the search query.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query</td> 
   <td>Enter the search query.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td>Enter or map the maximum number of contacts Workfront Fusion should return during one scenario execution cycle. </td> 
  </tr> 
 </tbody> 
</table>

#### List Contacts {#list-contacts}

Returns all contacts that have been created in the portal. The output is limited to 5000 contacts. To list previous or next contacts, you can use the advanced parameter to offset the list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>The maximum number of contacts Workfront Fusion should return during one scenario execution cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output properties</td> 
   <td>Select the properties that you want to appear in the module's output. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### List Contacts of a Company {#list-contacts-of-a-company}

Retrieves a list of contacts in the company. The output is limited to 5000 contacts. To list previous or next contacts, you can use the advanced parameter to offset the list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter the ID of the company whose contacts you want to list. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>The maximum number of contacts Workfront Fusion should return during one scenario execution cycle. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### Watch contacts added to a list

This trigger module starts a scenario when a new contact is added to a list. This is available only to users with a paid Marketing account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID</td> 
   <td>Enter or map the ID of the list that contains the contacts you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output Properties</td> 
   <td>Select the properties that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Deals  {#deals}

* [List Deal/Ticket Pipelines](#list-deal-ticket-pipelines) 
* [Get a Deal's CRM Pipeline](#get-a-deal-s-crm-pipeline)

#### List Deal/Ticket Pipelines {#list-deal-ticket-pipelines}

Returns all deal and ticket pipelines for a given portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object Type </td> 
   <td>Select whether you want to list deals or tickets.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a Deal's CRM Pipeline {#get-a-deal-s-crm-pipeline}

Returns a specific deal pipeline..

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pipeline ID </td> 
   <td>Enter or map the ID of the pipeline you want to retrieve details for. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stage ID </td> 
   <td>Enter or map the ID of the stage you want to retrieve details for. </td> 
  </tr> 
 </tbody> 
</table>

### Companies  {#companies}

#### Search for Companies by domain

Retrieves a list of companies based on an exact match to the domain property.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Domain </td> 
   <td>Enter the domain of the companies you want to search for, such as <code>hubspot.com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>The maximum number of companies Workfront Fusion should return during one scenario execution cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output properties</td> 
   <td>Select the properties that you want to appear in the module's output. </td> 
  </tr> 
 </tbody> 
</table>

### Files {#files}

* [Create a Folder](#create-a-folder) 
* [Delete a Folder](#delete-a-folder) 
* [Move a File](#move-a-file)

#### Create a Folder {#create-a-folder}

This module creates a folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder Name </td> 
   <td>Enter or map a name for the new folder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Parent Folder ID </td> 
   <td>Select the ID of the parent folder for the folder you are creating. </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Folder {#delete-a-folder}

Marks a folder as deleted.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter the ID of the folder that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Move a File {#move-a-file}

Moves a file to a different folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File ID </td> 
   <td>Enter or map the ID of the file you want to move. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID </td> 
   <td>Select the ID of the folder where you want to move the file. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name</td> 
   <td>Enter a name for the moved file.</td> 
  </tr> 
 </tbody> 
</table>

### Tickets {#tickets}

#### Delete a Ticket

Deletes an existing ticket by its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter the ID of the ticket that you want to delete. </td> 
  </tr> 
 </tbody> 
</table>

### Make an API Call {#make-an-api-call}

Allows you to perform a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your HubSpot CRM account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to https://api.hubapi.com/. For example, /contacts/v1/lists/all/contacts/all</p> <p>For the list of available endpoints, refer to the <a href="https://legacydocs.hubspot.com/docs/overview">HubSpot API Documentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP method you want to use:</p> <p>GET</p> <p>to retrieve information for an entry.</p> <p>POST</p> <p>to create a new entry.</p> <p>PUT</p> <p>to update/replace an existing entry.</p> <p>PATCH</p> <p>to make a partial entry update.</p> <p>DELETE</p> <p>to delete an entry.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p> Enter the desired request headers. You don't have to add authorization headers; we already did that for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Example:** The following API call returns all contacts in your HubSpot account:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Method**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>Matches of the search can be found in the module's Output under Bundle > Body > contacts.
>
>In our example, 3 contacts were returned:
>
>![](assets/hubspot-api-output.png)

## Create a new application

1. Log in to your HubSpot developer account.
1. Select the Create an App option.
1. Enter the App Name and Save the dialog.
1. Select the scopes you will need for your webhook.

   For example, add contacts scopes for triggering the module when a new contact is created or deleted.

   The contacts scope is all you need to receive contacts, deals, and company event webhooks.

   >[!IMPORTANT]
   >
   >Do not fill in the Redirect URL field.

