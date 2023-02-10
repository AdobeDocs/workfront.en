---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Airtable modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
author: Becky
hidefromtoc: true
---

# Airtable modules

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
In an Adobe Workfront Fusion scenario, you can automate workflows that use Airtable, as well as connect it to multiple third-party applications and services.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Connect Airtable to Workfront Fusion {#connect-airtable-to-workfront-fusion}

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
1. Open Workfront Fusion and the **Create a connection** dialog of the desired module.
1. Enter a name for the connection.
1. Enter the generated API key in the **API token** field.

   ![](assets/airtable-create-a-connection-350x263.png)

1. Click the **Continue** button. The connection is now established.

## Airtable modules and their fields

### Records

* [Create a Record](#create-a-record) 
* [Delete a Record](#delete-a-record) 
* [Get a record](#get-a-record) 
* [Search Records](#search-records) 
* [Update a Record](#update-a-record) 
* [Watch Records](#watch-records)

#### Create a Record {#create-a-record}

This action module creates a new record.

You specify the data you want in the record and where you want it to be stored.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your [Fusion App] account to Workfront Fusion, see <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Select the base that the new record will belong to.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the table that the new record will belong to.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Record</p> </td> 
   <td> <p>Enter the values for the new record. Available fields are based on the table you selected.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Smart links</td> 
   <td> <p>Enable this option to enter names instead of record IDs to fields that link to another table. The record is automatically created in the linked table if there is no match.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Record {#delete-a-record}

This action module deletes a particular record.

You specify the ID and locates of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your [Fusion App] account to Workfront Fusion, see <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Select the base that contains the record you want to delete.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the that contains the record you want to delete.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID</td> 
   <td> <p>Enter or map the unique Airtable ID of the record that you want the module to delete. You can retrieve the ID, for example, using the Search Records module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a record {#get-a-record}

This action module retrieves record details.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your [Fusion App] account to Workfront Fusion, see <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Select the base that contains the table with the record you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td>Table</td> 
   <td> <p> Select the table that contains the record you want to retrieve details for.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID</td> 
   <td> <p> Enter or map the ID of the record you want to retrieve details for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Records {#search-records}

This search module looks for records in an object in Airtable that match the search query you specify.

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your [Fusion App] account to Workfront Fusion, see <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Select the base you want to search for records.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the table you want to search for records.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formula</p> </td> 
   <td> <p>A formula used to filter records. The formula is evaluated for each record, and if the result is not <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>, or <code>#Error!</code> the record is included in the response.</p> <p>If combined with the <code>view</code>, only records in that view which satisfy the formula are returned.</p> <p>For example, to only include records where Name isn't empty, pass in:<code> NOT({Name} = '')</code></p> <p>To learn more, search for information about formula field references in the Airtable support documentation.</p> </td> 
  </tr> 
  <tr> 
   <td>Sort </td> 
   <td> <p>Select the sorting direction and the field you want to sort the results by.</p> </td> 
  </tr> 
  <tr> 
   <td>View </td> 
   <td> <p>Select the view you want to search for records.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Record {#update-a-record}

This action module updates a particular record.

You specify the ID of the record and the new data you want it to contain.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p style="font-weight: normal;">Establish a connection to your Airtable account. (See <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connect Airtable to Workfront Fusion</a>.)</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID </td> 
   <td> <p>Enter or map the unique Airtable ID of the record that you want the module to update. You can retrieve the ID, for example, using the Search Records module.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Record</p> </td> 
   <td> <p>Enter the values for the new record.</p> <p>In order to delete the content of the field, use the erase function. </p> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">screenshot</p>
    --> <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL such as airtable.com or https://airtable.com/universe.</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value; must be equal to or more than 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Smart links</td> 
   <td> <p>Enter names instead of record IDs to fields that link to another table. The record is automatically created in the linked table if there is no match.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Records {#watch-records}

This trigger module executes a scenario when a new record is added or updated in the table. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

>[!NOTE]
>
>In order to use this module, the Created Time field must be created in your table.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your [Fusion App] account to Workfront Fusion, see <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the table you want to watch for new records.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Trigger configuration</p> </td> 
   <td> <p style="font-weight: bold;">Trigger field</p> <p>A <code>Created Time</code> field that is used to sort records. If you do not have a <code>Created Time</code> field in your schema, you need to create one. </p> <p style="font-weight: bold;">Label field</p> <p>A field that is used as a label for a record, for example, in the Choose where to start dialog.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Formula</p> </td> 
   <td> <p>A formula used to filter records. The formula is evaluated for each record, and if the result is not <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>, or <code>#Error!</code> the record is included in the response.</p> <p>If combined with the <code>view</code>, only records in that view which satisfy the formula are returned.</p> <p>For example, to only include records where Name isn't empty, pass in:<code> NOT({Name} = '')</code></p> <p>To learn more, see the information about formula field references in the Airtable support documentation.</p> </td> 
  </tr> 
  <tr> 
   <td>Max Records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Responses

This trigger module starts a scenario when a form is submitted.

>[!NOTE]
>
>This functionality is available only for paid Airtable Pro Plan only.

The webhook URL needs to be generated in Workfront Fusion and then added to form configuration in Airtable.

1. Add the Watch New Responses module to your Workfront Fusion scenario.
1. Generate and copy the webhook URL.

   For instructions, see [Instant triggers (webhooks) in Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Log in to your Airtable account.
1. Open the Base and the table you want to use for the form and create a Form view.
1. Set the form as needed, scroll down the form, and enable the Redirect to URL after the form is submitted option.
1. Enter the Webhook URL generated in step 2 to the displayed dialog box and add the ?record_id={record_id} just after the webhook URL to include the Record ID in the module's output, then click Save. The resulting URL will, for example, look like this:
1. Go back to your Workfront Fusion scenario and run the Watch Responses module only to load fields from Airtable and to be able to map those fields into the other modules.
1. Submit the form in Airtable where the Redirect to URL after the form is submitted option is enabled and Webhook URL added (step 6 above).

   The Watch Responses module is triggered and the desired data are loaded.

1. Add the Airtable > Get a Record module just after the Airtable > Watch Responses module and map the record_id to the Record ID field.

Now, every time the form is submitted, the Watch Responses module in your Workfront Fusion scenario is triggered, and the Get a Record module returns the submitted form details.
