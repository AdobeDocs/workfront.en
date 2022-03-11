---
filename: active-campaign-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: ActiveCampaign modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
---

# ActiveCampaign modules

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
In a Adobe Workfront Fusion scenario, you can connect your ActiveCampaign account to multiple third-party applications and services. You can create, update, list, and delete automations, campaigns, calendar feeds, contacts, deals, messages, notes, organizations, tags, and tasks in your ActiveCampaign account.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md). For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Connect Active Campaign to Workfront Fusion

1. Log in to your ActiveCampaign account.
1. From the left menu, click `Settings` > `Developer`.

1. Copy the API `Key` to the clipboard.
1. Go to Workfront Fusion, add an ActiveCampaign module to a scenario, and open the `Create a Connection` box,

   XsCCPEaX9L.gif

   If you need instructions, see [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

1. In the API Key field, enter the API Key copied in step 3.
1. In the Account name field, enter the account name in your ActiveCampaign URL.

   For example, if your URL is

   ```
   live1.activehosted.com
   ```

   then the account name is 

   ```
   live1
   ```

   .

1. Click `Continue`.

## ActiveCampaign Contact modules

* [Create a Contact](#create) 
* [Create/Update a Contact](#create/u) 
* [Delete a Contact](#delete) 
* [Get a Contact](#get) 
* [Create/Update a Contact's Custom Field Value](#create/u2) 
* [Update Contact's List Status](#update) 
* [Add a Tag to a Contact](#add) 
* [Remove a Tag from a Contact](#remove) 
* [List Contacts](#list) 
* [Get Info About Logged-in User](#get2) 
* [Watch Contacts](#watch)

### Create a Contact

This action module creates a new contact.

You specify the person's contact information.

The module returns the ID of the  contact and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">Email </span> </td> 
   <td> <p>Enter the email address of the contact.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">First Name</span> </td> 
   <td> <p> Enter the first name of the contact.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">Last Name</span> </td> 
   <td> <p> Enter the last name of the contact.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">Phone </span> </td> 
   <td> <p>Enter the phone number of the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Create/Update a Contact

This action module creates a new contact or updates an existing contact.

You specify the contact information.

The module returns the ID of the  contact and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Email </span> </td> 
   <td> <p>Enter the email address of the contact.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">First Name</span> </td> 
   <td> <p> Enter the first name of the contact.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Last Name</span> </td> 
   <td> <p> Enter the last name of the contact.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Phone </span> </td> 
   <td> <p>Enter the phone number of the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete a Contact

This action module deletes an existing contact.

You specify the ID of the contact.

The module returns the ID of the  contact and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">ID </span> </td> 
   <td> <p>Enter or map the unique ActiveCampaign ID of the contact that you want the module to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Get a Contact

This action module retrieves a contact.

You specify the ID of the contact.

The module returns the ID of the contact and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">ID </span> </td> 
   <td> <p>Select the type of [Fusion app] record from which you want the module to retrieve details.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Create/Update a Contact's Custom Field Value

This action module creates or updates a custom field value for the given contact.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Contact ID</span> </td> 
   <td> <p> Select the Contact ID whose Custom Field value you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Field ID</span> </td> 
   <td> <p><![CDATA[	]]>Enter the unique [Fusion app] ID of the record that you want the module to update.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Field Value</span> </td> 
   <td> <p> Enter the new field value to update.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Contact's field ID</span> </td> 
   <td> <p> Enter the ID of the contact field to edit.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Update Contact's List Status

This action module updates the list status for a contact.

You specify the contact ID, list ID, and status.

The module returns the ID of the  status and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Contact ID</span> </td> 
   <td> <p> Select the Contact ID whose list status you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">List ID</span> </td> 
   <td> <p> Select the List ID of the contacts you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Status</span> </p> </td> 
   <td> <p>Select the status to update:</p> 
    <ul> 
     <li>Active</li> 
     <li>Unsubscribed</li> 
     <li>Bounced</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Add a Tag to a Contact

This action module adds a tag to a contact.

You specify the IDs of the contact and of the tag.

The module returns the ID of the  tag and contact and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Contact ID</span> </td> 
   <td> <p> Enter the Contact ID to which you want to add the tag.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Tag ID</span> </td> 
   <td> <p> Enter the Tag ID you want to add to the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Remove a Tag from a Contact

This action module removes a tag from a contact.

You specify the ID of the contact.

The module returns the ID of the  contact tag and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Contact's Tag ID</span><![CDATA[	]]></td> 
   <td> <p>Enter the Tag ID to remove from the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

### List Contacts

This action module retrieves a list of contacts.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Limit </span> </td> 
   <td> <p>The maximum number of contacts should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Order by</span> </p> </td> 
   <td> <p>Select the order in which you want to list the contacts:</p> 
    <ul> 
     <li>Creation date</li> 
     <li>Email</li> 
     <li>Name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">ASC/DESC</span> </td> 
   <td> <p> Select the order to list the contacts:</p> 
    <ul> 
     <li>ASC - Ascending order</li> 
     <li>DESC - Descending order</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Email </span> </td> 
   <td> <p>Enter the email address of the contacts you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Email-like pattern</span> </td> 
   <td> <p> Enter the email pattern to list the contacts that contain the given value in the email address.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Search pattern</span> </td> 
   <td> <p> Enter the search pattern to list contacts that match the given value in the contact names, organization, phone or email.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Organization ID</span> </td> 
   <td> <p> Select the Organization ID whose contacts you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">List ID</span> </td> 
   <td> <p> Select the List ID of the contacts you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Segment ID</span> </td> 
   <td> <p> Select the Segment ID whose contacts you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Status</span><![CDATA[	]]></td> 
   <td> <p>Select the status of the contacts you want to list:</p> 
    <ul> 
     <li>Any</li> 
     <li>Unconfirmed</li> 
     <li>Active</li> 
     <li>Unsubscribed</li> 
     <li>Bounced</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Tag ID</span> </td> 
   <td> <p> Select the Tag ID for the contact.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Form ID</span> </td> 
   <td> <p> Select the Form ID for the contact.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Since DateTime</span> </td> 
   <td> <p> Select the date from which you want to list the contacts.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Until DateTime</span> </td> 
   <td> <p> Select the date until which you want to list the contacts.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Get Info About Logged-in User

This action module gets information about the logged-in users.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Contacts

This trigger module executes a scenario when a new contact is created. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Limit </span> </td> 
   <td> <p>The maximum number of contacts should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Email </span> </td> 
   <td> <p>Enter the email address of the contacts you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Email-like Pattern</span> </td> 
   <td> <p> Enter the email pattern to list the contacts that contain the given value in the email address.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Search Pattern</span> </td> 
   <td> <p> Enter the search pattern to list contacts that match the given value in the contact names, organization, phone or email.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Organization ID</span> </td> 
   <td> <p> Select the Organization ID whose contacts you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">List ID</span> </td> 
   <td> <p> Select the List ID of the contacts you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Segment ID</span> </td> 
   <td> <p> Select the Segment ID whose contacts you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Status </span> </td> 
   <td> <p>Select the status of the contacts you want to watch:</p> 
    <ul> 
     <li>Any</li> 
     <li>Unconfirmed</li> 
     <li>Active</li> 
     <li>Unsubscribed</li> 
     <li>Bounced</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Tag ID</span> </td> 
   <td> <p> Select the Tag ID whose contacts you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Form ID</span> </td> 
   <td> <p> Select the Form ID for the contact you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Since DateTime</span> </td> 
   <td> <p> Select the date from which you want to watch the contacts.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Until DateTime</span> </td> 
   <td> <p> Select the date until which you want to watch the contacts.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ActiveCampaign Deal modules

* [Create a Deal](#create3) 
* [Update a Deal](#update3) 
* [Get a Deal](#get4) 
* [Delete a Deal](#delete2) 
* [Move Details to Another Deal Stage](#move) 
* [List Deals](#list3) 
* [Watch Deals](#watch3)

### Create a Deal

This action module creates a new deal.

You specify information about the deal.

The module returns the ID of the deal and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Title </span> </td> 
   <td> <p>Enter the name of the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Description </span> </td> 
   <td> <p>Enter the details of the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Contact ID</span> </td> 
   <td> <p> Select the Contact ID to assign the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Pipeline ID </span> </td> 
   <td> <p>Select the Pipeline ID for the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Stage </span> </td> 
   <td> <p>Enter the stage name of the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Owner ID</span> </td> 
   <td> <p> Select the Owner ID to assign as the deal owner.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Value </span> </td> 
   <td> <p>Enter the deal value in cents.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Currency </span> </td> 
   <td> <p>Select the currency applicable for the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Percent </span> </td> 
   <td> <p>Enter the deal's percentage.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Status </span> </td> 
   <td> <p>Select the status of the deal:</p> 
    <ul> 
     <li>Open</li> 
     <li>Lost</li> 
     <li>Won</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Custom Fields</span> </p> </td> 
   <td> <p>Add the custom fields.</p> 
    <ul> 
     <li> <p>Custom Field ID</p> <p>Select the Custom Field ID.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Update a Deal

This action module updates an existing deal.

You specify the new information about the deal.

The module returns the ID of the  deal and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Deal ID</span> </td> 
   <td> <p> Select the Deal ID you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Title </span> </td> 
   <td> <p>Enter the name for the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Description</span><![CDATA[	]]></td> 
   <td> <p>Enter the details for the deal.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Contact ID</span> </p> </td> 
   <td> <p>Select the Contact ID to assign the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Pipeline ID</span> </td> 
   <td> <p> Select the Pipeline ID for the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Stage </span> </td> 
   <td> <p>Enter the stage name of the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Owner ID</span> </td> 
   <td> <p> Select the Owner ID to assign as the deal owner.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Value </span> </td> 
   <td> <p>Enter the deal value in cents.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Currency </span> </td> 
   <td> <p>Select the currency applicable for the deal.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Percent </span> </td> 
   <td> <p>Enter the deal's percentage.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Status </span> </td> 
   <td> <p>Select the status of the deal:</p> 
    <ul> 
     <li>Open</li> 
     <li>Lost</li> 
     <li>Won</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Get a Deal

This action module returns a deal.

You specify the ID of the deal.

The module returns the ID of the deal and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">ID </span> </td> 
   <td> <p>Enter the Deal ID whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete a Deal

This action module deletes an existing deal.

You specify the ID of the deal.

The module returns the ID of the  deal and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">ID </span> </td> 
   <td> <p>Select the Deal ID you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Move Details to Another Deal Stage

This action module moves all deals in one stage to another stage.

You specify the IDs of the stage and of the target stage.

The module returns the ID of the  stage and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Stage ID</span> </td> 
   <td> <p> Select the Stage ID whose details you want to move to another stage.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Target stage ID</span> </td> 
   <td> <p> Select the Stage ID to which you want to move the details.</p> </td> 
  </tr> 
 </tbody> 
</table>

### List Deals

This action module retrieves a list of deals.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Limit </span> </td> 
   <td> <p>The maximum number of deals should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Group </span> </td> 
   <td> <p>Enter the group name of the deal you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Stage</span> </td> 
   <td> <p>Enter the stage name of the deals you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Owner </span> </td> 
   <td> <p>Enter the owner name of the deals you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Status </span> </td> 
   <td> <p>Enter the status of the deals you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Due date</span> </td> 
   <td> <p> Enter the due date of the deal that you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Tag </span> </td> 
   <td> <p>Enter the tag names to filter the deals.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Task Type</span> </td> 
   <td> <p> Select the task type of the deal that you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Created Before</span> </td> 
   <td> <p> Enter the date from which the deals that you want to list were created.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Created After</span> </td> 
   <td> <p> Enter the date from which the deals that you want to list were created.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Updated Before</span> </td> 
   <td> <p> Enter the date before which the deals that you want to list were updated.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Updated After</span> </td> 
   <td> <p> Enter the date from which the deals that you want to list were updated.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Organization </span> </td> 
   <td> <p>Select the organization whose deals you want to list.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Deals

This trigger module executes a scenario when a deal is created. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Connection </span> </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Limit </span> </td> 
   <td> <p>The maximum number of deals should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Title </span> </td> 
   <td> <p>Enter the name to filter the deal you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Group </span> </td> 
   <td> <p>Enter the group name of the deals you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Stage </span> </td> 
   <td> <p>Enter the stage name of the deals you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Owner </span> </td> 
   <td> <p>Enter the owner name of the deals you want to watch</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Status </span> </td> 
   <td> <p>Enter the status of the deals you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Due Date</span> </td> 
   <td> <p> Enter the due date of the deal that you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Tag </span> </td> 
   <td> <p>Enter the tag names to filter the deals.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Task Type</span> </td> 
   <td> <p> Select the task type of the deal that you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Created Before</span> </td> 
   <td> <p> Enter the date from which the deals that you want to watch were created.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Created After</span> </td> 
   <td> <p> Enter the date from which the deals that you want to watch were created.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Updated Before</span> </td> 
   <td> <p> Enter the date before which the deals that you want to watch were updated.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Updated After</span> </td> 
   <td> <p> Enter the date from which the deals that you want to watch were updated.</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Organization</span> </td> 
   <td> <p> Select the organization whose deals you want to watch.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ActiveCampaign Campaign modules

* [Get a Campaign](#get5) 
* [Delete a Campaign](#delete3) 
* [List Campaigns](#list4)

### Get a Campaign

This action module retrieves a campaign.

You specify the ID of the campaign.

The module returns the ID of the campaign and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Enter the Campaign ID whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete a Campaign

This action module deletes an existing campaign.

You specify the ID of the campaign.

The module returns the ID of the  campaign and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Enter or map the unique ActiveCampaign ID of the campaign that you want the module to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### List Campaigns

This action module retrieves a list of campaigns.

You specify the highest number of records you want the module to list during each scenario execution cycle.

The module returns the ID of the list and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to list during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ActiveCampaign Task modules

* [Create/Update a Task](#create/u4) 
* [Delete a Task](#delete4) 
* [Watch Tasks](#watch4)

### Create/Update a Task

This action module creates a new task or updates an existing task.

You specify information about the task.

The module returns the ID of the  task and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Owner type</td> 
   <td> <p> Select the task owner type of the task you want to create:</p> 
    <ul> 
     <li>Deal</li> 
     <li>Contact</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Due Date </td> 
   <td> <p>Enter the date by which the task must be completed.</p> </td> 
  </tr> 
  <tr> 
   <td>End Date</td> 
   <td> <p> Enter the date on which the task expires.</p> </td> 
  </tr> 
  <tr> 
   <td>Task Type</td> 
   <td> <p> Select the task type:</p> 
    <ul> 
     <li>Calls</li> 
     <li>Email</li> 
     <li>Lunch</li> 
     <li>Meeting</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Title </td> 
   <td> <p>Enter the name of the task.</p> </td> 
  </tr> 
  <tr> 
   <td>Status </td> 
   <td> <p>Enter the status of the task.</p> </td> 
  </tr> 
  <tr> 
   <td>Note </td> 
   <td> <p>Enter the details of the task.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Enter the Task ID to update.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete a Task

This action module deletes an existing task.

You specify the ID of the task.

The module returns the ID of the  task and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Select the Task ID you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Tasks

This trigger module executes a scenario when a new task is assigned to a deal. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>The maximum number of tasks should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title </td> 
   <td> <p>Enter the name to filter the tasks.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Deal ID</td> 
   <td> <p> Select the Deal ID whose tasks you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status </td> 
   <td> <p>Select the status of the task you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Note </td> 
   <td> <p>Enter the note to filter the task you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Due Date</td> 
   <td> <p> Enter the due date of the task you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Task Type</td> 
   <td> <p> Select the task type you want to watch:</p> 
    <ul> 
     <li>Call</li> 
     <li>Email</li> 
     <li>Lunch</li> 
     <li>Meeting</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## ActiveCampaign Note modules

* [Create a Note](#create5) 
* [Create a Deal Note](#create6)

### Create a Note

This action module adds a note to an activity, a deal, a deal task, or to a subscriber.

You specify the note and the object.

The module returns the ID of the  note and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Note</td> 
   <td>Enter the note text</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Associated Object ID</td> 
   <td>Enter the ID of the object whose note you are creating.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Associated Object Type</td> 
   <td>Select the object type.</td> 
  </tr> 
 </tbody> 
</table>

### Create a Deal Note

This action module creates a new note for a deal.

You specify the note and the ID of the deal.

The module returns the ID of the  note and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Enter the Deal ID to which you want to create a deal note.</p> </td> 
  </tr> 
  <tr> 
   <td>Note </td> 
   <td> <p>Enter the note to add to the deal.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
ActiveCampaign Event modules
-->

  <!--
  Watch Events
  -->

<!--
Watch Events
-->

<!--
I don't see this one
-->

<!--
This trigger module executes a scenario when a new event is fired. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.
-->

<!--
Webhook Name Enter the webhook name. Connection For instructions about connecting your ActiveCampaign account to Workfront Fusion, see Connect Active Campaign to Workfront Fusion in this article. Custom webhook name in ActiveCampaign Enter the webhook name mentioned in the ActiveCampaign. Events Select the events you want to watch: Campaign forwarded Campaign opened Campaign shared Campaign starts sending Contact added Contact note added Contact tag added Contact tag removed Contact unsubscription Contact updated Deal added Deal note added Deal pipeline added Deal stage added Deal task added Deal task completed Deal task type added Deal updated Email bounces Email replies Link clicked List added SMS reply SMS sent SMS unsubscribe Sources Select the sources which causes the events: Run the hooks when a contact triggers the action Run the hooks when an admin user triggers the action Run the hooks when an API call triggers the action Run the hooks when automated systems trigger the action
-->

## ActiveCampaign Automation modules

* [List Automations](#list6) 
* [List Organizations](#list7) 
* [Add a Contact to an Automation](#add3) 
* [Get an Automation a Contact Is In](#get6) 
* [Remove a Contact from an Automation](#remove2) 
* [List All Automations a Contacts Is In](#list8)

### List Automations

This action module retrieves a list of automations.

You specify the highest number of records you want the module to list during each scenario execution cycle.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### List Organizations

This action module retrieves a list of organizations.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>The maximum number of organizations should return during one scenario execution cycle.</p> </td> 
  </tr> <!--
   Name Enter the name of the organization whose details you want to retrieve.
  --> 
 </tbody> 
</table>

### Add a Contact to an Automation

This action module adds a contact to an automation.

You specify the IDs of the contact and of the automation.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Contact ID</p> </td> 
   <td> <p>Select the Contact ID you want to add to an automation.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Automation ID</p> </td> 
   <td> <p>Select the Automation ID to which you want to add the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Get an Automation a Contact Is In

This action module retrieves an automation that contains a contact.

You specify the ID of the contact.

The module returns the ID of the automation and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Enter the Contact ID whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Remove a Contact from an Automation

This action module removes a contact from an automation.

You specify the ID of the contact.

The module returns the ID of the  contact and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Select the Contact ID you want to remove from an automation.</p> </td> 
  </tr> 
 </tbody> 
</table>

### List All Automations a Contacts Is In

This action module retrieves a list of automations that contain a contact.

You specify the maximum number of automations you want to list.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>The maximum number of automations you want listed during 1 execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ActiveCampaign Message modules

### Create a Message

This action module creates a message.

You specify the information for the message.

The module returns the ID of the  message and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>From Name</td> 
   <td> <p> Enter the name from whom the message will be sent.</p> </td> 
  </tr> 
  <tr> 
   <td>From Email </td> 
   <td> <p>Enter the email address from which the message will be sent.</p> </td> 
  </tr> 
  <tr> 
   <td>Reply Email </td> 
   <td> <p>Enter the email address to send the reply</p> </td> 
  </tr> 
  <tr> 
   <td>Subject</td> 
   <td> <p> Enter the message subject.</p> </td> 
  </tr> 
  <tr> 
   <td>Preheader Text </td> 
   <td> <p>Enter the preheader text for the message.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ActiveCampaign Calendar Feed modules

* [Create/Update a Calendar Feed](#create/u5) 
* [Delete a Calendar Feed](#delete5) 
* [Watch Calendar Feeds](#watch6)

### Create/Update a Calendar Feed

This action module creates or updates a calendar feed.

You specify information about the feed.

The module returns the ID of the  feed and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Title </td> 
   <td> <p>Enter the name of the calendar feed.</p> </td> 
  </tr> 
  <tr> 
   <td>Type </td> 
   <td> <p>Enter the calendar feed type:</p> 
    <ul> 
     <li>All</li> 
     <li>Deals</li> 
     <li>Contacts</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Notification flag</td> 
   <td> 
    <ul> 
     <li> Select Yes if this calendar feed has notifications:</li> 
     <li>Yes</li> 
     <li>No</li> 
     <li>Not defined</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Select the Calendar Feed ID you want to update.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete a Calendar Feed

This action module deletes a calendar feed.

You specify the ID of the record.

The module returns the ID of the  calendar feed and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>ID </td> 
   <td> <p>Select the Calendar Feed ID you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Calendar Feeds

This trigger module executes a scenario when a new calendar feed is created or updated.

The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

You specify the maximum number of calendar feeds that you want listed.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>The maximum number of calendar feeds should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
Other ActiveCampaign modules
-->

  <!--
  Make an API Call
  -->

  <!--
  Make a Legacy API Call
  -->

<!--
Make an API Call
-->

<!--
Make a Legacy API Call
-->

## Troubleshooting

The trigger for watching all automations associated with a contact returns dates without time zones. It is a bug in the API, v.2.

### How to connect to an ActiveCampaign List with Webhook

These steps seem really wonky in Alloy article. Test!

<ol> 
 <li value="1">Add a Watch events module to your scenario.</li> 
 <li value="2"> <p>Set up the webhook.</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Connection </td> 
     <td> <p>For instructions about connecting your ActiveCampaign account to Workfront Fusion, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion</a> in this article.</p> </td> 
    </tr> 
    <tr> 
     <td>Custom Webhook Name</td> 
     <td> <p> Enter the name for your webhook. E.g. Contacts Webhook.</p> </td> 
    </tr> 
    <tr> 
     <td>Events </td> 
     <td> <p>Select events that will trigger the webhook.</p> </td> 
    </tr> 
    <tr> 
     <td>Sources </td> 
     <td> <p>Select who initates the webhook, whether it is contact, admin, API, or system processes.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3">Save your setting by clicking the <span class="bold">Save</span> button, then close and save the Watch events webhook module by clicking <span class="bold">OK</span>.</li> 
 <li value="4">Log in to your ActiveCampaign account.</li> 
 <li value="5"> <p>In the <span class="bold">Settings</span> dropdown menu, click <span class="bold">Developer</span>, then click <span class="bold">Manage Webhooks</span>.</p> <!--
   screenshot
  --> </li> 
 <li value="6"> <p>In the Webhook settings fields, click <span class="bold">Edit</span> to open the webhook settings in the ActiveCampaign.</p> <!--
   screenshot
  --> </li> 
 <li value="7"> <p>In the Webhook settings section, in the <span class="bold">List</span> dropdown menu, select the list that you want to work with the Workfront Fusion webhook.</p> <!--
   screenshot
  --> </li> 
 <li value="8">Run your scenario in Workfront Fusion and then <span class="bold">send sample Data</span> so that you can confirm if the webhook catches the correct data.</li> 
 <li value="9"> <p> <span class="bold">Update</span> to save your work.</p> <p class="PinkDraftNote">Screenshot</p> </li> 
</ol>

